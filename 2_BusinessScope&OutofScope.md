# Business Scope & Out of Scope

Tài liệu này xác định rõ phạm vi nghiệp vụ của hệ thống, bao gồm những gì hệ thống chịu trách nhiệm thực hiện và những gì nằm ngoài phạm vi.  
Mục tiêu là tránh hiểu nhầm, kiểm soát kỳ vọng và hạn chế scope creep trong suốt vòng đời dự án.

---

## 1. Business Scope (Trong phạm vi)

### 1.1 Phạm vi nghiệp vụ tổng quát
- Lĩnh vực nghiệp vụ mà hệ thống phục vụ
- Các nghiệp vụ cốt lõi được hỗ trợ
- Đối tượng nghiệp vụ chính
- Vai trò của hệ thống trong toàn bộ quy trình nghiệp vụ

---

### 1.2 Chức năng thuộc phạm vi
- Danh sách các nhóm chức năng chính
- Mô tả ngắn gọn mục đích của từng nhóm chức năng
- Actor / role sử dụng các chức năng này
- Mức độ ưu tiên (core / important / optional)

---

### 1.3 Quy trình nghiệp vụ được hỗ trợ
- Các luồng nghiệp vụ chính
- Các bước nghiệp vụ mà hệ thống tham gia
- Điểm bắt đầu và kết thúc của mỗi quy trình
- Tương tác với người dùng hoặc hệ thống khác

---

### 1.4 Dữ liệu thuộc phạm vi quản lý
- Các loại dữ liệu hệ thống chịu trách nhiệm lưu trữ
- Dữ liệu được tạo mới, cập nhật hoặc xóa
- Vòng đời dữ liệu (data lifecycle)
- Trách nhiệm về tính toàn vẹn và chính xác dữ liệu

---

### 1.5 Tích hợp trong phạm vi
- Hệ thống bên ngoài được tích hợp
- Mục đích của từng tích hợp
- Dữ liệu trao đổi giữa các hệ thống
- Hình thức tích hợp (API, message, file, webhook)

---

## 2. Out of Scope (Ngoài phạm vi)

### 2.1 Chức năng không được hỗ trợ
- Các chức năng được xác định rõ là không thuộc hệ thống
- Các nghiệp vụ liên quan nhưng không được triển khai
- Các yêu cầu đã bị loại trừ có chủ đích

---

### 2.2 Quy trình nghiệp vụ không xử lý
- Các bước nghiệp vụ diễn ra hoàn toàn bên ngoài hệ thống
- Các quyết định nghiệp vụ không do hệ thống tự động thực hiện
- Các quy trình được xử lý thủ công hoặc bởi hệ thống khác

---

### 2.3 Dữ liệu không thuộc phạm vi
- Loại dữ liệu hệ thống không lưu trữ
- Dữ liệu chỉ được tham chiếu nhưng không quản lý
- Trách nhiệm dữ liệu thuộc về hệ thống hoặc bộ phận khác

---

### 2.4 Tích hợp ngoài phạm vi
- Các hệ thống không tích hợp trong giai đoạn hiện tại
- Các tích hợp có thể xem xét trong tương lai
- Giới hạn về mặt kỹ thuật hoặc nghiệp vụ đối với tích hợp

---

## 3. Assumptions & Constraints

### 3.1 Assumptions (Giả định)
- Giả định về nghiệp vụ
- Giả định về người dùng
- Giả định về dữ liệu
- Giả định về hạ tầng hoặc hệ thống liên quan

---

### 3.2 Constraints (Ràng buộc)
- Ràng buộc về thời gian
- Ràng buộc về nguồn lực
- Ràng buộc về công nghệ
- Ràng buộc pháp lý hoặc tuân thủ

---

## 4. Scope Change Management

- Nguyên tắc thay đổi phạm vi
- Quy trình đề xuất thay đổi
- Cách đánh giá ảnh hưởng của thay đổi
- Cách cập nhật tài liệu SpecKit khi scope thay đổi

---

## 5. Liên kết với tài liệu khác
- Liên kết tới Functional Requirements
- Liên kết tới System Architecture
- Liên kết tới Risk & Assumptions
