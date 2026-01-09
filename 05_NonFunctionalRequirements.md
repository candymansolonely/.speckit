# Non-Functional Requirements

Tài liệu này mô tả các yêu cầu phi chức năng của hệ thống, tập trung vào chất lượng, hiệu năng, bảo mật và khả năng vận hành.  
Các yêu cầu trong tài liệu này áp dụng xuyên suốt toàn bộ hệ thống và có ảnh hưởng trực tiếp đến kiến trúc và công nghệ được lựa chọn.

---

## 1. Tổng quan về Non-Functional Requirements
- Mục đích của tài liệu
- Phạm vi áp dụng (toàn hệ thống / module cụ thể)
- Nguyên tắc định nghĩa NFR (có thể đo lường, kiểm chứng được)
- Mối liên hệ với kiến trúc và thiết kế hệ thống

---

## 2. Performance (Hiệu năng)
- Thời gian phản hồi mong muốn
- Throughput (số lượng request / giao dịch)
- Độ trễ chấp nhận được
- Giới hạn tài nguyên (CPU, memory, IO)
- Yêu cầu về xử lý đồng thời (concurrency)

---

## 3. Scalability (Khả năng mở rộng)
- Khả năng scale theo chiều ngang
- Khả năng scale theo chiều dọc
- Giới hạn hiện tại và mục tiêu mở rộng
- Chiến lược scale theo tải
- Các thành phần cần ưu tiên mở rộng

---

## 4. Availability & Reliability (Độ sẵn sàng & tin cậy)
- Uptime mục tiêu
- Thời gian downtime chấp nhận được
- Chiến lược failover
- Cơ chế retry và recovery
- Khả năng chịu lỗi (fault tolerance)

---

## 5. Security (Bảo mật)
- Yêu cầu xác thực
- Yêu cầu phân quyền
- Bảo vệ dữ liệu (at rest / in transit)
- Quản lý secret và credential
- Phòng chống các rủi ro bảo mật phổ biến

---

## 6. Data Integrity & Consistency
- Đảm bảo toàn vẹn dữ liệu
- Quy tắc nhất quán dữ liệu
- Xử lý giao dịch (transaction)
- Chiến lược rollback
- Kiểm soát xung đột dữ liệu

---

## 7. Maintainability (Khả năng bảo trì)
- Khả năng đọc và hiểu code
- Chuẩn code và convention
- Khả năng mở rộng tính năng
- Chiến lược refactor
- Tài liệu hóa và comment

---

## 8. Observability (Logging, Monitoring, Tracing)
- Logging level và format
- Monitoring metrics
- Distributed tracing (nếu có)
- Alerting
- Khả năng debug và phân tích sự cố

---

## 9. Compatibility & Portability
- Tương thích trình duyệt / thiết bị
- Tương thích hệ điều hành
- Khả năng deploy trên nhiều môi trường
- Phụ thuộc nền tảng

---

## 10. Compliance & Legal
- Yêu cầu tuân thủ pháp lý
- Quy định về dữ liệu người dùng
- Chính sách bảo mật và quyền riêng tư
- Yêu cầu audit và truy vết

---

## 11. Usability & Accessibility
- Yêu cầu về trải nghiệm người dùng
- Tính dễ sử dụng
- Khả năng tiếp cận (accessibility)
- Hỗ trợ đa ngôn ngữ (nếu có)

---

## 12. Backup & Disaster Recovery
- Chiến lược sao lưu dữ liệu
- Tần suất backup
- Thời gian phục hồi (RTO)
- Mức độ mất dữ liệu chấp nhận được (RPO)
- Kịch bản khôi phục sự cố

---

## 13. Constraints & Limitations
- Giới hạn kỹ thuật
- Giới hạn hạ tầng
- Giới hạn ngân sách
- Giới hạn thời gian

---

## 14. Verification & Acceptance
- Cách kiểm chứng từng yêu cầu
- Chỉ số đo lường
- Điều kiện được xem là đạt yêu cầu
- Liên kết tới test plan

---

## 15. Liên kết với tài liệu khác
- Liên kết tới System Architecture
- Liên kết tới Technology Stack
- Liên kết tới Deployment & DevOps
- Liên kết tới Logging, Monitoring, Audit
