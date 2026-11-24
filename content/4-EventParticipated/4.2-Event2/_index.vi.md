\---

title: "Event 2"
date: 2026-09-29
weight: 2
chapter: false
pre: "  **4.2.**  "
---

# Bài thu hoạch: “AWS Cloud \& AI Day Hanoi 2026”

### Thông tin chung

* **Sự kiện:** AWS Cloud \& AI Day Hanoi 2026
* **Thời gian:** 09:00 – 17:00, ngày 29/09/2026
* **Địa điểm:** Tầng 26, Bitexco Financial Tower, số 2 Hải Triều, TP. Hồ Chí Minh
* **Vai trò:** Người tham dự

### Lý do tham gia và kỳ vọng

* Nắm được vì sao cloud, Generative AI và Agentic AI đang chuyển từ thử nghiệm để đi vào vận hành thực tế tại doanh nghiệp.
* Cập nhật cách xây dựng ứng dụng cloud-native, hạ tầng, nền tảng dữ liệu, định danh cho workload và quản trị AI.
* Xem các doanh nghiệp Việt Nam cùng AWS hiện đại hóa hệ thống ở quy mô lớn như thế nào.
* Tìm hiểu cách bảo mật, quản trị, khả năng quan sát và sự giám sát của con người cần được nâng cấp khi AI ngày càng tự chủ.
* Gắn nội dung sự kiện với hướng đi của bản thân trong lĩnh vực an ninh mạng và bảo mật cloud.

### Khách mời và diễn giả

* **Dr. Werner Vogels** – CTO Amazon.com, diễn giả keynote
* **Eric Yeo** – Tổng giám đốc AWS phụ trách Malaysia, Việt Nam và Đông Dương
* **Mai Le** – Giám đốc Quản lý sản phẩm, Katalon
* **Dr. Jens Lottner** – Tổng giám đốc điều hành Techcombank
* Các chuyên gia, kiến trúc sư và lãnh đạo kỹ thuật từ AWS, Katalon, Techcombank, TCBS, Techcom Life, VPBank và một số đơn vị khác

### Những nội dung đáng chú ý

#### &#x20;Từ kiến trúc cloud-native đến Agentic AI

* Xu hướng không dừng ở việc “chuyển máy chủ lên cloud” mà là xây hệ thống linh hoạt, tự động hóa cao dựa trên container, Kubernetes, serverless, kiến trúc hướng sự kiện và các dịch vụ được quản lý.
* Platform Engineering cùng Internal Developer Platform đưa ra các “Golden Path” có sẵn, nhờ đó lập trình viên ít phải chờ phê duyệt thủ công qua ticket để có hạ tầng.
* Bộ công cụ được nhắc tới gồm Amazon EKS, Crossplane, Terragrunt, Backstage, FluxCD và GitOps, giúp việc triển khai nhất quán, lặp lại được và dễ kiểm toán.

#### &#x20;Đưa AI agent từ bản thử nghiệm vào môi trường thật

Làm ra một agent chạy được thì dễ, giữ cho nó vận hành an toàn mới khó. Có bốn trụ cột cần đáp ứng:

* **Vận hành ổn định:** độ tin cậy, xử lý lỗi, độ trễ và giám sát liên tục.
* **Quản trị dữ liệu:** ai sở hữu dữ liệu, dữ liệu mới đến đâu, chất lượng ra sao và ai được truy cập.
* **An toàn và tin cậy:** kiểm soát danh tính, công cụ được phép gọi, quyền hạn và thông tin nhạy cảm.
* **Con người giám sát:** các hành động có tác động lớn hoặc không thể hoàn tác phải có người chịu trách nhiệm.

Các phiên về Amazon Bedrock, Bedrock AgentCore, Strands Agents, Model Context Protocol (MCP) và mô hình ReAct minh họa cách agent suy luận, tra cứu thông tin, gọi công cụ, nhớ ngữ cảnh và hành động trong phạm vi quyền đã được xác định.

#### &#x20;Định danh, đặc quyền tối thiểu và bảo mật AI

* Thay vì chỉ bỏ access key dài hạn, hướng đi mới là cấp danh tính cho workload để có thể xác minh khi đi qua nhiều ranh giới tin cậy.
* Các cơ chế then chốt gồm AWS IAM, AWS STS (thông tin xác thực ngắn hạn), trust policy, session policy, session tag, source identity và ABAC, áp dụng cho EC2, ECS/Fargate, Lambda, EKS, CI/CD, hệ thống đa tài khoản và cả AI agent.

#### &#x20;Quản trị AI và an toàn dữ liệu

* AI trong doanh nghiệp không chỉ là chọn model mà còn là bài toán dữ liệu và quản trị: độ chính xác, độ mới, nguồn gốc, quyền sở hữu, phân quyền, bằng chứng cho câu trả lời và khả năng truy vết quyết định.
* Chuỗi bảo mật được tóm gọn là: **Danh tính → Dữ liệu → Model → Công cụ → Agent → Hành động → Kiểm toán**.

#### &#x20;Quan sát bảo mật cho ứng dụng AI

Bốn tín hiệu vàng truyền thống (độ trễ, lỗi, lưu lượng, mức bão hòa) cần được mở rộng thêm:

