# Database Design

Tài liệu này mô tả thiết kế cơ sở dữ liệu của hệ thống, bao gồm cấu trúc dữ liệu, mối quan hệ và các nguyên tắc quản lý dữ liệu.  
Nội dung tập trung vào **mô hình dữ liệu**, **toàn vẹn dữ liệu** và **khả năng mở rộng**, không phụ thuộc vào chi tiết triển khai cụ thể.

---

## 1. Tổng quan về Database Design
- Mục đích của thiết kế cơ sở dữ liệu
- Phạm vi áp dụng (toàn hệ thống / module)
- Loại cơ sở dữ liệu sử dụng (relational / NoSQL / hybrid)
- Nguyên tắc thiết kế dữ liệu

---

## 2. Data Model Overview
- Danh sách domain / bounded context
- Các nhóm dữ liệu chính
- Mối quan hệ giữa các domain
- Ranh giới sở hữu dữ liệu (data ownership)

---

## 3. Entity / Table Definition

### 3.1 Entity Structure
Đối với mỗi entity / table, mô tả:
- Tên entity / table
- Mục đích nghiệp vụ
- Mô tả ngắn gọn
- Phạm vi sử dụng

---

### 3.2 Attributes / Columns
- Tên cột
- Kiểu dữ liệu
- Bắt buộc / không bắt buộc
- Giá trị mặc định
- Ý nghĩa nghiệp vụ

---

### 3.3 Primary Key
- Tên khóa chính
- Kiểu khóa (auto-increment, UUID, composite)
- Quy tắc sinh khóa
- Phạm vi duy nhất

---

### 3.4 Foreign Key & Relationships
- Quan hệ giữa các entity
- Kiểu quan hệ (1–1, 1–n, n–n)
- Quy tắc cascade
- Optional / mandatory relationship

---

## 4. Constraints & Validation
- Unique constraint
- Check constraint
- Business rule constraint
- Giới hạn dữ liệu hợp lệ

---

## 5. Indexing Strategy
- Các index chính
- Mục đích của từng index
- Index cho truy vấn đọc
- Index cho truy vấn tìm kiếm
- Trade-off giữa đọc và ghi

---

## 6. Normalization & Denormalization
- Mức độ chuẩn hóa
- Trường hợp denormalization
- Lý do và tác động
- Chiến lược cân bằng hiệu năng

---

## 7. Transaction & Consistency
- Phạm vi transaction
- Isolation level
- Xử lý concurrent update
- Chiến lược đảm bảo nhất quán dữ liệu

---

## 8. Data Lifecycle Management
- Tạo dữ liệu
- Cập nhật dữ liệu
- Xóa dữ liệu (soft delete / hard delete)
- Lưu trữ và archive
- Chính sách retention

---

## 9. Auditing & History
- Audit field (created, updated, deleted)
- Tra
