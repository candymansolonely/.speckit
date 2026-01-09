# Deployment & DevOps

Tài liệu này mô tả chiến lược triển khai, vận hành và tự động hóa vòng đời phần mềm.  
Mục tiêu là đảm bảo **triển khai ổn định – phát hành nhanh – rollback an toàn – vận hành dễ dàng**.

---

## 1. Tổng quan
- Mục đích của tài liệu
- Phạm vi áp dụng (dev / staging / production)
- Đối tượng sử dụng (dev, DevOps, SRE)
- Nguyên tắc DevOps áp dụng

---

## 2. Environment Strategy
- Danh sách môi trường
- Mục đích của từng môi trường
- Quy ước cấu hình theo môi trường
- Phân tách tài nguyên

---

## 3. Source Control & Branching Strategy
- Hệ thống quản lý mã nguồn
- Quy ước đặt tên branch
- Flow phát triển (Git Flow, Trunk-based, v.v.)
- Quy tắc merge & review

---

## 4. CI Pipeline
- Trigger build
- Các bước build
- Kiểm tra chất lượng mã
- Chạy test tự động
- Artifact management

---

## 5. CD Pipeline
- Chiến lược triển khai
- Các bước deploy
- Approval gate
- Tự động hóa rollback

---

## 6. Build & Packaging
- Build strategy
- Artifact format
- Containerization
- Version tagging

---

## 7. Infrastructure as Code (IaC)
- Công cụ IaC
- Phạm vi quản lý hạ tầng
- Cấu trúc repo IaC
- Quy ước thay đổi hạ tầng

---

## 8. Configuration & Secret Management
- Cách quản lý cấu hình
- Quản lý secrets
- Quy ước đặt tên
- Rotation policy

---

## 9. Deployment Strategy
- Rolling update
- Blue–Green deployment
- Canary release
- Zero-downtime deployment

---

## 10. Rollback & Recovery
- Điều kiện rollback
- Quy trình rollback
- Data rollback
- Disaster recovery

---

## 11. Database Deployment & Migration
- Chiến lược migration
- Versioning schema
- Backward compatibility
- Rollback migration

---

## 12. Monitoring & Alerting in Deployment
- Health check
- Deployment metrics
- Alert trong quá trình deploy
- Post-deployment verification

---

## 13. Security in DevOps
- Secure pipeline
- Access control
- Artifact integrity
- Audit deployment

---

## 14. Release Management
- Quy trình phát hành
- Release note
- Versioning
- Feature flag

---

## 15. Operational Procedures
- On-call process
- Incident response
- Runbook
- Post-mortem

---

## 16. Constraints & Risks
- Giới hạn hạ tầng
- Rủi ro triển khai
- Điểm nghẽn DevOps
- Kế hoạch cải tiến

---

## 17. Liên kết với tài liệu khác
- System Architecture
- Technology Stack
- Logging, Monitoring, Audit
- Risk & Assumptions
