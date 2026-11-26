---

title: "Event 3"
date: 2026-10-24
weight: 3
chapter: false
pre: " <b> 4.3. </b>  "
---

# Bài thu hoạch sự kiện: “First Cloud AI Journey: Weekly Meet Up”

* **Tên sự kiện:** First Cloud AI Journey: Weekly Meet Up
* **Thời gian:** 09:00 – 12:00, Thứ Bảy, 24/10/2026
* **Địa điểm:** Lầu 26, Bitexco Financial Tower, TP. Hồ Chí Minh
* **Vai trò:** Khách tham dự

### Mục đích tham gia

* Tiếp thu kinh nghiệm triển khai Cloud và AI Agents ngoài thực tế, được chia sẻ trực tiếp bởi các Tech Lead và kỹ sư đang làm việc tại doanh nghiệp
* Tìm hiểu những góc nhìn thực chiến, từ Voice AI tiếng Việt có độ trễ thấp, việc dùng chung tài nguyên giữa nhiều tài khoản, kiểm thử bảo mật ngay từ đầu cho đến nền tảng đưa Agent vào môi trường production
* Vận dụng các bài học về tối ưu chi phí, quản lý context/memory, các lớp bảo vệ an toàn và cách vận hành agent liên tục 24/7 vào lộ trình học của bản thân
* Rèn luyện sự tự tin khi giao lưu, chủ động kết nối và nỗ lực học hỏi hơn nữa cùng cộng đồng

### Danh sách diễn giả

* **Anh Kiệt Trần** – Revve AI
* **Anh Long Huỳnh** – Styl Solution
* **Anh Thịnh Nguyễn** – Styl Solution
* **Anh Xuân An** – Trưởng nhóm AWS Student Builder Group HCMUTE
* **Anh Khoa Kiều** – Tech Lead tại ACB
* **Anh Nghi Danh** – AWS Community Builder

### Nội dung đáng chú ý

#### 1\. Hear, Think, Speak – Dựng tổng đài Voice-AI tiếng Việt trên AWS (Anh Kiệt Trần – Revve AI)

* Tìm hiểu kiến trúc **Voice AI** cùng bài toán rút ngắn thời gian phản hồi còn khoảng **\~1.8s**, giúp cuộc hội thoại diễn ra liền mạch
* Phần demo trực tiếp cho thấy hệ thống AI tự gọi điện phỏng vấn sơ bộ ứng viên **Cloud Engineer** bằng tiếng Việt, rất tự nhiên và gây ấn tượng mạnh

#### 2\. AWS Resource Access Manager (Anh Long Huỳnh – Styl Solution)

* Trình bày cách chia sẻ tài nguyên một cách an toàn giữa các tài khoản thuộc cùng **AWS Organization**
* Giải pháp này giúp giảm chi phí, quản lý mạng tập trung và phối hợp **IAM policy** với **SCP** để mọi người đều không thể vượt quá giới hạn quyền được cấp

#### 3\. AWS Pentest with AWS Continuum / Security Agent (Anh Thịnh Nguyễn – Styl Solution)

* Giới thiệu bộ giải pháp đánh giá an toàn hạ tầng ngay từ giai đoạn đầu: rà soát code **Terraform**, tích hợp thẳng vào **GitLab/GitHub PR** để phát hiện lỗi sớm
* Để **Security Agent** đóng vai người dùng thật nhằm pentest tự động trên môi trường **SIT/UAT** trước khi triển khai chính thức

#### 4\. Amazon Bedrock AgentCore (Anh Xuân An – Trưởng nhóm AWS Student Builder Group HCMUTE)

* Đem lại bức tranh tổng quan về hai thành phần giúp đưa Agent vào production:

  * **Agent Runtime**: Chạy **MicroVM** trên **EC2 Spot** để tiết giảm chi phí tính toán
  * **Memory**: Chia tầng giữa **Short-term** (đồng bộ) và **Long-term** (bất đồng bộ) để Agent nắm bắt ngữ cảnh người dùng sâu hơn

#### 5\. Kiro Crew (Anh Khoa Kiều – Tech Lead tại ACB \& Anh Nghi Danh – AWS Community Builder)

* Đây là session mình tâm đắc nhất, xoay quanh bài toán cho AI Agent hoạt động **24/7** để hỗ trợ review code và kiểm tra hệ thống, kèm phần hỏi đáp kỹ thuật rất cuốn hút ở cuối buổi:

  * **Artifacts**: Tự động thu thập dữ liệu tuyển dụng thực tế và vẽ biểu đồ thống kê trực quan ngay trong khung chat
  * **Quản lý Context Window**: Cơ chế **Auto Compact** kích hoạt khi ngữ cảnh đạt ngưỡng **70–90%**, cùng tính năng **Break down context** để xem chi tiết lượng token mà từng thành phần tiêu tốn
  * **Quản lý Memory \& Guardrails**: Dọn các memory cũ để chi phí không bị đội lên, đồng thời dựng lớp bảo vệ ngăn AI tự ý xóa hạ tầng hoặc làm lộ secret/credential của máy chủ

### Những bài học rút ra

#### Quản lý đa tài khoản \& Kiểm tra bảo mật từ sớm

