---

title: "Blog 1"
date: 2026-11-22
weight: 1
chapter: false
pre: " <b> 3.1. </b>  "
---

# DOES SQS FIFO REALLY GUARANTEE “EXACTLY-ONCE PROCESSING”?

An interesting scenario when studying asynchronous systems on AWS: an application receives the event “Order #1042 has been created”. AWS Lambda processes the message from Amazon SQS FIFO and writes to DynamoDB successfully, but the function times out just before it removes the message from SQS. The same message is then received again. If we already use a FIFO queue, why can reprocessing still happen? This post clarifies the difference between duplicate-send prevention, order preservation, and preventing duplicate business effects, based on the AWS Documentation.

Key points to remember:

* **Standard Queue** offers very high throughput and at-least-once delivery, but messages may be received more than once or out of order. **FIFO Queue** supports ordering within each `MessageGroupId` and message deduplication; different groups can be processed in parallel.
* SQS FIFO's “exactly-once” is duplicate-send prevention at the messaging layer. It does **not** mean the whole business logic in Lambda runs exactly once.
* **Deduplication has only a 5-minute window:** if a producer resends the same `MessageDeduplicationId` within 5 minutes, SQS does not add another copy to the queue. If it is resent after that, the message may be treated as new.
* With content-based deduplication enabled, SQS generates the deduplication ID from the SHA-256 of the **message body**, not including message attributes. So changing attributes does not make a different message for deduplication purposes.
* **Lambda + SQS can still process duplicates:** event source mappings have at-least-once semantics. If processing fails or times out, the message reappears after the visibility timeout and is received again, even though the data was already written successfully.
* **Idempotency** means performing the same request multiple times still gives the same business result as performing it once. For example, use DynamoDB `PutItem` with `ConditionExpression: attribute\_not\_exists(eventId)` so a later attempt does not overwrite the existing item.
* A `PutItem` condition only prevents duplicate writes for that item; it does not create end-to-end exactly-once. If a workflow also sends emails, calls a payment API, or updates multiple systems, you need additional transactions/outbox, a processing state, or downstream API idempotency.
* **Retry and partial batch response:** by default, if one message in a batch fails, the whole batch may be retried. Enable `ReportBatchItemFailures` to report only the failed messages. For FIFO, stop after the first failure and report all unprocessed messages as well, so ordering is not broken.
* **Dead-Letter Queue (DLQ):** configure a redrive policy with `maxReceiveCount` to move repeatedly failing messages to a DLQ; a FIFO source queue must use a FIFO DLQ. A DLQ helps isolate and investigate failures, but it can break strict business ordering when reprocessing and does not guarantee messages will eventually succeed on their own.
* **4 questions when designing an async system:**

  1. Must events be processed in order within each group? If so, `MessageGroupId` must represent the right business flow, for example `orderId`.
  2. If a message reappears after 5 minutes or Lambda retries, is it safe to run the logic again?
  3. Do the visibility timeout, batch failure handling, and retry policy fit the real processing time?
  4. If a message fails permanently, how will the operations team detect it, handle it, and redrive the DLQ?

Conclusion: “exactly-once delivery/deduplication” at the messaging layer is different from “exactly-once business effect” at the application layer. A reliable workflow needs FIFO semantics, visibility timeout, retry/DLQ, idempotency, and side-effect control designed together.

### 


https://www.facebook.com/share/p/1BmMVcWPia/

