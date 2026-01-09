# Authentication & Authorization

Tài liệu này mô tả cơ chế xác thực (authentication) và phân quyền (authorization) của hệ thống.  
Mục tiêu là đảm bảo **đúng người – đúng quyền – đúng ngữ cảnh**, đồng thời cung cấp nền tảng bảo mật nhất quán cho toàn bộ hệ thống.

---

## 1. Tổng quan
- Mục đích của tài liệu
- Phạm vi áp dụng (toàn hệ thống / module)
- Đối tượng áp dụng (user, system, third-party)
- Nguyên tắc thiết kế bảo mật

---

## 2. Authentication (Xác thực)

### 2.1 Các đối tượng cần xác thực
- Người dùng cuối
- Nhân sự nội bộ
- Hệ thống nội bộ
- Hệ thống bên thứ ba

---

### 2.2 Phương thức xác thực
- Username / password
- Token-based authentication
- OAuth / OpenID Connect
- Single Sign-On (SSO)
- API key / client credential

---

### 2.3 Authentication Flow
- Luồng đăng nhập
- Luồng làm mới phiên / token
- Luồng đăng xuất
- Xác thực nhiều bước (nếu có)

---

### 2.4 Credential Management
- Chính sách mật khẩu
- Lưu trữ credential
- Rotation / expiration
- Reset / recovery

---

## 3. Token & Session Management

### 3.1 Token Type
- Access token
- Refresh token
- Session token
- Machine-to-machine token

---

### 3.2 Token Lifecycle
- Cách cấp token
- Thời gian hiệu lực
- Làm mới token
- Thu hồi token (revoke)
- Hết hạn và xử lý lỗi

---

### 3.3 Session Handling
- Stateless / stateful session
- Session timeout
- Concurrent session handling
- Session invalidation

---

## 4. Authorization (Phân quyền)

### 4.1 Authorization Model
- Role-Based Access Control (RBAC)
- Permission-Based Access Control
- Policy-Based Access Control
- Attribute-Based Access Control (nếu có)

---

### 4.2 Role Definition
- Danh sách role
- Trách nhiệm của từng role
- Phạm vi quyền hạn
- Role mặc định

---

### 4.3 Permission Definition
- Danh sách permission
- Hành động được phép
- Đối tượng tác động
- Điều kiện áp dụng

---

### 4.4 Role – Permission Mapping
- Mapping giữa role và permission
- Kế thừa quyền
- Quyền đặc biệt
- Giới hạn quyền

---

## 5. Access Control

### 5.1 API Access Control
- Bảo vệ endpoint
- Kiểm tra quyền trước khi xử lý
- Quyền truy cập theo HTTP method
- Quy tắc truy cập đặc biệt

---

### 5.2 Resource-Level Access Control
- Kiểm soát quyền theo tài nguyên
- Ownership-based access
- Context-aware access
- Dynamic permission

---

## 6. Security Enforcement Points
- Nơi kiểm tra xác thực
- Nơi kiểm tra phân quyền
- Middleware / filter / gateway
- Consistency enforcement

---

## 7. Error Handling & Security Response
- Lỗi xác thực
- Lỗi phân quyền
- Thông báo lỗi an toàn
- Tránh rò rỉ thông tin nhạy cảm

---

## 8. Auditing & Logging
- Ghi log đăng nhập
- Ghi log thay đổi quyền
- Theo dõi hành vi bất thường
- Truy vết bảo mật

---

## 9. Integration với hệ thống khác
- Identity provider
- External auth service
- Trust relationship
- Token validation từ bên ngoài

---

## 10. Edge Cases & Special Scenarios
- Tài khoản bị khóa
- Quyền tạm thời
- Truy cập khẩn cấp
- Guest / anonymous access

---

## 11. Compliance & Policy
- Chính sách bảo mật
- Tuân thủ pháp lý
- Chính sách lưu trữ thông tin xác thực
- Yêu cầu audit

---

## 12. Testing & Verification
- Kiểm thử xác thực
- Kiểm thử phân quyền
- Security testing
- Penetration testing (nếu có)

---

## 13. Liên kết với tài liệu khác
- Liên kết tới Actors & Roles
- Liên kết tới API Specification
- Liên kết tới Error Handling & Convention
- Liên kết tới Logging, Monitoring, Audit
