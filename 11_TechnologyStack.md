# Technology Stack

Tài liệu này mô tả toàn bộ các công nghệ, framework, thư viện và công cụ được sử dụng trong dự án.  
Mục tiêu là đảm bảo **nhất quán công nghệ – dễ bảo trì – dễ mở rộng – dễ onboarding** cho các thành viên tham gia.

---

## 1. Tổng quan
- Mục đích lựa chọn công nghệ
- Phạm vi áp dụng
- Định hướng công nghệ dài hạn
- Nguyên tắc chọn tech stack

## 2. Backend Technology
### 2.1. Ngôn ngữ lập trình: C# 12 (.NET 8)
    - Nullable reference types enabled
    - Record types cho DTOs
    - Pattern matching
    - LINQ cho query logic
### 2.2.- Framework chính: .NET 8.0 (LTS)
    - ASP.NET Core 8.0 Web API
    - Minimal APIs cho endpoints đơn giản
    - MVC pattern cho business logic phức tạp
    - Entity Framework Core 8.0 cho ORM
### 2.3. Kiến trúc backend:
    - Core Layer: Domain entities, interfaces
    - Application Layer: Use cases, DTOs, validators
    - Infrastructure Layer: EF Core, external services
    - API Layer: Controllers, middleware, filters
### 2.4. Thư viện hỗ trợ chính:
    - Authentication & Authorization
        + IdentityServer4 / Duende IdentityServer (OpenID Connect & OAuth 2.0)
        + ASP.NET Core Identity (User management)
        + Microsoft.AspNetCore.Authentication.JwtBearer (JWT validation)
    - Validation & Mapping
        + FluentValidation 11.x (Request validation)
        + AutoMapper 13.x (Object mapping)
    - Security
        + BCrypt.Net-Next (Password hashing)
        + System.IdentityModel.Tokens.Jwt (JWT handling)
    - Utilities
        + Serilog 3.x (Structured logging)
        + MediatR 12.x (CQRS pattern - optional)
        + Polly 8.x (Resilience & retry policies)

## 3. Frontend Technology
### 3.1. Ngôn ngữ lập trình: TypeScript 5.3+
    - Strict mode enabled
    - Interfaces cho type safety
    - Enums cho constants
### 3.2. Framework / library: Angular 19
    - Standalone components (mặc định)
    - Signals cho state management
    - SSR (Server-Side Rendering) optional
### 3.3. Kiến trúc frontend: Standard alone
  src/
  ├── app/
  │   ├── core/          # Singleton services, guards, interceptors
  │   ├── shared/        # Shared components, directives, pipes
  │   ├── features/
  │   │   ├── auth/      # Login, register, forgot-password
  │   │   ├── user/      # User profile, settings
  │   │   └── admin/     # Admin panel
### 3.4. State management
    - Angular Signals (built-in)
    - RxJS 7.x (Reactive programming)
    - NgRx (nếu cần state phức tạp - optional) 
### 3.5. UI / component library
    - Angular Material 19 (Primary UI framework)
    - Tailwind CSS 3.x (Utility-first CSS)
    - PrimeNG (alternative - nếu cần rich components)

## 4. Mobile Technology (nếu có)
- Comming soon

## 5. Database & Storage: 
### 5.1. Database chính:
    - PostgreSQL 16.x
        + JSONB cho flexible data
        + Full-text search capabilities
        + Row-level security cho multi-tenancy
        + Partitioning cho audit logs
### 5.2. Database phụ / read replica
### 5.3. Caching system
    - Redis 7.x
        + Session storage
        + Token blacklist (logout, revocation)
        + Rate limiting counters
        + OTP codes (2FA)
### 5.4. Object / file storage
    - MinIO (S3-compatible, self-hosted)
        + User avatars
        + Document storage
        + Backup storage
    - Azure Blob Storage / AWS S3 (production alternative)
### 5.5. Search engine
    - Elasticsearch (nếu cần search phức tạp)

## 6. Messaging & Async Processing
### 6.1. Message broker
    - RabbitMQ 3.x (Recommended)
        + Email queue
        + Notification queue
        + Audit log processing
    - MassTransit (abstraction layer cho RabbitMQ)
### 6.2. Event streaming
    - Apache Kafka (nếu cần event sourcing - future)
### 6.3. Background job / worker
    - 
### 6.4. Scheduling

---

## 7. Authentication & Authorization Technology
- Identity provider
- Token mechanism
- RBAC / ABAC / Policy engine
- Single Sign-On (SSO)

---

## 8. Infrastructure & Cloud
- Cloud provider / On-premise
- Compute service
- Network & load balancing
- Container / orchestration

---

## 9. DevOps & CI/CD Tools
- Source control
- CI/CD pipeline
- Build tools
- Deployment strategy

---

## 10. Monitoring, Logging & Observability
- Logging stack
- Metrics & monitoring
- Tracing
- Alerting

---

## 11. Security Tools
- Secret management
- Vulnerability scanning
- Dependency scanning
- Security monitoring

---

## 12. Development Tools
- IDE / editor
- Code formatting & linting
- API testing
- Database tools

---

## 13. Testing Tools
- Unit testing
- Integration testing
- End-to-end testing
- Performance testing

---

## 14. Third-Party Services
- Payment
- Notification
- Analytics
- External APIs

---

## 15. Versioning & Compatibility
- Versioning strategy
- Backward compatibility
- Deprecation policy
- Upgrade guideline

---

## 16. Constraints & Trade-offs
- Công nghệ bị loại trừ
- Lý do lựa chọn
- Hạn chế đã biết
- Kế hoạch thay thế trong tương lai

---

## 17. Liên kết với tài liệu khác
- System Architecture
- Deployment & DevOps
- Logging, Monitoring, Audit
- Non-Functional Requirements
