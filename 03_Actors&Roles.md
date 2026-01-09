# Actors & Roles

Tài liệu này mô tả các đối tượng tham gia vào hệ thống (actor), vai trò (role) của họ và mức độ tương tác với hệ thống.  
Nội dung trong file này là nền tảng cho thiết kế chức năng, phân quyền, bảo mật và trải nghiệm người dùng.

---

## 1. Tổng quan về Actors
- Mục đích của việc xác định actor
- Phạm vi áp dụng (người dùng, hệ thống nội bộ, hệ thống bên ngoài)
- Nguyên tắc phân loại actor trong hệ thống

---

## 2. Phân loại Actors

### 2.1 Human Actors (Người dùng)
- Người dùng cuối
- Nhân sự nội bộ
- Quản trị viên
- Đối tác / khách hàng

---

### 2.2 System Actors (Hệ thống)
- Hệ thống nội bộ
- Hệ thống bên thứ ba
- Dịch vụ tự động / background job
- Scheduled task / integration service

---

## 3. Danh sách Actors

### 3.1 Actor Definition
Đối với mỗi actor, mô tả:
- Tên actor
- Loại actor (human / system)
- Mô tả ngắn gọn
- Mục tiêu khi tương tác với hệ thống
- Tần suất sử dụng
- Mức độ quan trọng

---

### 3.2 Actor Context
- Môi trường sử dụng (web, mobile, API)
- Thiết bị / nền tảng
- Điều kiện truy cập
- Phụ thuộc bên ngoài (nếu có)

---

## 4. Roles (Vai trò)

### 4.1 Danh sách Roles
- Tên role
- Mô tả trách nhiệm chính
- Phạm vi quyền hạn
- Mức độ đặc quyền (low / medium / high)

---

### 4.2 Quan hệ Actor – Role
- Một actor có thể có nhiều role hay không
- Điều kiện gán role
- Role mặc định
- Trường hợp đặc biệt (temporary / system role)

---

## 5. Permissions (Quyền hạn)

### 5.1 Permission Definition
- Tên permission
- Mô tả hành động được phép
- Đối tượng tác động
- Phạm vi áp dụng

---

### 5.2 Role – Permission Mapping
- Role nào có permission nào
- Quyền đọc / ghi / sửa / xóa
- Quyền nghiệp vụ đặc biệt
- Nguyên tắc kế thừa quyền

---

## 6. Actor Interaction

### 6.1 Actor – Feature Mapping
- Actor nào sử dụng chức năng nào
- Mức độ truy cập (full / limited / read-only)
- Điều kiện truy cập chức năng

---

### 6.2 Actor – System Interaction
- Actor tương tác trực tiếp hay gián tiếp
- Hình thức tương tác (UI, API, event)
- Tần suất và thời điểm tương tác

---

## 7. Authentication & Access Level
- Yêu cầu xác thực cho từng actor
- Phương thức xác thực (password, token, SSO)
- Mức độ truy cập hệ thống
- Hạn chế và điều kiện đặc biệt

---

## 8. Edge Cases & Special Scenarios
- Actor ẩn / actor hệ thống
- Actor không xác thực
- Actor bị hạn chế quyền
- Trường hợp actor bị khóa hoặc thu hồi quyền

---

## 9. Liên kết với tài liệu khác
- Liên kết tới Functional Requirements
- Liên kết tới Authentication & Authorization
- Liên kết tới API Specification
- Liên kết tới Error Handling & Convention
