# Logging, Monitoring, Audit

Tài liệu này mô tả chiến lược ghi log, giám sát hệ thống và kiểm toán hoạt động.  
Mục tiêu là đảm bảo **quan sát được hệ thống – phát hiện sự cố sớm – truy vết chính xác – tuân thủ và kiểm soát rủi ro**.

---

## 1. Tổng quan
- Mục đích của logging, monitoring và audit
- Phạm vi áp dụng
- Đối tượng sử dụng (dev, DevOps, SRE, security, audit)
- Nguyên tắc thiết kế

---

## 2. Logging Strategy

### 2.1 Log Levels
- Quy ước các mức log
- Mục đích sử dụng từng level
- Khi nào không nên log

---

### 2.2 Log Structure
- Định dạng log
- Trường thông tin bắt buộc
- Correlation / trace ID
- Timestamp & timezone

---

### 2.3 Log Content Guidelines
- Log nghiệp vụ
- Log kỹ thuật
- Mask dữ liệu nhạy cảm
- Tránh log dư thừa

---

### 2.4 Log Lifecycle
- Thu thập log
- Lưu trữ
- Retention policy
- Xóa log

---

## 3. Monitoring Strategy

### 3.1 Metrics Classification
- System metrics
- Application metrics
- Business metrics
- Custom metrics

---

### 3.2 Health Check & Heartbeat
- Liveness check
- Readiness check
- Dependency health
- Self-healing signal

---

### 3.3 Alerting Strategy
- Ngưỡng cảnh báo
- Severity level
- Alert routing
- Alert fatigue control

---

### 3.4 Dashboard & Visualization
- Dashboard cho vận hành
- Dashboard cho business
- Quy ước hiển thị
- Truy cập và phân quyền

---

## 4. Distributed Tracing
- Trace context propagation
- Span definition
- End-to-end tracing
- Phân tích bottleneck

---

## 5. Audit Logging

### 5.1 Audit Scope
- Đối tượng audit
- Hành vi cần audit
- Mức độ chi tiết
- Audit theo vai trò

---

### 5.2 Audit Log Structure
- Actor
- Action
- Target
- Thời gian
- Kết quả hành động

---

### 5.3 Audit Log Storage
- Vị trí lưu trữ
- Tính bất biến
- Retention & archiving
- Truy xuất audit log

---

## 6. Security & Compliance
- Tuân thủ tiêu chuẩn
- Phát hiện hành vi bất thường
- Chống chỉnh sửa log
- Quy định truy cập log

---

## 7. Incident Investigation
- Quy trình điều tra sự cố
- Truy vết từ log & trace
- Timeline reconstruction
- Root cause analysis

---

## 8. Performance & Cost Considerations
- Chi phí lưu trữ log
- Sampling strategy
- Tối ưu hóa metrics
- Cân bằng chi phí và độ chi tiết

---

## 9. Testing & Validation
- Kiểm thử logging
- Kiểm thử alert
- Chaos testing
- Validation dashboard

---

## 10. Operation & Maintenance
- Vận hành hệ thống quan sát
- Nâng cấp công cụ
- Backup & recovery
- Đánh giá định kỳ

---

## 11. Constraints & Risks
- Giới hạn hệ thống giám sát
- Rủi ro mất log
- Độ trễ giám sát
- Kế hoạch giảm thiểu

---

## 12. Liên kết với tài liệu khác
- Error Handling & Convention
- Deployment & DevOps
- Security
- Risk & Assumptions
