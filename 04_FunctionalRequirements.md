# Functional Requirements

Tài liệu này mô tả các chức năng mà hệ thống phải cung cấp nhằm đáp ứng nhu cầu nghiệp vụ.  
Nội dung tập trung vào **hành vi của hệ thống** thay vì chi tiết kỹ thuật triển khai.

---

## 1. Tổng quan về Functional Requirements
- Mục đích của tài liệu
- Phạm vi chức năng được mô tả
- Mối liên hệ với Business Scope & Actors & Roles
- Nguyên tắc mô tả chức năng (rõ ràng, không mơ hồ, kiểm chứng được)

---

## 2. Phân loại chức năng

### 2.1 Core Features
- Các chức năng cốt lõi của hệ thống
- Chức năng bắt buộc để hệ thống vận hành
- Chức năng trực tiếp tạo giá trị nghiệp vụ

---

### 2.2 Supporting Features
- Các chức năng hỗ trợ cho core features
- Chức năng cải thiện trải nghiệm hoặc vận hành
- Chức năng không ảnh hưởng đến logic nghiệp vụ chính

---

### 2.3 Administrative & System Features
- Chức năng dành cho quản trị viên
- Chức năng cấu hình hệ thống
- Chức năng phục vụ vận hành và bảo trì

---

## 3. Cấu trúc mô tả một chức năng

### 3.1 Thông tin chung
- Tên chức năng
- Mã chức năng (nếu có)
- Nhóm chức năng
- Độ ưu tiên (high / medium / low)
- Actor sử dụng
- Tần suất sử dụng

---

### 3.2 Mô tả chức năng
- Mục đích chức năng
- Hành vi mong muốn của hệ thống
- Kết quả đầu ra
- Giá trị nghiệp vụ mang lại

---

### 3.3 Luồng xử lý chính (Main Flow)
- Điều kiện bắt đầu
- Các bước xử lý chính
- Kết quả thành công

---

### 3.4 Luồng thay thế (Alternative Flow)
- Các trường hợp ngoại lệ
- Các nhánh xử lý phụ
- Điều kiện chuyển luồng

---

### 3.5 Điều kiện trước và sau
- Pre-condition
- Post-condition
- Trạng thái hệ thống sau khi hoàn thành

---

### 3.6 Quy tắc nghiệp vụ (Business Rules)
- Quy tắc ràng buộc
- Điều kiện hợp lệ dữ liệu
- Giới hạn nghiệp vụ

---

## 4. Actor – Function Mapping
- Mapping giữa actor và chức năng
- Mức độ truy cập (full / limited / read-only)
- Điều kiện đặc biệt khi sử dụng chức năng

---

## 5. Chức năng liên quan đến dữ liệu
- Tạo mới dữ liệu
- Cập nhật dữ liệu
- Xóa dữ liệu
- Truy vấn và tìm kiếm
- Ảnh hưởng tới các entity khác

---

## 6. Chức năng liên quan đến tích hợp
- Gửi dữ liệu sang hệ thống khác
- Nhận dữ liệu từ hệ thống khác
- Đồng bộ dữ liệu
- Xử lý lỗi tích hợp

---

## 7. Chức năng liên quan đến bảo mật
- Yêu cầu xác thực
- Yêu cầu phân quyền
- Giới hạn truy cập theo vai trò
- Điều kiện đặc biệt về bảo mật

---

## 8. Trạng thái và hành vi hệ thống
- Trạng thái hệ thống trước và sau chức năng
- Trạng thái đối tượng nghiệp vụ
- Thay đổi trạng thái theo luồng xử lý

---

## 9. Tiêu chí chấp nhận (Acceptance Criteria)
- Điều kiện được xem là hoàn thành chức năng
- Trường hợp thành công
- Trường hợp thất bại
- Điều kiện kiểm thử

---

## 10. Liên kết với tài liệu khác
- Liên kết tới Business Scope & Out of Scope
- Liên kết tới Actors & Roles
- Liên kết tới Non-Functional Requirements
- Liên kết tới API Specification
- Liên kết tới Database Design