* **Chi phí:** lượng token tiêu thụ và những đợt tăng bất thường.
* **An toàn:** lộ thông tin cá nhân, prompt injection, công cụ chạy sai mục đích.
* **Chất lượng:** hallucination và câu trả lời thiếu chính xác.

Dữ liệu giám sát nên được gộp từ hạ tầng, sự kiện bảo mật, truy cập dữ liệu và hành vi của agent.

#### &#x20;Phát triển phần mềm có AI hỗ trợ nhưng vẫn an toàn

* Kiro và AI-DLC đưa AI vào toàn bộ vòng đời phát triển: lập kế hoạch, thiết kế, viết mã, kiểm thử, tài liệu, triển khai, xử lý nợ kỹ thuật và hiện đại hóa. TCBS báo cáo rút ngắn khoảng 26% thời gian phát triển.
* Điều kiện đi kèm là phải có kiểm chứng, rà soát bảo mật, quản trị, phê duyệt của con người và tích hợp DevSecOps.

#### &#x20;Hiện đại hóa cloud và bảo mật doanh nghiệp

* Các trường hợp từ Techcombank, Techcom Life, TCBS, VPBank và Katalon xoay quanh hiện đại hóa ứng dụng và cơ sở dữ liệu, container hóa, hợp nhất nền tảng dữ liệu, tự động hóa hạ tầng, quan sát hệ thống, tuân thủ và khả năng phục hồi.
* Với yêu cầu dữ liệu phải lưu tại chỗ, AWS giới thiệu Local Zone tại Hà Nội và AWS Outposts thế hệ thứ hai. Bài toán chung là cân bằng giữa bảo mật, tuân thủ, độ tin cậy, hiệu năng, chi phí và sự linh hoạt kinh doanh.

### Bài học rút ra

#### Về tư duy bảo mật

* **Danh tính chính là một ranh giới bảo mật.** Mỗi workload, pipeline, dịch vụ và AI agent nên có danh tính riêng với thông tin xác thực ngắn hạn, cấp quyền tối thiểu.
* **Bảo vệ cả chuỗi AI** từ danh tính đến kiểm toán, và để con người quyết định ở các bước rủi ro cao.
* **Mở rộng giám sát** sang hành vi của AI, truy cập dữ liệu, độ an toàn, chất lượng và chi phí.

#### Về kiến trúc và kỹ thuật

* Ưu tiên hạ tầng có thể tái lập và truy vết (managed service, container, serverless, IaC, GitOps) thay cho việc đăng nhập SSH sửa tay.
* Kết hợp IAM, STS, ABAC và truy cập đa tài khoản với nguồn dữ liệu đáng tin cậy.

#### Về AI và an ninh mạng

* Cần đánh giá agent xem nó làm việc có đúng danh tính, đúng quyền, đúng dữ liệu và có bằng chứng hay không, vì AI mở ra bề mặt tấn công mới như prompt injection, rò rỉ dữ liệu, thừa quyền, hành động trái phép, hallucination và chi phí khó kiểm soát.
* Cloud Security, DevSecOps, AI Security và Security Operations ngày càng gắn chặt với nhau.

### Dự định áp dụng

* Thực hành IAM đặc quyền tối thiểu với credentials ngắn hạn: làm lab nhỏ gồm role, trust policy, session tag, rồi kiểm tra dấu vết trong audit log.
* Mở rộng giám sát: gom log hạ tầng, sự kiện danh tính, telemetry ứng dụng và hoạt động của AI agent; tìm hiểu cách đưa Wazuh và SIEM vào bảo mật cloud và AI.
* Áp dụng GitOps và IaC cho thay đổi hạ tầng, đồng thời đặt ranh giới về quyền, dữ liệu, ghi log và phê duyệt khi thử nghiệm AI agent.
* Dùng công cụ AI để tăng tốc nhưng vẫn rà soát bảo mật và có người duyệt, và nối kiến thức bảo mật mạng/endpoint với bảo mật cloud-native.

### Cảm nhận cá nhân

Buổi sự kiện cho mình cái nhìn rộng về việc hiện đại hóa hệ thống, agentic AI và bảo mật ở quy mô doanh nghiệp.

* Nghe lãnh đạo AWS và các doanh nghiệp chia sẻ giúp mình thấy công nghệ luôn phải đi cùng quản trị, vận hành, bảo mật và thay đổi trong tổ chức.
* Các ví dụ thực tế gắn kiến thức cloud và AI với yêu cầu tuân thủ và quy mô sản xuất thật.
* Tự động hóa mà thiếu quản trị có thể làm rủi ro tăng nhanh không kém năng suất. Hệ thống càng tự chủ thì việc kiểm soát danh tính và phân quyền càng phải chặt.
* Người làm bảo mật không chỉ phát hiện tấn công mà còn phải biết bảo vệ, giám sát và quản trị chính các hệ thống AI.

### Hình ảnh check-in
<img width="400" height="800" alt="image" src="https://github.com/user-attachments/assets/6b879863-b277-4418-9f71-932996846950" />
<img width="400" height="800" alt="image" src="https://github.com/user-attachments/assets/b2ccd5d2-24d1-4ef4-911f-1838e00c2fa7" />