* **Giới hạn quyền khi dùng chung tài nguyên**: Phối hợp **IAM policy** và **SCP** khi chia sẻ tài nguyên trong **AWS Organization** giúp tối ưu chi phí, quản trị mạng tập trung và giữ quyền hạn trong đúng phạm vi
* **Phát hiện lỗi hạ tầng trước khi triển khai thật**: Rà soát mã **Terraform** trực tiếp trên **GitLab/GitHub PR** và chạy pentest tự động bằng **Security Agent** trên **SIT/UAT** giúp nhận diện rủi ro sớm

#### Đưa Agent vào Production, Kiểm soát chi phí \& Lớp bảo vệ an toàn

* **Runtime và bộ nhớ nhiều tầng**: Để đưa Agent vào production, cần chạy **MicroVM** trên **EC2 Spot** nhằm tiết kiệm chi phí, đồng thời kết hợp bộ nhớ **Short-term** đồng bộ với **Long-term** bất đồng bộ để duy trì ngữ cảnh sâu
* **Khống chế chi phí và rủi ro khi chạy 24/7**: Quản lý context window (**Auto Compact**, **Break down context**), dọn memory cũ và đặt guardrails giúp chi phí không phình to, tránh xóa nhầm hạ tầng hay lộ secret/credential

### Vận dụng vào công việc

* **Phối hợp IAM policy và SCP**: Dùng cơ chế giới hạn quyền tối đa khi chia sẻ tài nguyên giữa các tài khoản trong **AWS Organization**
* **Đưa kiểm tra bảo mật lên sớm**: Review **Terraform** ngay trên PR và chạy pentest tự động trên **SIT/UAT** trước khi triển khai thực tế
* **Quản lý context, memory và guardrails cho Agent**: Theo dõi lượng token, dọn memory cũ và thiết lập lớp bảo vệ cho hạ tầng, secret và credential khi làm việc với AI Agent
* **Mạnh dạn giao lưu và chủ động học hỏi**: Rèn sự tự tin khi giao tiếp, tích cực kết nối với diễn giả/bạn bè và cố gắng học hỏi nhiều hơn mỗi ngày

### Cảm nhận về sự kiện

Sáng thứ Bảy 24/10/2026 tại lầu 26, Bitexco Financial Tower, dù chỉ kéo dài từ 9:00 – 12:00 nhưng buổi meet-up để lại rất nhiều kiến thức thực tế và nguồn năng lượng tích cực khi được nghe các anh Tech Lead và kỹ sư chia sẻ về Cloud và AI Agent. Những điểm đáng nhớ gồm:

#### Học hỏi từ các anh Tech Lead và diễn giả

* Phần chia sẻ từ **Revve AI**, **Styl Solution**, **AWS Student Builder Group HCMUTE**, **ACB** và **AWS Community Builder** giúp mình nhận ra kiến thức thực tế rộng và hấp dẫn đến nhường nào.
* **Kiro Crew** là session mình ưng ý nhất, nhất là phần hỏi đáp kỹ thuật về cách tạo **Artifacts**, **Auto Compact**, **Break down context**, dọn memory và thiết lập **Guardrails** cho Agent chạy **24/7**.

#### Tiếp cận kiến trúc và bài toán thực hành

* Được làm quen với những bài toán rất cụ thể: hạ độ trễ **Voice AI** xuống **\~1.8s** cùng demo phỏng vấn sơ bộ **Cloud Engineer** bằng tiếng Việt, **AWS Resource Access Manager** phối hợp **IAM** và **SCP**, kiểm tra **Terraform** trên PR và pentest tự động trên **SIT/UAT**, cùng **Amazon Bedrock AgentCore** (**Agent Runtime** dạng MicroVM trên **EC2 Spot** và **Memory** chia tầng).

#### Kết nối và tinh thần cộng đồng

* Không khí chia sẻ cởi mở tại lầu 26 Bitexco tiếp thêm cho mình nhiều động lực trên chặng đường học Cloud và AI.
* Sau buổi meet-up, mình nhận ra rõ hơn rằng mình cần mạnh dạn giao lưu, chủ động kết nối và nỗ lực học hỏi nhiều hơn nữa.

#### Bài học kinh nghiệm

* Các hệ thống AI và Cloud trong thực tế đòi hỏi sự cân bằng giữa năng lực xử lý (như độ trễ giọng nói, ngữ cảnh sâu), chi phí vận hành và các lớp bảo vệ an toàn.
* Khi để AI Agent chạy lâu dài hoặc **24/7**, việc quản lý context/memory và đặt guardrails để ngăn xóa hạ tầng hay lộ secret/credential là điều then chốt.
* Sự tự tin trong kết nối, tinh thần chủ động và tính kiên trì học hỏi sẽ giúp hành trình Cloud của mình vững vàng và đầy động lực hơn.

#### Một số hình ảnh sự kiện
<img width="2560" height="1920" alt="image" src="https://github.com/user-attachments/assets/dbb2a9e7-e9d5-4f18-b6a8-cc3da658d7bf" />
<img width="1920" height="2560" alt="image" src="https://github.com/user-attachments/assets/561f7ca3-276e-4a2c-b501-cb7de1e3a219" />



> Tổng kết lại, buổi meet-up mang đến rất nhiều kiến thức thực tiễn qua 5 session chất lượng—từ Voice AI, quản lý đa tài khoản đến pentest sớm và guardrails cho Agent—đồng thời tiếp thêm động lực để mình mạnh dạn kết nối và học hỏi nhiều hơn.

