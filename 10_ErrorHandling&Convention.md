# Error Handling & Convention

Tài liệu này định nghĩa các quy ước xử lý lỗi và phản hồi lỗi thống nhất trong toàn bộ hệ thống.  
Mục tiêu là đảm bảo **nhất quán – dễ hiểu – an toàn – dễ tích hợp** cho tất cả các thành phần sử dụng hệ thống.

---

## 1. Tổng quan
- Mục đích của tài liệu
- Phạm vi áp dụng (API, service nội bộ, background job)
- Đối tượng sử dụng (frontend, backend, integration)
- Nguyên tắc xử lý lỗi

---

## 2. Error Classification
- Validation error
- Business logic error
- Authorization / authentication error
- Resource not found
- System / infrastructure error
- External service error

---

## 3. Error Code Convention

### 3.1 Error Code Structure
- Định dạng mã lỗi
- Phân nhóm mã lỗi
- Quy ước đặt tên
- Tính duy nhất của mã lỗi

---

### 3.2 Error Code Categories
- Nhóm lỗi nghiệp vụ
- Nhóm lỗi hệ thống
- Nhóm lỗi bảo mật
- Nhóm lỗi tích hợp

---

## 4. Error Response Structure

### 4.1 Standard Error Response
- HTTP status code
- Error code
- Error message
- Error detail
- Trace / correlation ID
- Timestamp

---

### 4.2 Validation Error Response
- Danh sách field lỗi
- Thông báo chi tiết cho từng field
- Quy ước hiển thị lỗi

---

## 5. HTTP Status Code Usage
- Mapping lỗi với HTTP status code
- Trường hợp sử dụng 4xx
- Trường hợp sử dụng 5xx
- Tránh lạm dụng status code

---

## 6. Error Handling Flow
- Điểm phát sinh lỗi
- Cách propagate lỗi
- Xử lý lỗi toàn cục
- Fallback và graceful degradation

---

## 7. Logging & Error Tracking
- Log level cho từng loại lỗi
- Nội dung log bắt buộc
- Masking thông tin nhạy cảm
- Liên kết log với error response

---

## 8. Client-Side Error Handling
- Cách frontend xử lý lỗi
- Thông báo người dùng
- Retry logic
- Xử lý lỗi nền (silent error)

---

## 9. Security Considerations
- Tránh lộ thông tin nội bộ
- Thông báo lỗi an toàn
- Phân biệt lỗi public và internal
- Quy tắc expose error message

---

## 10. Internationalization & Localization
- Hỗ trợ đa ngôn ngữ cho lỗi
- Mapping error code với message
- Quy ước quản lý message

---

## 11. Retry & Recovery Strategy
- Điều kiện retry
- Backoff strategy
- Giới hạn retry
- Xử lý khi retry thất bại

---

## 12. Edge Cases & Special Scenarios
- Lỗi không xác định
- Lỗi chain nhiều service
- Partial failure
- Timeout

---

## 13. Testing & Validation
- Test case cho từng loại lỗi
- Kiểm thử error boundary
- Kiểm thử backward compatibility
- Automation testing cho lỗi

---

## 14. Documentation & Maintenance
- Cách cập nhật error catalog
- Versioning error code
- Deprecate error code
- Đồng bộ với API specification

---

## 15. Liên kết với tài liệu khác
- Liên kết tới API Specification
- Liên kết tới Authentication & Authorization
- Liên kết tới Logging, Monitoring, Audit
- Liên kết tới Non-Functional Requirements
