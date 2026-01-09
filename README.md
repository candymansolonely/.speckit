# 📘 SpecKit – Project Documentation Index

Thư mục `.speckit` chứa toàn bộ tài liệu đặc tả chính thức cho dự án hoặc module.  
Mục tiêu của SpecKit là chuẩn hóa tài liệu, giảm mơ hồ giữa các bên liên quan và trở thành nguồn tham chiếu lâu dài cho phát triển, vận hành và mở rộng hệ thống.

---

## 🎯 Mục tiêu của SpecKit
- Chuẩn hóa cấu trúc tài liệu dự án
- Giảm tranh cãi giữa PM – Dev – QA – Stakeholder
- Làm rõ phạm vi, trách nhiệm và ranh giới hệ thống
- Hỗ trợ bảo trì, mở rộng và chuyển giao dự án

---

## 📂 Cấu trúc tài liệu trong thư mục

### 1. Introduction & Product Vision
- Tổng quan về sản phẩm
- Vấn đề cần giải quyết
- Mục tiêu kinh doanh và kỹ thuật
- Đối tượng người dùng
- Giá trị cốt lõi của hệ thống
- KPI / tiêu chí thành công

---

### 2. Business Scope & Out of Scope
- Phạm vi nghiệp vụ hệ thống chịu trách nhiệm
- Các chức năng nằm ngoài phạm vi
- Giả định nghiệp vụ
- Giới hạn và ràng buộc của hệ thống

---

### 3. Actors & Roles
- Danh sách actor (người dùng hoặc hệ thống)
- Phân loại actor (human / system)
- Vai trò (role)
- Quyền hạn tổng quát của từng role
- Mối quan hệ giữa actor và chức năng

---

### 4. Functional Requirements
- Danh sách chức năng chính
- Phân nhóm chức năng (core / supporting / admin)
- Actor sử dụng từng chức năng
- Mô tả ngắn gọn hành vi hệ thống
- Điều kiện trước và sau (nếu có)

---

### 5. Non-Functional Requirements
- Hiệu năng (performance)
- Khả năng mở rộng (scalability)
- Bảo mật (security)
- Độ sẵn sàng (availability)
- Khả năng bảo trì (maintainability)
- Logging và audit requirement

---

### 6. System Architecture
- Kiến trúc tổng thể hệ thống
- Phân tầng (layer, module, service)
- Giao tiếp giữa các thành phần
- Luồng dữ liệu chính
- Tích hợp với hệ thống bên ngoài

---

### 7. Database Design
- Danh sách entity / bảng dữ liệu
- Mô tả mục đích từng bảng
- Quan hệ giữa các bảng
- Khóa chính (PK), khóa ngoại (FK)
- Index và constraint quan trọng

---

### 8. API Specification
- Danh sách API endpoint
- HTTP method
- Request format (header, query, body)
- Response format (success / error)
- Authentication requirement
- Quy ước versioning

---

### 9. Authentication & Authorization
- Luồng xác thực người dùng
- Cơ chế cấp và kiểm tra token
- Phân quyền theo role / permission
- Token lifecycle
- Cơ chế revoke và logout

---

### 10. Error Handling & Convention
- Quy ước mã lỗi (error code)
- Cấu trúc response lỗi
- Validation error
- Business error
- System / unexpected error

---

### 11. Technology Stack
- Backend framework
- Frontend framework
- Database
- Cache / Message Queue
- Third-party service
- Version và lý do lựa chọn công nghệ

---

### 12. Deployment & DevOps
- Các môi trường (development / staging / production)
- CI/CD pipeline
- Chiến lược build và release
- Quản lý cấu hình và secrets
- Rollback strategy

---

### 13. Logging, Monitoring, Audit
- Chiến lược logging
- Log level và format
- Monitoring metrics
- Alerting
- Audit log (theo dõi hành động người dùng)

---

### 14. Risk & Assumptions
- Rủi ro kỹ thuật
- Rủi ro nghiệp vụ
- Phụ thuộc bên thứ ba
- Giả định quan trọng
- Phương án giảm thiểu rủi ro

---

### 15. Appendix (Glossary, Diagram)
- Thuật ngữ chuyên môn
- Sơ đồ kiến trúc, luồng nghiệp vụ
- Tài liệu tham khảo
- Ghi chú bổ sung

---

## 📌 Nguyên tắc sử dụng SpecKit
- Mỗi project hoặc module có một thư mục `.speckit` riêng
- Spec được cập nhật song song với code
- Spec là nguồn sự thật duy nhất (single source of truth)
- Mọi thay đổi lớn cần được phản ánh trong tài liệu
