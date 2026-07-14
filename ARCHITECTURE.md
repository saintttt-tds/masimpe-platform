masimpe-platform/
│
├── 📄 README.md
├── 📄 LICENSE
├── 📄 .gitignore
├── 📄 .dockerignore
├── 📄 .env.example
├── 📄 .eslintrc.js
├── 📄 .prettierrc
├── 📄 .editorconfig
├── 📄 docker-compose.yml
├── 📄 docker-compose.prod.yml
├── 📄 package.json
├── 📄 pnpm-workspace.yaml
├── 📄 turbo.json
├── 📄 Makefile
├── 📄 CHANGELOG.md
├── 📄 CONTRIBUTING.md
├── 📄 SECURITY.md
├── 📄 ARCHITECTURE.md
├── 📄 API-REFERENCE.md
├── 📄 DEPLOYMENT.md
├── 📄 SCALABILITY.md
│
├── 📦 packages/
│   │
│   ├── 📦 @masimpe/shared/
│   │   ├── 📄 package.json
│   │   ├── 📄 tsconfig.json
│   │   ├── 📄 tsconfig.build.json
│   │   ├── 📄 vitest.config.ts
│   │   ├── 📄 .eslintrc.js
│   │   └── 📂 src/
│   │       ├── 📄 index.ts
│   │       │
│   │       ├── 📂 types/
│   │       │   ├── 📄 index.ts
│   │       │   ├── 📄 hierarchy.ts          // National → Province → District → Zone → School
│   │       │   ├── 📄 user.ts               // Base user interface
│   │       │   ├── 📄 roles.ts              // Role definitions and hierarchy
│   │       │   ├── 📄 student.ts            // Student entity
│   │       │   ├── 📄 parent.ts             // Parent/Guardian entity
│   │       │   ├── 📄 teacher.ts            // Teacher entity
│   │       │   ├── 📄 teacher-performance.ts // Teacher performance metrics
│   │       │   ├── 📄 teacher-transfer.ts   // Teacher transfer records
│   │       │   ├── 📄 psc.ts               // Public Service Commission integration
│   │       │   ├── 📄 private-teacher.ts   // Private/independent teachers
│   │       │   ├── 📄 ancillary-staff.ts   // Non-teaching staff
│   │       │   ├── 📄 head.ts              // School Head/Principal
│   │       │   ├── 📄 school.ts            // School entity
│   │       │   ├── 📄 attendance.ts        // Attendance records
│   │       │   ├── 📄 academic.ts          // Academic records
│   │       │   ├── 📄 exam.ts              // Examination entity
│   │       │   ├── 📄 testing.ts           // Testing/Assessment entity
│   │       │   ├── 📄 testing-hierarchical.ts // Multi-level testing
│   │       │   ├── 📄 report.ts            // Report entity
│   │       │   ├── 📄 finance.ts           // Finance entity
│   │       │   ├── 📄 payroll.ts           // Payroll entity
│   │       │   ├── 📄 notification.ts      // Notification entity
│   │       │   ├── 📄 meeting.ts           // Meeting entity
│   │       │   ├── 📄 governance.ts        // Governance entity
│   │       │   ├── 📄 open-door.ts         // Open Door Policy entity
│   │       │   ├── 📄 student-leadership.ts // Prefects, Houses
│   │       │   ├── 📄 calendar.ts          // Calendar entity
│   │       │   ├── 📄 duty.ts              // Duty roster entity
│   │       │   ├── 📄 club.ts              // Club entity
│   │       │   ├── 📄 application.ts       // Application entity
│   │       │   ├── 📄 health.ts            // Health entity
│   │       │   ├── 📄 inventory.ts         // Inventory entity
│   │       │   ├── 📄 facility.ts          // Facility entity
│   │       │   ├── 📄 biometric.ts         // Biometric entity
│   │       │   ├── 📄 mapping.ts           // Mapping entity
│   │       │   ├── 📄 geolocation.ts       // Geolocation entity
│   │       │   ├── 📄 security-event.ts    // Security event entity
│   │       │   ├── 📄 design-system.ts     // Design system types
│   │       │   └── 📄 scalability.ts       // Scalability configuration
│   │       │
│   │       ├── 📂 validators/
│   │       │   ├── 📄 index.ts
│   │       │   ├── 📄 student-id.ts        // Student ID validation
│   │       │   ├── 📄 usi.ts               // USI (Unique Student Identifier)
│   │       │   ├── 📄 email.ts             // Email validation
│   │       │   ├── 📄 phone.ts             // Phone number validation
│   │       │   ├── 📄 password.ts          // Password policy
│   │       │   ├── 📄 payroll.ts           // Payroll validation
│   │       │   ├── 📄 biometric.ts         // Biometric data validation
│   │       │   └── 📄 geolocation.ts       // Geolocation validation
│   │       │
│   │       ├── 📂 constants/
│   │       │   ├── 📄 index.ts
│   │       │   ├── 📄 roles.ts             // Role constants
│   │       │   ├── 📄 permissions.ts       // Permission matrix
│   │       │   ├── 📄 provinces.ts         // Zimbabwe provinces
│   │       │   ├── 📄 districts.ts         // District list
│   │       │   ├── 📄 zones.ts             // Zone/Cluster list
│   │       │   ├── 📄 school-clusters.ts   // School clusters
│   │       │   ├── 📄 subjects.ts          // School subjects
│   │       │   ├── 📄 grades.ts            // Grade levels
│   │       │   ├── 📄 school-types.ts      // School types (Primary, Secondary)
│   │       │   ├── 📄 staff-categories.ts  // Staff categories
│   │       │   ├── 📄 allowance-types.ts   // Allowance types
│   │       │   ├── 📄 deduction-types.ts   // Deduction types
│   │       │   ├── 📄 tax-brackets.ts      // Tax brackets
│   │       │   ├── 📄 meeting-types.ts     // Meeting types
│   │       │   ├── 📄 committee-types.ts   // Committee types
│   │       │   ├── 📄 governance-types.ts  // Governance types
│   │       │   ├── 📄 prefect-portfolios.ts // Prefect portfolios
│   │       │   ├── 📄 notification-types.ts // Notification types
│   │       │   ├── 📄 biometric-types.ts   // Biometric types
│   │       │   └── 📄 retention-periods.ts // Data retention periods
│   │       │
│   │       ├── 📂 security/
│   │       │   ├── 📄 index.ts
│   │       │   ├── 📄 encryption.ts        // Encryption utilities
│   │       │   ├── 📄 field-encryption.ts  // Field-level encryption
│   │       │   ├── 📄 tokenization.ts      // Tokenization
│   │       │   ├── 📄 hierarchical-access.ts // Hierarchical access control
│   │       │   ├── 📄 rbac-service.ts      // RBAC service
│   │       │   ├── 📄 permission-checker.ts // Permission checker
│   │       │   ├── 📄 rate-limiter.ts      // Rate limiting
│   │       │   ├── 📄 data-classification.ts // Data classification
│   │       │   ├── 📄 csrf-protection.ts   // CSRF protection
│   │       │   ├── 📄 sql-injection-prevention.ts // SQL injection prevention
│   │       │   ├── 📄 xss-prevention.ts    // XSS prevention
│   │       │   └── 📄 zero-trust.ts        // Zero trust architecture
│   │       │
│   │       ├── 📂 auth/
│   │       │   ├── 📄 index.ts
│   │       │   ├── 📄 jwt-service.ts       // JWT service
│   │       │   ├── 📄 mfa-service.ts       // MFA service
│   │       │   ├── 📄 biometric-auth.ts    // Biometric authentication
│   │       │   ├── 📄 password-policy.ts   // Password policy
│   │       │   ├── 📄 session-manager.ts   // Session management
│   │       │   └── 📄 role-hierarchy.ts    // Role hierarchy
│   │       │
│   │       ├── 📂 crypto/
│   │       │   ├── 📄 index.ts
│   │       │   ├── 📄 hashing.ts           // Hashing utilities
│   │       │   ├── 📄 blockchain.ts        // Blockchain integration
│   │       │   ├── 📄 qrcode.ts            // QR code generation
│   │       │   └── 📄 digital-signature.ts // Digital signatures
│   │       │
│   │       ├── 📂 utils/
│   │       │   ├── 📄 index.ts
│   │       │   ├── 📄 date.ts              // Date utilities
│   │       │   ├── 📄 format.ts            // Formatting utilities
│   │       │   ├── 📄 id-generators.ts     // ID generators
│   │       │   └── 📄 slug-generator.ts    // Slug generator
│   │       │
│   │       └── 📂 config/
│   │           └── 📄 scalability.config.ts // Scalability configuration
│   │
│   │
│   ├── 📦 @masimpe/backend/
│   │   ├── 📄 package.json
│   │   ├── 📄 tsconfig.json
│   │   ├── 📄 tsconfig.build.json
│   │   ├── 📄 nest-cli.json
│   │   ├── 📄 Dockerfile
│   │   ├── 📄 .eslintrc.js
│   │   ├── 📄 vitest.config.ts
│   │   ├── 📄 prisma/
│   │   │   ├── 📄 schema.prisma
│   │   │   └── 📂 migrations/
│   │   │       └── 📄 20240101000000_init.sql
│   │   └── 📂 src/
│   │       ├── 📄 main.ts
│   │       ├── 📄 app.module.ts
│   │       │
│   │       ├── 📂 core/
│   │       │   ├── 📂 auth/
│   │       │   │   ├── 📄 auth.module.ts
│   │       │   │   ├── 📄 auth.service.ts
│   │       │   │   ├── 📄 auth.controller.ts
│   │       │   │   ├── 📄 jwt.strategy.ts
│   │       │   │   ├── 📄 local.strategy.ts
│   │       │   │   ├── 📄 api-key.strategy.ts
│   │       │   │   └── 📄 guards/
│   │       │   │       ├── 📄 jwt-auth.guard.ts
│   │       │   │       └── 📄 roles.guard.ts
│   │       │   │
│   │       │   ├── 📂 audit/
│   │       │   │   ├── 📄 audit.module.ts
│   │       │   │   ├── 📄 audit.service.ts
│   │       │   │   ├── 📄 audit.controller.ts
│   │       │   │   └── 📄 entities/
│   │       │   │       └── 📄 audit-log.entity.ts
│   │       │   │
│   │       │   ├── 📂 cache/
│   │       │   │   ├── 📄 cache.module.ts
│   │       │   │   └── 📄 cache.service.ts
│   │       │   │
│   │       │   ├── 📂 queue/
│   │       │   │   ├── 📄 queue.module.ts
│   │       │   │   ├── 📄 queue.service.ts
│   │       │   │   └── 📂 processors/
│   │       │   │       ├── 📄 email.processor.ts
│   │       │   │       ├── 📄 sms.processor.ts
│   │       │   │       ├── 📄 whatsapp.processor.ts
│   │       │   │       ├── 📄 notification.processor.ts
│   │       │   │       ├── 📄 pdf.processor.ts
│   │       │   │       ├── 📄 transcript.processor.ts
│   │       │   │       ├── 📄 certificate.processor.ts
│   │       │   │       ├── 📄 report-card.processor.ts
│   │       │   │       └── 📄 blockchain.processor.ts
│   │       │   │
│   │       │   ├── 📂 storage/
│   │       │   │   ├── 📄 storage.module.ts
│   │       │   │   └── 📄 storage.service.ts
│   │       │   │
│   │       │   └── 📂 template/
│   │       │       ├── 📄 template.module.ts
│   │       │       ├── 📄 template.service.ts
│   │       │       ├── 📄 template-renderer.service.ts
│   │       │       └── 📂 templates/
│   │       │           ├── 📂 email/
│   │       │           │   ├── 📄 welcome.hbs
│   │       │           │   ├── 📄 reset-password.hbs
│   │       │           │   └── 📄 notification.hbs
│   │       │           ├── 📂 sms/
│   │       │           │   ├── 📄 welcome.txt
│   │       │           │   └── 📄 notification.txt
│   │       │           └── 📂 pdf/
│   │       │               ├── 📄 payslip.hbs
│   │       │               └── 📄 transcript.hbs
│   │       │
│   │       ├── 📂 modules/
│   │       │   │
│   │       │   │   // ==========================================================
│   │       │   │   // 🏛️ NATIONAL LEVEL MODULES
│   │       │   │   // ==========================================================
│   │       │   │
│   │       │   ├── 📂 ministry-policy/
│   │       │   │   ├── 📄 ministry-policy.module.ts
│   │       │   │   ├── 📄 ministry-policy.service.ts
│   │       │   │   ├── 📄 ministry-policy.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-policy.dto.ts
│   │       │   │   │   └── 📄 update-policy.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 policy.entity.ts
│   │       │   │
│   │       │   ├── 📂 national-budget/
│   │       │   │   ├── 📄 national-budget.module.ts
│   │       │   │   ├── 📄 national-budget.service.ts
│   │       │   │   ├── 📄 national-budget.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-budget.dto.ts
│   │       │   │   │   └── 📄 allocate-budget.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 budget.entity.ts
│   │       │   │
│   │       │   ├── 📂 curriculum-development/
│   │       │   │   ├── 📄 curriculum-development.module.ts
│   │       │   │   ├── 📄 curriculum-development.service.ts
│   │       │   │   ├── 📄 curriculum-development.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-curriculum.dto.ts
│   │       │   │   │   └── 📄 update-curriculum.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 curriculum.entity.ts
│   │       │   │
│   │       │   ├── 📂 teacher-profession/
│   │       │   │   ├── 📄 teacher-profession.module.ts
│   │       │   │   ├── 📄 teacher-profession.service.ts
│   │       │   │   ├── 📄 teacher-profession.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 register-teacher.dto.ts
│   │       │   │   │   └── 📄 update-profession.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 profession.entity.ts
│   │       │   │
│   │       │   ├── 📂 national-examinations/
│   │       │   │   ├── 📄 national-examinations.module.ts
│   │       │   │   ├── 📄 national-examinations.service.ts
│   │       │   │   ├── 📄 national-examinations.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-exam.dto.ts
│   │       │   │   │   └── 📄 publish-exam.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 national-exam.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-standards/
│   │       │   │   ├── 📄 school-standards.module.ts
│   │       │   │   ├── 📄 school-standards.service.ts
│   │       │   │   ├── 📄 school-standards.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-standard.dto.ts
│   │       │   │   │   └── 📄 compliance-check.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 standard.entity.ts
│   │       │   │
│   │       │   ├── 📂 international-relations/
│   │       │   │   ├── 📄 international-relations.module.ts
│   │       │   │   ├── 📄 international-relations.service.ts
│   │       │   │   ├── 📄 international-relations.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-partnership.dto.ts
│   │       │   │   │   └── 📄 update-partnership.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 partnership.entity.ts
│   │       │   │
│   │       │   ├── 📂 research-statistics/
│   │       │   │   ├── 📄 research-statistics.module.ts
│   │       │   │   ├── 📄 research-statistics.service.ts
│   │       │   │   ├── 📄 research-statistics.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-research.dto.ts
│   │       │   │   │   └── 📄 statistics-query.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 research.entity.ts
│   │       │   │
│   │       │   ├── 📂 legal-compliance/
│   │       │   │   ├── 📄 legal-compliance.module.ts
│   │       │   │   ├── 📄 legal-compliance.service.ts
│   │       │   │   ├── 📄 legal-compliance.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-compliance.dto.ts
│   │       │   │   │   └── 📄 audit-request.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 compliance-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 parliament-relations/
│   │       │   │   ├── 📄 parliament-relations.module.ts
│   │       │   │   ├── 📄 parliament-relations.service.ts
│   │       │   │   ├── 📄 parliament-relations.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-report.dto.ts
│   │       │   │   │   └── 📄 submit-report.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 parliamentary-report.entity.ts
│   │       │   │
│   │       │   ├── 📂 cabinet-relations/
│   │       │   │   ├── 📄 cabinet-relations.module.ts
│   │       │   │   ├── 📄 cabinet-relations.service.ts
│   │       │   │   ├── 📄 cabinet-relations.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-memo.dto.ts
│   │       │   │   │   └── 📄 update-memo.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 cabinet-memo.entity.ts
│   │       │   │
│   │       │   ├── 📂 judicial/
│   │       │   │   ├── 📄 judicial.module.ts
│   │       │   │   ├── 📄 judicial.service.ts
│   │       │   │   ├── 📄 judicial.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-case.dto.ts
│   │       │   │   │   └── 📄 update-case.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 judicial-case.entity.ts
│   │       │   │
│   │       │   ├── 📂 accreditation/
│   │       │   │   ├── 📄 accreditation.module.ts
│   │       │   │   ├── 📄 accreditation.service.ts
│   │       │   │   ├── 📄 accreditation.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-accreditation.dto.ts
│   │       │   │   │   └── 📄 review-accreditation.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 accreditation.entity.ts
│   │       │   │
│   │       │   ├── 📂 education-financing/
│   │       │   │   ├── 📄 education-financing.module.ts
│   │       │   │   ├── 📄 education-financing.service.ts
│   │       │   │   ├── 📄 education-financing.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 allocate-funds.dto.ts
│   │       │   │   │   └── 📄 report-utilization.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 funding-allocation.entity.ts
│   │       │   │
│   │       │   ├── 📂 human-resources/
│   │       │   │   ├── 📄 human-resources.module.ts
│   │       │   │   ├── 📄 human-resources.service.ts
│   │       │   │   ├── 📄 human-resources.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-position.dto.ts
│   │       │   │   │   └── 📄 appoint-official.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 position.entity.ts
│   │       │   │
│   │       │   ├── 📂 edtech/
│   │       │   │   ├── 📄 edtech.module.ts
│   │       │   │   ├── 📄 edtech.service.ts
│   │       │   │   ├── 📄 edtech.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 deploy-device.dto.ts
│   │       │   │   │   └── 📄 update-device.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 edtech-device.entity.ts
│   │       │   │
│   │       │   ├── 📂 disaster-management/
│   │       │   │   ├── 📄 disaster-management.module.ts
│   │       │   │   ├── 📄 disaster-management.service.ts
│   │       │   │   ├── 📄 disaster-management.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-plan.dto.ts
│   │       │   │   │   └── 📄 respond-disaster.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 disaster-plan.entity.ts
│   │       │   │
│   │       │   ├── 📂 international-reporting/
│   │       │   │   ├── 📄 international-reporting.module.ts
│   │       │   │   ├── 📄 international-reporting.service.ts
│   │       │   │   ├── 📄 international-reporting.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-report.dto.ts
│   │       │   │   │   └── 📄 submit-un-report.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 international-report.entity.ts
│   │       │   │
│   │       │   ├── 📂 awards-recognition/
│   │       │   │   ├── 📄 awards-recognition.module.ts
│   │       │   │   ├── 📄 awards-recognition.service.ts
│   │       │   │   ├── 📄 awards-recognition.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-award.dto.ts
│   │       │   │   │   └── 📄 nominate.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 award.entity.ts
│   │       │   │
│   │       │   ├── 📂 future-planning/
│   │       │   │   ├── 📄 future-planning.module.ts
│   │       │   │   ├── 📄 future-planning.service.ts
│   │       │   │   ├── 📄 future-planning.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-strategy.dto.ts
│   │       │   │   │   └── 📄 update-vision.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 strategic-plan.entity.ts
│   │       │   │
│   │       │   │
│   │       │   │   // ==========================================================
│   │       │   │   // 📍 PROVINCIAL LEVEL MODULES
│   │       │   │   // ==========================================================
│   │       │   │
│   │       │   ├── 📂 provincial-strategic-planning/
│   │       │   │   ├── 📄 provincial-strategic-planning.module.ts
│   │       │   │   ├── 📄 provincial-strategic-planning.service.ts
│   │       │   │   ├── 📄 provincial-strategic-planning.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-plan.dto.ts
│   │       │   │   │   └── 📄 update-plan.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 provincial-plan.entity.ts
│   │       │   │
│   │       │   ├── 📂 provincial-budget/
│   │       │   │   ├── 📄 provincial-budget.module.ts
│   │       │   │   ├── 📄 provincial-budget.service.ts
│   │       │   │   ├── 📄 provincial-budget.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-budget.dto.ts
│   │       │   │   │   └── 📄 allocate-funds.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 provincial-budget.entity.ts
│   │       │   │
│   │       │   ├── 📂 infrastructure-projects/
│   │       │   │   ├── 📄 infrastructure-projects.module.ts
│   │       │   │   ├── 📄 infrastructure-projects.service.ts
│   │       │   │   ├── 📄 infrastructure-projects.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-project.dto.ts
│   │       │   │   │   └── 📄 update-project.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 infrastructure-project.entity.ts
│   │       │   │
│   │       │   ├── 📂 curriculum-implementation/
│   │       │   │   ├── 📄 curriculum-implementation.module.ts
│   │       │   │   ├── 📄 curriculum-implementation.service.ts
│   │       │   │   ├── 📄 curriculum-implementation.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 implement-curriculum.dto.ts
│   │       │   │   │   └── 📄 report-progress.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 curriculum-implementation.entity.ts
│   │       │   │
│   │       │   ├── 📂 provincial-examinations/
│   │       │   │   ├── 📄 provincial-examinations.module.ts
│   │       │   │   ├── 📄 provincial-examinations.service.ts
│   │       │   │   ├── 📄 provincial-examinations.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-exam.dto.ts
│   │       │   │   │   └── 📄 publish-results.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 provincial-exam.entity.ts
│   │       │   │
│   │       │   ├── 📂 provincial-teacher-management/
│   │       │   │   ├── 📄 provincial-teacher-management.module.ts
│   │       │   │   ├── 📄 provincial-teacher-management.service.ts
│   │       │   │   ├── 📄 provincial-teacher-management.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 deploy-teacher.dto.ts
│   │       │   │   │   └── 📄 transfer-teacher.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 provincial-teacher.entity.ts
│   │       │   │
│   │       │   ├── 📂 inter-district/
│   │       │   │   ├── 📄 inter-district.module.ts
│   │       │   │   ├── 📄 inter-district.service.ts
│   │       │   │   ├── 📄 inter-district.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-cooperation.dto.ts
│   │       │   │   │   └── 📄 resolve-dispute.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 inter-district-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 provincial-quality-assurance/
│   │       │   │   ├── 📄 provincial-quality-assurance.module.ts
│   │       │   │   ├── 📄 provincial-quality-assurance.service.ts
│   │       │   │   ├── 📄 provincial-quality-assurance.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 schedule-inspection.dto.ts
│   │       │   │   │   └── 📄 report-findings.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 quality-assurance-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 special-programs/
│   │       │   │   ├── 📄 special-programs.module.ts
│   │       │   │   ├── 📄 special-programs.service.ts
│   │       │   │   ├── 📄 special-programs.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-program.dto.ts
│   │       │   │   │   └── 📄 enroll-participant.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 special-program.entity.ts
│   │       │   │
│   │       │   ├── 📂 teacher-education/
│   │       │   │   ├── 📄 teacher-education.module.ts
│   │       │   │   ├── 📄 teacher-education.service.ts
│   │       │   │   ├── 📄 teacher-education.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-training.dto.ts
│   │       │   │   │   └── 📄 approve-training.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 teacher-training.entity.ts
│   │       │   │
│   │       │   ├── 📂 private-education/
│   │       │   │   ├── 📄 private-education.module.ts
│   │       │   │   ├── 📄 private-education.service.ts
│   │       │   │   ├── 📄 private-education.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 register-school.dto.ts
│   │       │   │   │   └── 📄 inspect-school.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 private-school.entity.ts
│   │       │   │
│   │       │   ├── 📂 gender-equity/
│   │       │   │   ├── 📄 gender-equity.module.ts
│   │       │   │   ├── 📄 gender-equity.service.ts
│   │       │   │   ├── 📄 gender-equity.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-program.dto.ts
│   │       │   │   │   └── 📄 report-metrics.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 gender-equity-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 partnerships/
│   │       │   │   ├── 📄 partnerships.module.ts
│   │       │   │   ├── 📄 partnerships.service.ts
│   │       │   │   ├── 📄 partnerships.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-partnership.dto.ts
│   │       │   │   │   └── 📄 update-partnership.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 partnership.entity.ts
│   │       │   │
│   │       │   ├── 📂 labor-relations/
│   │       │   │   ├── 📄 labor-relations.module.ts
│   │       │   │   ├── 📄 labor-relations.service.ts
│   │       │   │   ├── 📄 labor-relations.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-dispute.dto.ts
│   │       │   │   │   └── 📄 resolve-dispute.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 labor-dispute.entity.ts
│   │       │   │
│   │       │   ├── 📂 policy-implementation/
│   │       │   │   ├── 📄 policy-implementation.module.ts
│   │       │   │   ├── 📄 policy-implementation.service.ts
│   │       │   │   ├── 📄 policy-implementation.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 implement-policy.dto.ts
│   │       │   │   │   └── 📄 report-progress.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 policy-implementation.entity.ts
│   │       │   │
│   │       │   ├── 📂 provincial-emergency/
│   │       │   │   ├── 📄 provincial-emergency.module.ts
│   │       │   │   ├── 📄 provincial-emergency.service.ts
│   │       │   │   ├── 📄 provincial-emergency.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 declare-emergency.dto.ts
│   │       │   │   │   └── 📄 respond-emergency.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 emergency-record.entity.ts
│   │       │   │
│   │       │   │
│   │       │   │   // ==========================================================
│   │       │   │   // 📍 DISTRICT LEVEL MODULES
│   │       │   │   // ==========================================================
│   │       │   │
│   │       │   ├── 📂 school-registration/
│   │       │   │   ├── 📄 school-registration.module.ts
│   │       │   │   ├── 📄 school-registration.service.ts
│   │       │   │   ├── 📄 school-registration.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 register-school.dto.ts
│   │       │   │   │   ├── 📄 approve-school.dto.ts
│   │       │   │   │   └── 📄 inspect-school.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 school-registration.entity.ts
│   │       │   │
│   │       │   ├── 📂 teacher-deployment/
│   │       │   │   ├── 📄 teacher-deployment.module.ts
│   │       │   │   ├── 📄 teacher-deployment.service.ts
│   │       │   │   ├── 📄 teacher-deployment.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 deploy-teacher.dto.ts
│   │       │   │   │   └── 📄 allocate-teacher.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 deployment-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 teacher-performance/
│   │       │   │   ├── 📄 teacher-performance.module.ts
│   │       │   │   ├── 📄 teacher-performance.service.ts
│   │       │   │   ├── 📄 teacher-performance.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 evaluate-performance.dto.ts
│   │       │   │   │   └── 📄 report-performance.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 performance-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 teacher-retraining/
│   │       │   │   ├── 📄 teacher-retraining.module.ts
│   │       │   │   ├── 📄 teacher-retraining.service.ts
│   │       │   │   ├── 📄 teacher-retraining.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-training.dto.ts
│   │       │   │   │   └── 📄 enroll-teacher.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 retraining-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 teacher-transfers/
│   │       │   │   ├── 📄 teacher-transfers.module.ts
│   │       │   │   ├── 📄 teacher-transfers.service.ts
│   │       │   │   ├── 📄 teacher-transfers.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 request-transfer.dto.ts
│   │       │   │   │   └── 📄 approve-transfer.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 transfer-request.entity.ts
│   │       │   │
│   │       │   ├── 📂 psc-integration/
│   │       │   │   ├── 📄 psc-integration.module.ts
│   │       │   │   ├── 📄 psc-integration.service.ts
│   │       │   │   ├── 📄 psc-integration.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 sync-teacher.dto.ts
│   │       │   │   │   └── 📄 update-payslip.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 psc-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 private-teachers/
│   │       │   │   ├── 📄 private-teachers.module.ts
│   │       │   │   ├── 📄 private-teachers.service.ts
│   │       │   │   ├── 📄 private-teachers.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 register-private-teacher.dto.ts
│   │       │   │   │   └── 📄 update-private-teacher.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 private-teacher.entity.ts
│   │       │   │
│   │       │   ├── 📂 ancillary-staff/
│   │       │   │   ├── 📄 ancillary-staff.module.ts
│   │       │   │   ├── 📄 ancillary-staff.service.ts
│   │       │   │   ├── 📄 ancillary-staff.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-staff.dto.ts
│   │       │   │   │   └── 📄 update-staff.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 staff-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 head-appointment/
│   │       │   │   ├── 📄 head-appointment.module.ts
│   │       │   │   ├── 📄 head-appointment.service.ts
│   │       │   │   ├── 📄 head-appointment.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 appoint-head.dto.ts
│   │       │   │   │   └── 📄 evaluate-head.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 head-appointment.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-payroll/
│   │       │   │   ├── 📄 district-payroll.module.ts
│   │       │   │   ├── 📄 district-payroll.service.ts
│   │       │   │   ├── 📄 district-payroll.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 process-payroll.dto.ts
│   │       │   │   │   ├── 📄 generate-payslip.dto.ts
│   │       │   │   │   ├── 📄 calculate-tax.dto.ts
│   │       │   │   │   ├── 📄 calculate-nssa.dto.ts
│   │       │   │   │   ├── 📄 add-allowance.dto.ts
│   │       │   │   │   ├── 📄 add-deduction.dto.ts
│   │       │   │   │   ├── 📄 create-loan.dto.ts
│   │       │   │   │   └── 📄 request-advance.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 payroll-record.entity.ts
│   │       │   │       ├── 📄 payslip.entity.ts
│   │       │   │       ├── 📄 tax-record.entity.ts
│   │       │   │       ├── 📄 nssa-record.entity.ts
│   │       │   │       ├── 📄 allowance.entity.ts
│   │       │   │       ├── 📄 deduction.entity.ts
│   │       │   │       ├── 📄 loan.entity.ts
│   │       │   │       └── 📄 salary-advance.entity.ts
│   │       │   │
│   │       │   ├── 📂 resource-allocation/
│   │       │   │   ├── 📄 resource-allocation.module.ts
│   │       │   │   ├── 📄 resource-allocation.service.ts
│   │       │   │   ├── 📄 resource-allocation.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 allocate-resource.dto.ts
│   │       │   │   │   ├── 📄 distribute-textbooks.dto.ts
│   │       │   │   │   └── 📄 report-utilization.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 resource-allocation.entity.ts
│   │       │   │
│   │       │   ├── 📂 grants-management/
│   │       │   │   ├── 📄 grants-management.module.ts
│   │       │   │   ├── 📄 grants-management.service.ts
│   │       │   │   ├── 📄 grants-management.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 apply-grant.dto.ts
│   │       │   │   │   ├── 📄 approve-grant.dto.ts
│   │       │   │   │   └── 📄 disburse-grant.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 grant-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-finance/
│   │       │   │   ├── 📄 district-finance.module.ts
│   │       │   │   ├── 📄 district-finance.service.ts
│   │       │   │   ├── 📄 district-finance.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-invoice.dto.ts
│   │       │   │   │   ├── 📄 process-payment.dto.ts
│   │       │   │   │   ├── 📄 create-scholarship.dto.ts
│   │       │   │   │   ├── 📄 create-bursary.dto.ts
│   │       │   │   │   ├── 📄 create-aid.dto.ts
│   │       │   │   │   └── 📄 create-loan.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 invoice.entity.ts
│   │       │   │       ├── 📄 payment.entity.ts
│   │       │   │       ├── 📄 scholarship.entity.ts
│   │       │   │       ├── 📄 bursary.entity.ts
│   │       │   │       ├── 📄 financial-aid.entity.ts
│   │       │   │       └── 📄 student-loan.entity.ts
│   │       │   │
│   │       │   ├── 📂 cluster-coordination/
│   │       │   │   ├── 📄 cluster-coordination.module.ts
│   │       │   │   ├── 📄 cluster-coordination.service.ts
│   │       │   │   ├── 📄 cluster-coordination.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-cluster.dto.ts
│   │       │   │   │   ├── 📄 schedule-meeting.dto.ts
│   │       │   │   │   └── 📄 generate-report.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 cluster.entity.ts
│   │       │   │       ├── 📄 cluster-meeting.entity.ts
│   │       │   │       └── 📄 cluster-report.entity.ts
│   │       │   │
│   │       │   ├── 📂 conflict-resolution/
│   │       │   │   ├── 📄 conflict-resolution.module.ts
│   │       │   │   ├── 📄 conflict-resolution.service.ts
│   │       │   │   ├── 📄 conflict-resolution.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 report-conflict.dto.ts
│   │       │   │   │   ├── 📄 mediate-dispute.dto.ts
│   │       │   │   │   └── 📄 resolve-grievance.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 conflict-record.entity.ts
│   │       │   │       ├── 📄 dispute-record.entity.ts
│   │       │   │       └── 📄 grievance-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 crisis-management/
│   │       │   │   ├── 📄 crisis-management.module.ts
│   │       │   │   ├── 📄 crisis-management.service.ts
│   │       │   │   ├── 📄 crisis-management.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 declare-crisis.dto.ts
│   │       │   │   │   ├── 📄 respond-crisis.dto.ts
│   │       │   │   │   └── 📄 prepare-disaster.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 crisis-record.entity.ts
│   │       │   │       ├── 📄 emergency-response.entity.ts
│   │       │   │       └── 📄 disaster-plan.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-quality-assurance/
│   │       │   │   ├── 📄 district-quality-assurance.module.ts
│   │       │   │   ├── 📄 district-quality-assurance.service.ts
│   │       │   │   ├── 📄 district-quality-assurance.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 schedule-inspection.dto.ts
│   │       │   │   │   ├── 📄 report-inspection.dto.ts
│   │       │   │   │   └── 📄 set-standards.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 inspection-schedule.entity.ts
│   │       │   │       ├── 📄 inspection-report.entity.ts
│   │       │   │       └── 📄 quality-standard.entity.ts
│   │       │   │
│   │       │   ├── 📂 enrollment-management/
│   │       │   │   ├── 📄 enrollment-management.module.ts
│   │       │   │   ├── 📄 enrollment-management.service.ts
│   │       │   │   ├── 📄 enrollment-management.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 enroll-student.dto.ts
│   │       │   │   │   ├── 📄 register-student.dto.ts
│   │       │   │   │   ├── 📄 plan-capacity.dto.ts
│   │       │   │   │   ├── 📄 generate-usi.dto.ts
│   │       │   │   │   ├── 📄 validate-usi.dto.ts
│   │       │   │   │   └── 📄 link-parent.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 enrollment-record.entity.ts
│   │       │   │       ├── 📄 student-registration.entity.ts
│   │       │   │       ├── 📄 capacity-plan.entity.ts
│   │       │   │       ├── 📄 usi-record.entity.ts
│   │       │   │       └── 📄 parent-link.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-transport/
│   │       │   │   ├── 📄 district-transport.module.ts
│   │       │   │   ├── 📄 district-transport.service.ts
│   │       │   │   ├── 📄 district-transport.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-route.dto.ts
│   │       │   │   │   ├── 📄 schedule-bus.dto.ts
│   │       │   │   │   └── 📄 report-safety.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 bus-route.entity.ts
│   │       │   │       ├── 📄 bus-schedule.entity.ts
│   │       │   │       └── 📄 transport-safety.entity.ts
│   │       │   │
│   │       │   ├── 📂 special-education/
│   │       │   │   ├── 📄 special-education.module.ts
│   │       │   │   ├── 📄 special-education.service.ts
│   │       │   │   ├── 📄 special-education.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-program.dto.ts
│   │       │   │   │   ├── 📄 enroll-student.dto.ts
│   │       │   │   │   └── 📄 allocate-device.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 special-education-program.entity.ts
│   │       │   │       ├── 📄 inclusive-education-record.entity.ts
│   │       │   │       └── 📄 assistive-device.entity.ts
│   │       │   │
│   │       │   ├── 📂 sports-culture/
│   │       │   │   ├── 📄 sports-culture.module.ts
│   │       │   │   ├── 📄 sports-culture.service.ts
│   │       │   │   ├── 📄 sports-culture.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-event.dto.ts
│   │       │   │   │   ├── 📄 organize-competition.dto.ts
│   │       │   │   │   └── 📄 register-team.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 sports-event.entity.ts
│   │       │   │       ├── 📄 competition.entity.ts
│   │       │   │       └── 📄 cultural-event.entity.ts
│   │       │   │
│   │       │   ├── 📂 child-protection/
│   │       │   │   ├── 📄 child-protection.module.ts
│   │       │   │   ├── 📄 child-protection.service.ts
│   │       │   │   ├── 📄 child-protection.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 report-concern.dto.ts
│   │       │   │   │   ├── 📄 safeguard-child.dto.ts
│   │       │   │   │   └── 📄 refer-case.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 child-protection-record.entity.ts
│   │       │   │       ├── 📄 safeguarding-plan.entity.ts
│   │       │   │       └── 📄 welfare-referral.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-health/
│   │       │   │   ├── 📄 district-health.module.ts
│   │       │   │   ├── 📄 district-health.service.ts
│   │       │   │   ├── 📄 district-health.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 schedule-screening.dto.ts
│   │       │   │   │   ├── 📄 record-immunization.dto.ts
│   │       │   │   │   ├── 📄 record-vision.dto.ts
│   │       │   │   │   ├── 📄 record-hearing.dto.ts
│   │       │   │   │   ├── 📄 record-mental-health.dto.ts
│   │       │   │   │   ├── 📄 record-nutrition.dto.ts
│   │       │   │   │   ├── 📄 record-menstrual.dto.ts
│   │       │   │   │   ├── 📄 record-chronic.dto.ts
│   │       │   │   │   ├── 📄 record-dental.dto.ts
│   │       │   │   │   ├── 📄 record-sleep.dto.ts
│   │       │   │   │   ├── 📄 record-counselling.dto.ts
│   │       │   │   │   └── 📄 record-crisis.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 health-screening.entity.ts
│   │       │   │       ├── 📄 immunization-record.entity.ts
│   │       │   │       ├── 📄 vision-record.entity.ts
│   │       │   │       ├── 📄 hearing-record.entity.ts
│   │       │   │       ├── 📄 mental-health-record.entity.ts
│   │       │   │       ├── 📄 nutrition-record.entity.ts
│   │       │   │       ├── 📄 menstrual-health-record.entity.ts
│   │       │   │       ├── 📄 chronic-condition-record.entity.ts
│   │       │   │       ├── 📄 dental-record.entity.ts
│   │       │   │       ├── 📄 sleep-record.entity.ts
│   │       │   │       ├── 📄 counselling-record.entity.ts
│   │       │   │       └── 📄 crisis-intervention-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 ict-coordination/
│   │       │   │   ├── 📄 ict-coordination.module.ts
│   │       │   │   ├── 📄 ict-coordination.service.ts
│   │       │   │   ├── 📄 ict-coordination.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 deploy-device.dto.ts
│   │       │   │   │   ├── 📄 install-edtech.dto.ts
│   │       │   │   │   └── 📄 manage-device.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 ict-device.entity.ts
│   │       │   │       ├── 📄 edtech-deployment.entity.ts
│   │       │   │       └── 📄 device-management-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 environmental/
│   │       │   │   ├── 📄 environmental.module.ts
│   │       │   │   ├── 📄 environmental.service.ts
│   │       │   │   ├── 📄 environmental.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-garden.dto.ts
│   │       │   │   │   └── 📄 manage-waste.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 school-garden.entity.ts
│   │       │   │       └── 📄 waste-management-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 stakeholder-engagement/
│   │       │   │   ├── 📄 stakeholder-engagement.module.ts
│   │       │   │   ├── 📄 stakeholder-engagement.service.ts
│   │       │   │   ├── 📄 stakeholder-engagement.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 register-stakeholder.dto.ts
│   │       │   │   │   ├── 📄 outreach-program.dto.ts
│   │       │   │   │   └── 📄 engage-parent.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 stakeholder.entity.ts
│   │       │   │       ├── 📄 outreach-record.entity.ts
│   │       │   │       └── 📄 parent-engagement-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 community-mobilization/
│   │       │   │   ├── 📄 community-mobilization.module.ts
│   │       │   │   ├── 📄 community-mobilization.service.ts
│   │       │   │   ├── 📄 community-mobilization.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-project.dto.ts
│   │       │   │   │   ├── 📄 register-volunteer.dto.ts
│   │       │   │   │   └── 📄 organize-event.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 community-project.entity.ts
│   │       │   │       ├── 📄 volunteer-record.entity.ts
│   │       │   │       └── 📄 community-event.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-data-management/
│   │       │   │   ├── 📄 district-data-management.module.ts
│   │       │   │   ├── 📄 district-data-management.service.ts
│   │       │   │   ├── 📄 district-data-management.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 collect-data.dto.ts
│   │       │   │   │   ├── 📄 sync-emis.dto.ts
│   │       │   │   │   └── 📄 validate-data.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 data-collection-record.entity.ts
│   │       │   │       ├── 📄 emis-sync-record.entity.ts
│   │       │   │       └── 📄 data-validation-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-governance/
│   │       │   │   ├── 📄 district-governance.module.ts
│   │       │   │   ├── 📄 district-governance.service.ts
│   │       │   │   ├── 📄 district-governance.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-committee.dto.ts
│   │       │   │   │   ├── 📄 appoint-member.dto.ts
│   │       │   │   │   ├── 📄 conduct-election.dto.ts
│   │       │   │   │   └── 📄 vet-candidate.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 committee.entity.ts
│   │       │   │       ├── 📄 committee-member.entity.ts
│   │       │   │       ├── 📄 election-record.entity.ts
│   │       │   │       └── 📄 vetting-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-meetings/
│   │       │   │   ├── 📄 district-meetings.module.ts
│   │       │   │   ├── 📄 district-meetings.service.ts
│   │       │   │   ├── 📄 district-meetings.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 schedule-meeting.dto.ts
│   │       │   │   │   ├── 📄 create-agenda.dto.ts
│   │       │   │   │   ├── 📄 record-minutes.dto.ts
│   │       │   │   │   ├── 📄 track-resolution.dto.ts
│   │       │   │   │   └── 📄 track-action.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 meeting.entity.ts
│   │       │   │       ├── 📄 meeting-agenda.entity.ts
│   │       │   │       ├── 📄 meeting-minutes.entity.ts
│   │       │   │       ├── 📄 resolution.entity.ts
│   │       │   │       └── 📄 action-item.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-open-door/
│   │       │   │   ├── 📄 district-open-door.module.ts
│   │       │   │   ├── 📄 district-open-door.service.ts
│   │       │   │   ├── 📄 district-open-door.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 record-walkin.dto.ts
│   │       │   │   │   ├── 📄 schedule-appointment.dto.ts
│   │       │   │   │   ├── 📄 register-complaint.dto.ts
│   │       │   │   │   └── 📄 resolve-grievance.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 walk-in-record.entity.ts
│   │       │   │       ├── 📄 appointment.entity.ts
│   │       │   │       ├── 📄 complaint-record.entity.ts
│   │       │   │       └── 📄 grievance-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 student-leadership/
│   │       │   │   ├── 📄 student-leadership.module.ts
│   │       │   │   ├── 📄 student-leadership.service.ts
│   │       │   │   ├── 📄 student-leadership.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 appoint-prefect.dto.ts
│   │       │   │   │   ├── 📄 create-house.dto.ts
│   │       │   │   │   └── 📄 conduct-election.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 prefect-record.entity.ts
│   │       │   │       ├── 📄 house.entity.ts
│   │       │   │       └── 📄 student-election.entity.ts
│   │       │   │
│   │       │   ├── 📂 clubs/
│   │       │   │   ├── 📄 clubs.module.ts
│   │       │   │   ├── 📄 clubs.service.ts
│   │       │   │   ├── 📄 clubs.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-club.dto.ts
│   │       │   │   │   ├── 📄 register-member.dto.ts
│   │       │   │   │   └── 📄 schedule-activity.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 club.entity.ts
│   │       │   │       ├── 📄 club-member.entity.ts
│   │       │   │       └── 📄 club-activity.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-calendar/
│   │       │   │   ├── 📄 district-calendar.module.ts
│   │       │   │   ├── 📄 district-calendar.service.ts
│   │       │   │   ├── 📄 district-calendar.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-event.dto.ts
│   │       │   │   │   └── 📄 update-event.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 calendar-event.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-duty/
│   │       │   │   ├── 📄 district-duty.module.ts
│   │       │   │   ├── 📄 district-duty.service.ts
│   │       │   │   ├── 📄 district-duty.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-roster.dto.ts
│   │       │   │   │   └── 📄 assign-duty.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 duty-roster.entity.ts
│   │       │   │       └── 📄 duty-assignment.entity.ts
│   │       │   │
│   │       │   ├── 📂 applications/
│   │       │   │   ├── 📄 applications.module.ts
│   │       │   │   ├── 📄 applications.service.ts
│   │       │   │   ├── 📄 applications.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-application.dto.ts
│   │       │   │   │   ├── 📄 process-placement.dto.ts
│   │       │   │   │   ├── 📄 process-appeal.dto.ts
│   │       │   │   │   ├── 📄 process-transfer.dto.ts
│   │       │   │   │   └── 📄 verify-application.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 application-record.entity.ts
│   │       │   │       ├── 📄 placement-record.entity.ts
│   │       │   │       ├── 📄 appeal-record.entity.ts
│   │       │   │       ├── 📄 transfer-application.entity.ts
│   │       │   │       └── 📄 verification-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 facilities/
│   │       │   │   ├── 📄 facilities.module.ts
│   │       │   │   ├── 📄 facilities.service.ts
│   │       │   │   ├── 📄 facilities.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 book-room.dto.ts
│   │       │   │   │   ├── 📄 allocate-parking.dto.ts
│   │       │   │   │   ├── 📄 track-bus.dto.ts
│   │       │   │   │   ├── 📄 manage-catering.dto.ts
│   │       │   │   │   └── 📄 organize-event.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 room-booking.entity.ts
│   │       │   │       ├── 📄 parking-allocation.entity.ts
│   │       │   │       ├── 📄 bus-tracking-record.entity.ts
│   │       │   │       ├── 📄 catering-record.entity.ts
│   │       │   │       └── 📄 event-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-inventory/
│   │       │   │   ├── 📄 district-inventory.module.ts
│   │       │   │   ├── 📄 district-inventory.service.ts
│   │       │   │   ├── 📄 district-inventory.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 add-item.dto.ts
│   │       │   │   │   ├── 📄 update-item.dto.ts
│   │       │   │   │   └── 📄 report-usage.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 inventory-item.entity.ts
│   │       │   │       └── 📄 usage-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 mapping/
│   │       │   │   ├── 📄 mapping.module.ts
│   │       │   │   ├── 📄 mapping.service.ts
│   │       │   │   ├── 📄 mapping.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-school-map.dto.ts
│   │       │   │   │   ├── 📄 create-district-map.dto.ts
│   │       │   │   │   ├── 📄 create-indoor-map.dto.ts
│   │       │   │   │   ├── 📄 create-tile.dto.ts
│   │       │   │   │   └── 📄 export-map.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 school-map.entity.ts
│   │       │   │       ├── 📄 district-map.entity.ts
│   │       │   │       ├── 📄 indoor-map.entity.ts
│   │       │   │       ├── 📄 map-tile.entity.ts
│   │       │   │       └── 📄 map-export.entity.ts
│   │       │   │
│   │       │   ├── 📂 biometric/
│   │       │   │   ├── 📄 biometric.module.ts
│   │       │   │   ├── 📄 biometric.service.ts
│   │       │   │   ├── 📄 biometric.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 enroll-fingerprint.dto.ts
│   │       │   │   │   ├── 📄 match-fingerprint.dto.ts
│   │       │   │   │   ├── 📄 recognize-face.dto.ts
│   │       │   │   │   ├── 📄 register-device.dto.ts
│   │       │   │   │   ├── 📄 sync-device.dto.ts
│   │       │   │   │   ├── 📄 store-template.dto.ts
│   │       │   │   │   ├── 📄 match-template.dto.ts
│   │       │   │   │   └── 📄 cache-offline.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 fingerprint-template.entity.ts
│   │       │   │       ├── 📄 facial-template.entity.ts
│   │       │   │       ├── 📄 biometric-device.entity.ts
│   │       │   │       ├── 📄 device-sync-record.entity.ts
│   │       │   │       ├── 📄 biometric-match.entity.ts
│   │       │   │       └── 📄 offline-cache.entity.ts
│   │       │   │
│   │       │   ├── 📂 attendance/
│   │       │   │   ├── 📄 attendance.module.ts
│   │       │   │   ├── 📄 attendance.service.ts
│   │       │   │   ├── 📄 attendance.controller.ts
│   │       │   │   ├── 📄 attendance.gateway.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 record-attendance.dto.ts
│   │       │   │   │   ├── 📄 bulk-attendance.dto.ts
│   │       │   │   │   ├── 📄 biometric-attendance.dto.ts
│   │       │   │   │   └── 📄 offline-attendance.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 attendance-record.entity.ts
│   │       │   │       ├── 📄 attendance-batch.entity.ts
│   │       │   │       └── 📄 attendance-sync.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-academics/
│   │       │   │   ├── 📄 district-academics.module.ts
│   │       │   │   ├── 📄 district-academics.service.ts
│   │       │   │   ├── 📄 district-academics.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-subject.dto.ts
│   │       │   │   │   ├── 📄 create-class.dto.ts
│   │       │   │   │   └── 📄 create-timetable.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 subject.entity.ts
│   │       │   │       ├── 📄 class.entity.ts
│   │       │   │       └── 📄 timetable.entity.ts
│   │       │   │
│   │       │   ├── 📂 testing/
│   │       │   │   ├── 📄 testing.module.ts
│   │       │   │   ├── 📄 testing.service.ts
│   │       │   │   ├── 📄 testing.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-test.dto.ts
│   │       │   │   │   ├── 📄 build-question.dto.ts
│   │       │   │   │   ├── 📄 auto-grade.dto.ts
│   │       │   │   │   └── 📄 check-plagiarism.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 test-record.entity.ts
│   │       │   │       ├── 📄 question.entity.ts
│   │       │   │       ├── 📄 grading-record.entity.ts
│   │       │   │       └── 📄 plagiarism-check.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-exams/
│   │       │   │   ├── 📄 district-exams.module.ts
│   │       │   │   ├── 📄 district-exams.service.ts
│   │       │   │   ├── 📄 district-exams.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-exam.dto.ts
│   │       │   │   │   ├── 📄 online-exam.dto.ts
│   │       │   │   │   ├── 📄 proctoring-config.dto.ts
│   │       │   │   │   └── 📄 lockdown-config.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 exam-record.entity.ts
│   │       │   │       ├── 📄 online-exam-record.entity.ts
│   │       │   │       ├── 📄 proctoring-record.entity.ts
│   │       │   │       └── 📄 lockdown-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 reports/
│   │       │   │   ├── 📄 reports.module.ts
│   │       │   │   ├── 📄 reports.service.ts
│   │       │   │   ├── 📄 reports.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 generate-report.dto.ts
│   │       │   │   │   ├── 📄 generate-transcript.dto.ts
│   │       │   │   │   ├── 📄 verify-transcript.dto.ts
│   │       │   │   │   └── 📄 generate-portfolio.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 report-record.entity.ts
│   │       │   │       ├── 📄 transcript.entity.ts
│   │       │   │       ├── 📄 transcript-verification.entity.ts
│   │       │   │       └── 📄 portfolio.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-communication/
│   │       │   │   ├── 📄 district-communication.module.ts
│   │       │   │   ├── 📄 district-communication.service.ts
│   │       │   │   ├── 📄 district-communication.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 send-sms.dto.ts
│   │       │   │   │   ├── 📄 send-email.dto.ts
│   │       │   │   │   ├── 📄 send-whatsapp.dto.ts
│   │       │   │   │   ├── 📄 send-voice.dto.ts
│   │       │   │   │   └── 📄 send-ussd.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 sms-record.entity.ts
│   │       │   │       ├── 📄 email-record.entity.ts
│   │       │   │       ├── 📄 whatsapp-record.entity.ts
│   │       │   │       ├── 📄 voice-record.entity.ts
│   │       │   │       └── 📄 ussd-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 notifications/
│   │       │   │   ├── 📄 notifications.module.ts
│   │       │   │   ├── 📄 notifications.service.ts
│   │       │   │   ├── 📄 notifications.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-notification.dto.ts
│   │       │   │   │   └── 📄 send-notification.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 notification-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-compliance/
│   │       │   │   ├── 📄 district-compliance.module.ts
│   │       │   │   ├── 📄 district-compliance.service.ts
│   │       │   │   ├── 📄 district-compliance.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 check-compliance.dto.ts
│   │       │   │   │   ├── 📄 regulatory-check.dto.ts
│   │       │   │   │   └── 📄 audit-trail.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 compliance-record.entity.ts
│   │       │   │       ├── 📄 regulatory-record.entity.ts
│   │       │   │       └── 📄 audit-trail-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 offline-sync/
│   │       │   │   ├── 📄 offline-sync.module.ts
│   │       │   │   ├── 📄 offline-sync.service.ts
│   │       │   │   ├── 📄 offline-sync.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 cache-offline.dto.ts
│   │       │   │   │   └── 📄 sync-offline.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 offline-cache.entity.ts
│   │       │   │       └── 📄 offline-sync-record.entity.ts
│   │       │   │
│   │       │   │
│   │       │   │   // ==========================================================
│   │       │   │   // 🏫 SCHOOL LEVEL MODULES
│   │       │   │   // ==========================================================
│   │       │   │
│   │       │   ├── 📂 school-profile/
│   │       │   │   ├── 📄 school-profile.module.ts
│   │       │   │   ├── 📄 school-profile.service.ts
│   │       │   │   ├── 📄 school-profile.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-school.dto.ts
│   │       │   │   │   ├── 📄 update-school.dto.ts
│   │       │   │   │   └── 📄 get-school.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 school.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-branding/
│   │       │   │   ├── 📄 school-branding.module.ts
│   │       │   │   ├── 📄 school-branding.service.ts
│   │       │   │   ├── 📄 school-branding.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 update-theme.dto.ts
│   │       │   │   │   ├── 📄 upload-logo.dto.ts
│   │       │   │   │   └── 📄 customize-branding.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 school-branding.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-accounts/
│   │       │   │   ├── 📄 school-accounts.module.ts
│   │       │   │   ├── 📄 school-accounts.service.ts
│   │       │   │   ├── 📄 school-accounts.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-account.dto.ts
│   │       │   │   │   └── 📄 update-account.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 school-account.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-timetable/
│   │       │   │   ├── 📄 school-timetable.module.ts
│   │       │   │   ├── 📄 school-timetable.service.ts
│   │       │   │   ├── 📄 school-timetable.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-timetable.dto.ts
│   │       │   │   │   └── 📄 update-timetable.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 timetable.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-classes/
│   │       │   │   ├── 📄 school-classes.module.ts
│   │       │   │   ├── 📄 school-classes.service.ts
│   │       │   │   ├── 📄 school-classes.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-class.dto.ts
│   │       │   │   │   └── 📄 update-class.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 class.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-subjects/
│   │       │   │   ├── 📄 school-subjects.module.ts
│   │       │   │   ├── 📄 school-subjects.service.ts
│   │       │   │   ├── 📄 school-subjects.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-subject.dto.ts
│   │       │   │   │   └── 📄 update-subject.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 subject.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-gradebook/
│   │       │   │   ├── 📄 school-gradebook.module.ts
│   │       │   │   ├── 📄 school-gradebook.service.ts
│   │       │   │   ├── 📄 school-gradebook.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-grade.dto.ts
│   │       │   │   │   └── 📄 update-grade.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 grade-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-transcripts/
│   │       │   │   ├── 📄 school-transcripts.module.ts
│   │       │   │   ├── 📄 school-transcripts.service.ts
│   │       │   │   ├── 📄 school-transcripts.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 generate-transcript.dto.ts
│   │       │   │   │   └── 📄 verify-transcript.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 transcript.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-verification/
│   │       │   │   ├── 📄 school-verification.module.ts
│   │       │   │   ├── 📄 school-verification.service.ts
│   │       │   │   ├── 📄 school-verification.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 verify-document.dto.ts
│   │       │   │   │   └── 📄 verify-student.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 verification-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-library/
│   │       │   │   ├── 📄 school-library.module.ts
│   │       │   │   ├── 📄 school-library.service.ts
│   │       │   │   ├── 📄 school-library.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 add-book.dto.ts
│   │       │   │   │   ├── 📄 borrow-book.dto.ts
│   │       │   │   │   └── 📄 return-book.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 library-book.entity.ts
│   │       │   │       ├── 📄 digital-book.entity.ts
│   │       │   │       ├── 📄 loan-record.entity.ts
│   │       │   │       └── 📄 oer-resource.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-duties/
│   │       │   │   ├── 📄 school-duties.module.ts
│   │       │   │   ├── 📄 school-duties.service.ts
│   │       │   │   ├── 📄 school-duties.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-roster.dto.ts
│   │       │   │   │   └── 📄 assign-duty.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 duty-roster.entity.ts
│   │       │   │       └── 📄 duty-assignment.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-clubs/
│   │       │   │   ├── 📄 school-clubs.module.ts
│   │       │   │   ├── 📄 school-clubs.service.ts
│   │       │   │   ├── 📄 school-clubs.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-club.dto.ts
│   │       │   │   │   └── 📄 register-member.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 club.entity.ts
│   │       │   │       └── 📄 club-member.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-health/
│   │       │   │   ├── 📄 school-health.module.ts
│   │       │   │   ├── 📄 school-health.service.ts
│   │       │   │   ├── 📄 school-health.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 record-health.dto.ts
│   │       │   │   │   ├── 📄 schedule-screening.dto.ts
│   │       │   │   │   └── 📄 refer-student.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 health-record.entity.ts
│   │       │   │       ├── 📄 screening-record.entity.ts
│   │       │   │       └── 📄 health-referral.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-facilities/
│   │       │   │   ├── 📄 school-facilities.module.ts
│   │       │   │   ├── 📄 school-facilities.service.ts
│   │       │   │   ├── 📄 school-facilities.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-facility.dto.ts
│   │       │   │   │   ├── 📄 book-room.dto.ts
│   │       │   │   │   └── 📄 maintain-facility.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 facility.entity.ts
│   │       │   │       ├── 📄 room-booking.entity.ts
│   │       │   │       └── 📄 maintenance-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-inventory/
│   │       │   │   ├── 📄 school-inventory.module.ts
│   │       │   │   ├── 📄 school-inventory.service.ts
│   │       │   │   ├── 📄 school-inventory.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 add-item.dto.ts
│   │       │   │   │   ├── 📄 update-item.dto.ts
│   │       │   │   │   └── 📄 report-usage.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 inventory-item.entity.ts
│   │       │   │       └── 📄 usage-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-finance/
│   │       │   │   ├── 📄 school-finance.module.ts
│   │       │   │   ├── 📄 school-finance.service.ts
│   │       │   │   ├── 📄 school-finance.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-invoice.dto.ts
│   │       │   │   │   ├── 📄 process-payment.dto.ts
│   │       │   │   │   ├── 📄 create-scholarship.dto.ts
│   │       │   │   │   └── 📄 create-bursary.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 invoice.entity.ts
│   │       │   │       ├── 📄 payment.entity.ts
│   │       │   │       ├── 📄 scholarship.entity.ts
│   │       │   │       └── 📄 bursary.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-fees/
│   │       │   │   ├── 📄 school-fees.module.ts
│   │       │   │   ├── 📄 school-fees.service.ts
│   │       │   │   ├── 📄 school-fees.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 set-fees.dto.ts
│   │       │   │   │   ├── 📄 collect-fees.dto.ts
│   │       │   │   │   └── 📄 report-fees.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 fee-structure.entity.ts
│   │       │   │       └── 📄 fee-collection.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-payments/
│   │       │   │   ├── 📄 school-payments.module.ts
│   │       │   │   ├── 📄 school-payments.service.ts
│   │       │   │   ├── 📄 school-payments.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 initiate-payment.dto.ts
│   │       │   │   │   ├── 📄 process-webhook.dto.ts
│   │       │   │   │   └── 📄 reconcile-payment.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 payment-record.entity.ts
│   │       │   │       ├── 📄 webhook-record.entity.ts
│   │       │   │       └── 📄 reconciliation-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-scholarships/
│   │       │   │   ├── 📄 school-scholarships.module.ts
│   │       │   │   ├── 📄 school-scholarships.service.ts
│   │       │   │   ├── 📄 school-scholarships.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-scholarship.dto.ts
│   │       │   │   │   └── 📄 award-scholarship.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 scholarship-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-bursaries/
│   │       │   │   ├── 📄 school-bursaries.module.ts│   │       │   │   ├── 📄 school-bursaries.service.ts
│   │       │   │   ├── 📄 school-bursaries.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-bursary.dto.ts
│   │       │   │   │   └── 📄 award-bursary.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 bursary-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-communication/
│   │       │   │   ├── 📄 school-communication.module.ts
│   │       │   │   ├── 📄 school-communication.service.ts
│   │       │   │   ├── 📄 school-communication.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 send-notification.dto.ts
│   │       │   │   │   ├── 📄 send-broadcast.dto.ts
│   │       │   │   │   └── 📄 send-reminder.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 notification.entity.ts
│   │       │   │       ├── 📄 broadcast-record.entity.ts
│   │       │   │       └── 📄 reminder-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-notifications/
│   │       │   │   ├── 📄 school-notifications.module.ts
│   │       │   │   ├── 📄 school-notifications.service.ts
│   │       │   │   ├── 📄 school-notifications.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-notification.dto.ts
│   │       │   │   │   └── 📄 send-notification.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 notification-record.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-events/
│   │       │   │   ├── 📄 school-events.module.ts
│   │       │   │   ├── 📄 school-events.service.ts
│   │       │   │   ├── 📄 school-events.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-event.dto.ts
│   │       │   │   │   └── 📄 update-event.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 event-record.entity.ts
│   │       │   │
│   │       │   └── 📂 school-reporting/
│   │       │       ├── 📄 school-reporting.module.ts
│   │       │       ├── 📄 school-reporting.service.ts
│   │       │       ├── 📄 school-reporting.controller.ts
│   │       │       ├── 📂 dto/
│   │       │       │   ├── 📄 generate-report.dto.ts
│   │       │       │   ├── 📄 export-report.dto.ts
│   │       │       │   └── 📄 schedule-report.dto.ts
│   │       │       └── 📂 entities/
│   │       │           ├── 📄 report-record.entity.ts
│   │       │           ├── 📄 export-record.entity.ts
│   │       │           └── 📄 scheduled-report.entity.ts
│   │       │
│   │       └── 📂 prisma/
│   │           ├── 📄 prisma.module.ts
│   │           └── 📄 prisma.service.ts
│   │
│   │
│   ├── 📦 @masimpe/testing-hierarchical/
│   │   ├── 📄 package.json
│   │   ├── 📄 tsconfig.json
│   │   ├── 📄 tsconfig.build.json
│   │   ├── 📄 Dockerfile
│   │   ├── 📄 .eslintrc.js
│   │   ├── 📄 vitest.config.ts
│   │   └── 📂 src/
│   │       ├── 📄 index.ts
│   │       │
│   │       ├── 📂 modules/
│   │       │   │
│   │       │   ├── 📂 national-testing/
│   │       │   │   ├── 📄 national-testing.module.ts
│   │       │   │   ├── 📄 national-testing.service.ts
│   │       │   │   ├── 📄 national-testing.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-national-test.dto.ts
│   │       │   │   │   ├── 📄 schedule-national-test.dto.ts
│   │       │   │   │   └── 📄 publish-national-results.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 national-test.entity.ts
│   │       │   │       └── 📄 national-result.entity.ts
│   │       │   │
│   │       │   ├── 📂 provincial-testing/
│   │       │   │   ├── 📄 provincial-testing.module.ts
│   │       │   │   ├── 📄 provincial-testing.service.ts
│   │       │   │   ├── 📄 provincial-testing.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-provincial-test.dto.ts
│   │       │   │   │   ├── 📄 schedule-provincial-test.dto.ts
│   │       │   │   │   └── 📄 publish-provincial-results.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 provincial-test.entity.ts
│   │       │   │       └── 📄 provincial-result.entity.ts
│   │       │   │
│   │       │   ├── 📂 district-testing/
│   │       │   │   ├── 📄 district-testing.module.ts
│   │       │   │   ├── 📄 district-testing.service.ts
│   │       │   │   ├── 📄 district-testing.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-district-test.dto.ts
│   │       │   │   │   ├── 📄 schedule-district-test.dto.ts
│   │       │   │   │   ├── 📄 benchmark-district.dto.ts
│   │       │   │   │   └── 📄 publish-district-results.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 district-test.entity.ts
│   │       │   │       ├── 📄 district-benchmark.entity.ts
│   │       │   │       └── 📄 district-result.entity.ts
│   │       │   │
│   │       │   ├── 📂 zonal-testing/
│   │       │   │   ├── 📄 zonal-testing.module.ts
│   │       │   │   ├── 📄 zonal-testing.service.ts
│   │       │   │   ├── 📄 zonal-testing.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-zonal-test.dto.ts
│   │       │   │   │   ├── 📄 schedule-zonal-test.dto.ts
│   │       │   │   │   └── 📄 publish-zonal-results.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 zonal-test.entity.ts
│   │       │   │       └── 📄 zonal-result.entity.ts
│   │       │   │
│   │       │   ├── 📂 school-testing/
│   │       │   │   ├── 📄 school-testing.module.ts
│   │       │   │   ├── 📄 school-testing.service.ts
│   │       │   │   ├── 📄 school-testing.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 create-school-test.dto.ts
│   │       │   │   │   ├── 📄 submit-school-test.dto.ts
│   │       │   │   │   └── 📄 analyze-school-test.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 school-test.entity.ts
│   │       │   │       └── 📄 school-test-result.entity.ts
│   │       │   │
│   │       │   └── 📂 aggregation/
│   │       │       ├── 📄 aggregation.module.ts
│   │       │       ├── 📄 aggregation.service.ts
│   │       │       ├── 📄 aggregation.controller.ts
│   │       │       ├── 📂 dto/
│   │       │       │   ├── 📄 aggregate-results.dto.ts
│   │       │       │   ├── 📄 generate-rankings.dto.ts
│   │       │       │   ├── 📄 calculate-performance-index.dto.ts
│   │       │       │   └── 📄 generate-league-tables.dto.ts
│   │       │       └── 📂 entities/
│   │       │           ├── 📄 aggregated-result.entity.ts
│   │       │           ├── 📄 ranking-record.entity.ts
│   │       │           ├── 📄 performance-index.entity.ts
│   │       │           └── 📄 league-table.entity.ts
│   │       │
│   │       └── 📂 question-types/
│   │           ├── 📄 multiple-choice.ts     // Multiple choice question
│   │           ├── 📄 true-false.ts          // True/False question
│   │           ├── 📄 short-answer.ts        // Short answer question
│   │           ├── 📄 essay.ts               // Essay question
│   │           ├── 📄 fill-blanks.ts         // Fill in the blanks
│   │           ├── 📄 matching.ts            // Matching question
│   │           ├── 📄 ordering.ts            // Ordering/Sequence question
│   │           ├── 📄 hotspot.ts             // Hotspot/Image click question
│   │           ├── 📄 numerical.ts           // Numerical question
│   │           ├── 📄 equation.ts            // Math equation question
│   │           ├── 📄 audio.ts               // Audio-based question
│   │           └── 📄 coding.ts              // Programming question
│   │
│   │
│   ├── 📦 @masimpe/analytics/
│   │   ├── 📄 package.json
│   │   ├── 📄 tsconfig.json
│   │   ├── 📄 tsconfig.build.json
│   │   ├── 📄 Dockerfile
│   │   ├── 📄 .eslintrc.js
│   │   ├── 📄 vitest.config.ts
│   │   └── 📂 src/
│   │       ├── 📄 index.ts
│   │       │
│   │       ├── 📂 dashboards/
│   │       │   ├── 📂 ministry-dashboard/
│   │       │   │   ├── 📄 ministry-dashboard.module.ts
│   │       │   │   ├── 📄 ministry-dashboard.service.ts
│   │       │   │   ├── 📄 ministry-dashboard.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 get-national-stats.dto.ts
│   │       │   │   │   └── 📄 get-policy-metrics.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 national-stat.entity.ts
│   │       │   │
│   │       │   ├── 📂 ped-dashboard/
│   │       │   │   ├── 📄 ped-dashboard.module.ts
│   │       │   │   ├── 📄 ped-dashboard.service.ts
│   │       │   │   ├── 📄 ped-dashboard.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 get-provincial-stats.dto.ts
│   │       │   │   │   └── 📄 get-infrastructure-metrics.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 provincial-stat.entity.ts
│   │       │   │
│   │       │   ├── 📂 dsi-dashboard/
│   │       │   │   ├── 📄 dsi-dashboard.module.ts
│   │       │   │   ├── 📄 dsi-dashboard.service.ts
│   │       │   │   ├── 📄 dsi-dashboard.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 get-district-stats.dto.ts
│   │       │   │   │   ├── 📄 get-school-performance.dto.ts
│   │       │   │   │   ├── 📄 get-teacher-deployment.dto.ts
│   │       │   │   │   ├── 📄 get-enrollment-trends.dto.ts
│   │       │   │   │   └── 📄 get-resource-utilization.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       ├── 📄 district-stat.entity.ts
│   │       │   │       ├── 📄 school-performance.entity.ts
│   │       │   │       ├── 📄 teacher-deployment-stat.entity.ts
│   │       │   │       ├── 📄 enrollment-trend.entity.ts
│   │       │   │       └── 📄 resource-utilization.entity.ts
│   │       │   │
│   │       │   ├── 📂 head-dashboard/
│   │       │   │   ├── 📄 head-dashboard.module.ts
│   │       │   │   ├── 📄 head-dashboard.service.ts
│   │       │   │   ├── 📄 head-dashboard.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 get-school-stats.dto.ts
│   │       │   │   │   ├── 📄 get-class-performance.dto.ts
│   │       │   │   │   └── 📄 get-fee-collection.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 school-stat.entity.ts
│   │       │   │
│   │       │   ├── 📂 teacher-dashboard/
│   │       │   │   ├── 📄 teacher-dashboard.module.ts
│   │       │   │   ├── 📄 teacher-dashboard.service.ts
│   │       │   │   ├── 📄 teacher-dashboard.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 get-class-stats.dto.ts
│   │       │   │   │   └── 📄 get-student-performance.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 class-stat.entity.ts
│   │       │   │
│   │       │   ├── 📂 student-dashboard/
│   │       │   │   ├── 📄 student-dashboard.module.ts
│   │       │   │   ├── 📄 student-dashboard.service.ts
│   │       │   │   ├── 📄 student-dashboard.controller.ts
│   │       │   │   ├── 📂 dto/
│   │       │   │   │   ├── 📄 get-student-progress.dto.ts
│   │       │   │   │   └── 📄 get-student-grades.dto.ts
│   │       │   │   └── 📂 entities/
│   │       │   │       └── 📄 student-progress.entity.ts
│   │       │   │
│   │       │   └── 📂 parent-dashboard/
│   │       │       ├── 📄 parent-dashboard.module.ts
│   │       │       ├── 📄 parent-dashboard.service.ts
│   │       │       ├── 📄 parent-dashboard.controller.ts
│   │       │       ├── 📂 dto/
│   │       │       │   ├── 📄 get-child-progress.dto.ts
│   │       │       │   └── 📄 get-child-attendance.dto.ts
│   │       │       └── 📂 entities/
│   │       │           └── 📄 child-progress.entity.ts
│   │       │
│   │       └── 📂 predictive/
│   │           ├── 📂 dropout-prediction/
│   │           │   ├── 📄 dropout-prediction.module.ts
│   │           │   ├── 📄 dropout-prediction.service.ts
│   │           │   ├── 📄 dropout-prediction.controller.ts
│   │           │   ├── 📂 dto/
│   │           │   │   ├── 📄 predict-dropout.dto.ts
│   │           │   │   └── 📄 get-risk-students.dto.ts
│   │           │   └── 📂 entities/
│   │           │       └── 📄 dropout-prediction.entity.ts
│   │           │
│   │           └── 📂 performance-prediction/
│   │               ├── 📄 performance-prediction.module.ts
│   │               ├── 📄 performance-prediction.service.ts
│   │               ├── 📄 performance-prediction.controller.ts
│   │               ├── 📂 dto/
│   │               │   ├── 📄 predict-performance.dto.ts
│   │               │   └── 📄 get-predicted-grades.dto.ts
│   │               └── 📂 entities/
│   │                   └── 📄 performance-prediction.entity.ts
│   │
│   │
│   ├── 📦 @masimpe/frontend/
│   │   ├── 📄 package.json
│   │   ├── 📄 tsconfig.json
│   │   ├── 📄 tsconfig.build.json
│   │   ├── 📄 next.config.js
│   │   ├── 📄 next-env.d.ts
│   │   ├── 📄 Dockerfile
│   │   ├── 📄 .eslintrc.js
│   │   ├── 📄 vitest.config.ts
│   │   ├── 📄 tailwind.config.js
│   │   ├── 📄 postcss.config.js
│   │   ├── 📂 public/
│   │   │   ├── 📄 index.html
│   │   │   ├── 📄 manifest.json
│   │   │   ├── 📄 sw.js               // Service worker for offline
│   │   │   ├── 📂 icons/
│   │   │   │   ├── 📄 favicon.ico
│   │   │   │   ├── 📄 icon-192.png
│   │   │   │   └── 📄 icon-512.png
│   │   │   ├── 📂 images/
│   │   │   │   ├── 📄 logo.svg
│   │   │   │   └── 📄 hero.jpg
│   │   │   └── 📂 fonts/
│   │   │       └── 📄 inter.ttf
│   │   │
│   │   └── 📂 src/
│   │       ├── 📄 index.ts
│   │       ├── 📄 app.ts
│   │       │
│   │       ├── 📂 app/
│   │       │   ├── 📄 layout.tsx
│   │       │   ├── 📄 page.tsx
│   │       │   ├── 📄 globals.css
│   │       │   │
│   │       │   ├── 📂 (auth)/
│   │       │   │   ├── 📂 login/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 login-form.tsx
│   │       │   │   └── 📂 register/
│   │       │   │       ├── 📄 page.tsx
│   │       │   │       └── 📄 register-form.tsx
│   │       │   │
│   │       │   ├── 📂 (ministry)/
│   │       │   │   ├── 📂 dashboard/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 stats.tsx
│   │       │   │   ├── 📂 policy/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 policy-form.tsx
│   │       │   │   ├── 📂 budget/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 budget-form.tsx
│   │       │   │   ├── 📂 curriculum/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 curriculum-form.tsx
│   │       │   │   ├── 📂 examinations/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 exam-form.tsx
│   │       │   │   ├── 📂 standards/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 standards-form.tsx
│   │       │   │   ├── 📂 research/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 research-form.tsx
│   │       │   │   ├── 📂 legal/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 legal-form.tsx
│   │       │   │   ├── 📂 accreditation/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 accreditation-form.tsx
│   │       │   │   └── 📂 international/
│   │       │   │       ├── 📄 page.tsx
│   │       │   │       └── 📄 international-form.tsx
│   │       │   │
│   │       │   ├── 📂 (ped)/
│   │       │   │   ├── 📂 dashboard/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 stats.tsx
│   │       │   │   ├── 📂 strategic-planning/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 plan-form.tsx
│   │       │   │   ├── 📂 infrastructure/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 project-form.tsx
│   │       │   │   ├── 📂 teacher-management/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 teacher-form.tsx
│   │       │   │   ├── 📂 inter-district/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 coordination-form.tsx
│   │       │   │   ├── 📂 quality-assurance/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 inspection-form.tsx
│   │       │   │   ├── 📂 special-programs/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 program-form.tsx
│   │       │   │   ├── 📂 gender-equity/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 equity-form.tsx
│   │       │   │   └── 📂 partnerships/
│   │       │   │       ├── 📄 page.tsx
│   │       │   │       └── 📄 partnership-form.tsx
│   │       │   │
│   │       │   ├── 📂 (dsi)/
│   │       │   │   ├── 📂 dashboard/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 stats.tsx
│   │       │   │   ├── 📂 schools/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   ├── 📄 school-list.tsx
│   │       │   │   │   └── 📄 school-form.tsx
│   │       │   │   ├── 📂 teachers/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   ├── 📄 teacher-list.tsx
│   │       │   │   │   └── 📄 teacher-form.tsx
│   │       │   │   ├── 📂 payroll/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   ├── 📄 payroll-list.tsx
│   │       │   │   │   └── 📄 payroll-form.tsx
│   │       │   │   ├── 📂 resources/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   ├── 📄 resource-list.tsx
│   │       │   │   │   └── 📄 resource-form.tsx
│   │       │   │   ├── 📂 grants/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   ├── 📄 grant-list.tsx
│   │       │   │   │   └── 📄 grant-form.tsx
│   │       │   │   ├── 📂 clusters/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   ├── 📄 cluster-list.tsx
│   │       │   │   │   └── 📄 cluster-form.tsx
│   │       │   │   ├── 📂 quality/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 inspection-form.tsx
│   │       │   │   ├── 📂 enrollment/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 enrollment-form.tsx
│   │       │   │   ├── 📂 health/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 health-form.tsx
│   │       │   │   ├── 📂 governance/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 governance-form.tsx
│   │       │   │   ├── 📂 meetings/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 meeting-form.tsx
│   │       │   │   ├── 📂 open-door/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 open-door-form.tsx
│   │       │   │   ├── 📂 leadership/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 leadership-form.tsx
│   │       │   │   ├── 📂 clubs/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 club-form.tsx
│   │       │   │   ├── 📂 calendar/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 calendar-form.tsx
│   │       │   │   ├── 📂 duties/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 duty-form.tsx
│   │       │   │   ├── 📂 applications/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 application-form.tsx
│   │       │   │   ├── 📂 facilities/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 facility-form.tsx
│   │       │   │   ├── 📂 biometric/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 biometric-form.tsx
│   │       │   │   ├── 📂 mapping/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 map-view.tsx
│   │       │   │   ├── 📂 attendance/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 attendance-form.tsx
│   │       │   │   ├── 📂 academics/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 academics-form.tsx
│   │       │   │   ├── 📂 testing/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 testing-form.tsx
│   │       │   │   ├── 📂 exams/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 exam-form.tsx
│   │       │   │   ├── 📂 reports/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 report-form.tsx
│   │       │   │   ├── 📂 communication/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 communication-form.tsx
│   │       │   │   └── 📂 compliance/
│   │       │   │       ├── 📄 page.tsx
│   │       │   │       └── 📄 compliance-form.tsx
│   │       │   │
│   │       │   ├── 📂 (head)/
│   │       │   │   ├── 📂 dashboard/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 stats.tsx
│   │       │   │   ├── 📂 students/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 student-form.tsx
│   │       │   │   ├── 📂 teachers/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 teacher-form.tsx
│   │       │   │   ├── 📂 classes/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 class-form.tsx
│   │       │   │   ├── 📂 timetable/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 timetable-form.tsx
│   │       │   │   ├── 📂 attendance/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 attendance-form.tsx
│   │       │   │   ├── 📂 gradebook/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 gradebook-form.tsx
│   │       │   │   ├── 📂 fees/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 fees-form.tsx
│   │       │   │   ├── 📂 library/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 library-form.tsx
│   │       │   │   ├── 📂 health/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 health-form.tsx
│   │       │   │   ├── 📂 facilities/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 facility-form.tsx
│   │       │   │   ├── 📂 inventory/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 inventory-form.tsx
│   │       │   │   ├── 📂 clubs/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 club-form.tsx
│   │       │   │   ├── 📂 events/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 event-form.tsx
│   │       │   │   └── 📂 reports/
│   │       │   │       ├── 📄 page.tsx
│   │       │   │       └── 📄 report-form.tsx
│   │       │   │
│   │       │   ├── 📂 (teacher)/
│   │       │   │   ├── 📂 dashboard/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 stats.tsx
│   │       │   │   ├── 📂 classes/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 class-view.tsx
│   │       │   │   ├── 📂 attendance/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 attendance-form.tsx
│   │       │   │   ├── 📂 gradebook/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 grade-form.tsx
│   │       │   │   ├── 📂 testing/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 test-form.tsx
│   │       │   │   ├── 📂 exams/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 exam-form.tsx
│   │       │   │   ├── 📂 duty/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 duty-form.tsx
│   │       │   │   └── 📂 reports/
│   │       │   │       ├── 📄 page.tsx
│   │       │   │       └── 📄 report-form.tsx
│   │       │   │
│   │       │   ├── 📂 (student)/
│   │       │   │   ├── 📂 dashboard/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 stats.tsx
│   │       │   │   ├── 📂 classes/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 class-view.tsx
│   │       │   │   ├── 📂 attendance/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 attendance-view.tsx
│   │       │   │   ├── 📂 grades/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 grades-view.tsx
│   │       │   │   ├── 📂 exams/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 exam-view.tsx
│   │       │   │   ├── 📂 library/
│   │       │   │   │   ├── 📄 page.tsx
│   │       │   │   │   └── 📄 library-view.tsx
│   │       │   │   └── 📂 clubs/
│   │       │   │       ├── 📄 page.tsx
│   │       │   │       └── 📄 club-view.tsx
│   │       │   │
│   │       │   └── 📂 (parent)/
│   │       │       ├── 📂 dashboard/
│   │       │       │   ├── 📄 page.tsx
│   │       │       │   └── 📄 stats.tsx
│   │       │       ├── 📂 child-progress/
│   │       │       │   ├── 📄 page.tsx
│   │       │       │   └── 📄 progress-view.tsx
│   │       │       ├── 📂 attendance/
│   │       │       │   ├── 📄 page.tsx
│   │       │       │   └── 📄 attendance-view.tsx
│   │       │       ├── 📂 fees/
│   │       │       │   ├── 📄 page.tsx
│   │       │       │   └── 📄 fees-view.tsx
│   │       │       └── 📂 communication/
│   │       │           ├── 📄 page.tsx
│   │       │           └── 📄 communication-view.tsx
│   │       │
│   │       ├── 📂 components/
│   │       │   ├── 📂 ui/
│   │       │   │   ├── 📄 button.tsx
│   │       │   │   ├── 📄 input.tsx
│   │       │   │   ├── 📄 select.tsx
│   │       │   │   ├── 📄 table.tsx
│   │       │   │   ├── 📄 modal.tsx
│   │       │   │   ├── 📄 toast.tsx
│   │       │   │   ├── 📄 dropdown.tsx
│   │       │   │   ├── 📄 card.tsx
│   │       │   │   ├── 📄 loading.tsx
│   │       │   │   ├── 📄 error.tsx
│   │       │   │   ├── 📄 success.tsx
│   │       │   │   └── 📄 empty-state.tsx
│   │       │   │
│   │       │   ├── 📂 auth/
│   │       │   │   ├── 📄 login-form.tsx
│   │       │   │   ├── 📄 register-form.tsx
│   │       │   │   ├── 📄 reset-password.tsx
│   │       │   │   ├── 📄 mfa-form.tsx
│   │       │   │   ├── 📄 biometric-auth.tsx
│   │       │   │   └── 📄 role-selector.tsx
│   │       │   │
│   │       │   ├── 📂 ministry/
│   │       │   │   ├── 📄 policy-list.tsx
│   │       │   │   ├── 📄 budget-list.tsx
│   │       │   │   ├── 📄 curriculum-list.tsx
│   │       │   │   ├── 📄 exam-list.tsx
│   │       │   │   ├── 📄 standard-list.tsx
│   │       │   │   ├── 📄 research-list.tsx
│   │       │   │   ├── 📄 legal-list.tsx
│   │       │   │   ├── 📄 accreditation-list.tsx
│   │       │   │   └── 📄 international-list.tsx
│   │       │   │
│   │       │   ├── 📂 provincial/
│   │       │   │   ├── 📄 strategic-plan-list.tsx
│   │       │   │   ├── 📄 project-list.tsx
│   │       │   │   ├── 📄 teacher-list.tsx
│   │       │   │   ├── 📄 coordination-list.tsx
│   │       │   │   ├── 📄 inspection-list.tsx
│   │       │   │   ├── 📄 program-list.tsx
│   │       │   │   ├── 📄 equity-list.tsx
│   │       │   │   └── 📄 partnership-list.tsx
│   │       │   │
│   │       │   ├── 📂 district/
│   │       │   │   ├── 📄 school-list.tsx
│   │       │   │   ├── 📄 teacher-list.tsx
│   │       │   │   ├── 📄 payroll-list.tsx
│   │       │   │   ├── 📄 resource-list.tsx
│   │       │   │   ├── 📄 grant-list.tsx
│   │       │   │   ├── 📄 cluster-list.tsx
│   │       │   │   ├── 📄 inspection-list.tsx
│   │       │   │   ├── 📄 enrollment-list.tsx
│   │       │   │   ├── 📄 health-list.tsx
│   │       │   │   ├── 📄 governance-list.tsx
│   │       │   │   ├── 📄 meeting-list.tsx
│   │       │   │   ├── 📄 open-door-list.tsx
│   │       │   │   ├── 📄 leadership-list.tsx
│   │       │   │   ├── 📄 club-list.tsx
│   │       │   │   ├── 📄 calendar-list.tsx
│   │       │   │   ├── 📄 duty-list.tsx
│   │       │   │   ├── 📄 application-list.tsx
│   │       │   │   ├── 📄 facility-list.tsx
│   │       │   │   ├── 📄 biometric-list.tsx
│   │       │   │   ├── 📄 map-view.tsx
│   │       │   │   ├── 📄 attendance-list.tsx
│   │       │   │   ├── 📄 academic-list.tsx
│   │       │   │   ├── 📄 test-list.tsx
│   │       │   │   ├── 📄 exam-list.tsx
│   │       │   │   ├── 📄 report-list.tsx
│   │       │   │   ├── 📄 communication-list.tsx
│   │       │   │   └── 📄 compliance-list.tsx
│   │       │   │
│   │       │   ├── 📂 school/
│   │       │   │   ├── 📄 school-profile.tsx
│   │       │   │   ├── 📄 school-branding.tsx
│   │       │   │   ├── 📄 school-accounts.tsx
│   │       │   │   ├── 📄 timetable-view.tsx
│   │       │   │   ├── 📄 class-list.tsx
│   │       │   │   ├── 📄 subject-list.tsx
│   │       │   │   ├── 📄 gradebook-view.tsx
│   │       │   │   ├── 📄 transcript-view.tsx
│   │       │   │   ├── 📄 verification-view.tsx
│   │       │   │   ├── 📄 library-view.tsx
│   │       │   │   ├── 📄 duty-roster.tsx
│   │       │   │   ├── 📄 club-list.tsx
│   │       │   │   ├── 📄 health-record.tsx
│   │       │   │   ├── 📄 facility-list.tsx
│   │       │   │   ├── 📄 inventory-list.tsx
│   │       │   │   ├── 📄 finance-view.tsx
│   │       │   │   ├── 📄 fees-view.tsx
│   │       │   │   ├── 📄 payment-view.tsx
│   │       │   │   ├── 📄 scholarship-view.tsx
│   │       │   │   ├── 📄 bursary-view.tsx
│   │       │   │   ├── 📄 communication-view.tsx
│   │       │   │   ├── 📄 notification-view.tsx
│   │       │   │   └── 📄 event-list.tsx
│   │       │   │
│   │       │   ├── 📂 teacher/
│   │       │   │   ├── 📄 class-view.tsx
│   │       │   │   ├── 📄 attendance-view.tsx
│   │       │   │   ├── 📄 gradebook-view.tsx
│   │       │   │   ├── 📄 test-view.tsx
│   │       │   │   ├── 📄 exam-view.tsx
│   │       │   │   ├── 📄 duty-view.tsx
│   │       │   │   └── 📄 report-view.tsx
│   │       │   │
│   │       │   ├── 📂 student/
│   │       │   │   ├── 📄 class-view.tsx
│   │       │   │   ├── 📄 attendance-view.tsx
│   │       │   │   ├── 📄 grades-view.tsx
│   │       │   │   ├── 📄 exam-view.tsx
│   │       │   │   ├── 📄 library-view.tsx
│   │       │   │   └── 📄 club-view.tsx
│   │       │   │
│   │       │   └── 📂 parent/
│   │       │       ├── 📄 progress-view.tsx
│   │       │       ├── 📄 attendance-view.tsx
│   │       │       ├── 📄 fees-view.tsx
│   │       │       └── 📄 communication-view.tsx
│   │       │
│   │       ├── 📂 design-system/
│   │       │   ├── 📂 tokens/
│   │       │   │   ├── 📂 skeomorphism/
│   │       │   │   │   ├── 📄 index.css
│   │       │   │   │   └── 📄 config.ts
│   │       │   │   ├── 📂 neomorphism/
│   │       │   │   │   ├── 📄 index.css
│   │       │   │   │   └── 📄 config.ts
│   │       │   │   ├── 📂 glassmorphism/
│   │       │   │   │   ├── 📄 index.css
│   │       │   │   │   └── 📄 config.ts
│   │       │   │   ├── 📂 claymorphism/
│   │       │   │   │   ├── 📄 index.css
│   │       │   │   │   └── 📄 config.ts
│   │       │   │   ├── 📂 minimalism/
│   │       │   │   │   ├── 📄 index.css
│   │       │   │   │   └── 📄 config.ts
│   │       │   │   ├── 📂 maximalism/
│   │       │   │   │   ├── 📄 index.css
│   │       │   │   │   └── 📄 config.ts
│   │       │   │   ├── 📂 brutalism/
│   │       │   │   │   ├── 📄 index.css
│   │       │   │   │   └── 📄 config.ts
│   │       │   │   ├── 📂 liquid-glass/
│   │       │   │   │   ├── 📄 index.css
│   │       │   │   │   └── 📄 config.ts
│   │       │   │   ├── 📂 bento-grid/
│   │       │   │   │   ├── 📄 index.css
│   │       │   │   │   └── 📄 config.ts
│   │       │   │   └── 📂 spatial-ui/
│   │       │   │       ├── 📄 index.css
│   │       │   │       └── 📄 config.ts
│   │       │   │
│   │       │   └── 📂 customizer/
│   │       │       ├── 📄 theme-selector.tsx
│   │       │       ├── 📄 color-customizer.tsx
│   │       │       ├── 📄 typography-customizer.tsx
│   │       │       ├── 📄 logo-injector.tsx
│   │       │       └── 📄 theme-preview.tsx
│   │       │
│   │       ├── 📂 lib/
│   │       │   ├── 📂 api/
│   │       │   │   ├── 📄 client.ts
│   │       │   │   ├── 📄 auth.ts
│   │       │   │   ├── 📄 schools.ts
│   │       │   │   ├── 📄 teachers.ts
│   │       │   │   ├── 📄 students.ts
│   │       │   │   └── 📄 index.ts
│   │       │   │
│   │       │   ├── 📂 store/
│   │       │   │   ├── 📄 auth-store.ts
│   │       │   │   ├── 📄 school-store.ts
│   │       │   │   ├── 📄 teacher-store.ts
│   │       │   │   ├── 📄 student-store.ts
│   │       │   │   └── 📄 index.ts
│   │       │   │
│   │       │   ├── 📂 hooks/
│   │       │   │   ├── 📄 use-auth.ts
│   │       │   │   ├── 📄 use-schools.ts
│   │       │   │   ├── 📄 use-teachers.ts
│   │       │   │   ├── 📄 use-students.ts
│   │       │   │   ├── 📄 use-attendance.ts
│   │       │   │   ├── 📄 use-offline.ts
│   │       │   │   └── 📄 index.ts
│   │       │   │
│   │       │   ├── 📂 utils/
│   │       │   │   ├── 📄 formatters.ts
│   │       │   │   ├── 📄 validators.ts
│   │       │   │   ├── 📄 date-helpers.ts
│   │       │   │   └── 📄 index.ts
│   │       │   │
│   │       │   └── 📂 offline/
│   │       │       ├── 📄 service-worker.ts
│   │       │       ├── 📄 sync-manager.ts
│   │       │       ├── 📄 cache-manager.ts
│   │       │       └── 📄 index.ts
│   │       │
│   │       └── 📂 styles/
│   │           ├── 📄 globals.css
│   │           ├── 📄 themes.css
│   │           └── 📄 variables.css
│   │
│   │
│   ├── 📦 @masimpe/mobile/
│   │   ├── 📄 package.json
│   │   ├── 📄 tsconfig.json
│   │   ├── 📄 tsconfig.build.json
│   │   ├── 📄 Dockerfile
│   │   ├── 📄 .eslintrc.js
│   │   ├── 📄 vitest.config.ts
│   │   └── 📂 src/
│   │       ├── 📄 index.ts
│   │       │
│   │       ├── 📂 ussd/
│   │       │   ├── 📄 app.ts
│   │       │   ├── 📄 session.ts
│   │       │   │
│   │       │   ├── 📂 menus/
│   │       │   │   ├── 📄 ministry-menus.ts        // Ministry level USSD
│   │       │   │   ├── 📄 provincial-menus.ts      // PED level USSD
│   │       │   │   ├── 📄 district-menus.ts        // DSI level USSD
│   │       │   │   ├── 📄 school-menus.ts          // School level USSD
│   │       │   │   ├── 📄 teacher-menus.ts         // Teacher level USSD
│   │       │   │   ├── 📄 student-menus.ts         // Student level USSD
│   │       │   │   └── 📄 parent-menus.ts          // Parent level USSD
│   │       │   │
│   │       │   ├── 📂 handlers/
│   │       │   │   ├── 📄 attendance.handler.ts
│   │       │   │   ├── 📄 results.handler.ts
│   │       │   │   ├── 📄 fees.handler.ts
│   │       │   │   ├── 📄 reports.handler.ts
│   │       │   │   ├── 📄 pin.handler.ts
│   │       │   │   └── 📄 info.handler.ts
│   │       │   │
│   │       │   └── 📂 dto/
│   │       │       ├── 📄 ussd-request.dto.ts
│   │       │       ├── 📄 ussd-response.dto.ts
│   │       │       └── 📄 ussd-session.dto.ts
│   │       │
│   │       └── 📂 sms/
│   │           ├── 📄 dispatcher.ts
│   │           ├── 📄 receivers.ts
│   │           │
│   │           ├── 📂 templates/
│   │           │   ├── 📄 attendance.txt
│   │           │   ├── 📄 results.txt
│   │           │   ├── 📄 fees.txt
│   │           │   ├── 📄 notification.txt
│   │           │   ├── 📄 reminder.txt
│   │           │   ├── 📄 alert.txt
│   │           │   └── 📄 report.txt
│   │           │
│   │           └── 📂 dto/
│   │               ├── 📄 sms-request.dto.ts
│   │               ├── 📄 sms-response.dto.ts
│   │               └── 📄 sms-template.dto.ts
│   │
│   │
│   └── 📦 @masimpe/docs/
│       ├── 📄 package.json
│       ├── 📄 docusaurus.config.js
│       ├── 📄 sidebars.js
│       ├── 📄 Dockerfile
│       ├── 📄 .eslintrc.js
│       ├── 📂 docs/
│       │   ├── 📄 index.md
│       │   │
│       │   ├── 📂 architecture/
│       │   │   ├── 📄 overview.md
│       │   │   ├── 📄 data-model.md
│       │   │   ├── 📄 security.md
│       │   │   ├── 📄 scalability.md
│       │   │   └── 📄 deployment.md
│       │   │
│       │   ├── 📂 api/
│       │   │   ├── 📄 overview.md
│       │   │   ├── 📄 auth.md
│       │   │   ├── 📄 schools.md
│       │   │   ├── 📄 teachers.md
│       │   │   ├── 📄 students.md
│       │   │   ├── 📄 attendance.md
│       │   │   ├── 📄 academics.md
│       │   │   ├── 📄 exams.md
│       │   │   ├── 📄 finance.md
│       │   │   ├── 📄 reports.md
│       │   │   └── 📄 webhooks.md
│       │   │
│       │   ├── 📂 user-guides/
│       │   │   ├── 📄 ministry-admin.md
│       │   │   ├── 📄 ped-admin.md
│       │   │   ├── 📄 dsi-admin.md
│       │   │   ├── 📄 head-teacher.md
│       │   │   ├── 📄 teacher.md
│       │   │   ├── 📄 student.md
│       │   │   └── 📄 parent.md
│       │   │
│       │   ├── 📂 operations/
│       │   │   ├── 📄 onboarding.md
│       │   │   ├── 📄 maintenance.md
│       │   │   ├── 📄 monitoring.md
│       │   │   ├── 📄 backup.md
│       │   │   ├── 📄 disaster-recovery.md
│       │   │   └── 📄 troubleshooting.md
│       │   │
│       │   └── 📂 compliance/
│       │       ├── 📄 gdpr.md
│       │       ├── 📄 pci-dss.md
│       │       ├── 📄 kyc-aml.md
│       │       ├── 📄 data-retention.md
│       │       └── 📄 zim-data-protection.md
│       │
│       ├── 📂 static/
│       │   ├── 📄 favicon.ico
│       │   ├── 📂 images/
│       │   │   ├── 📄 logo.png
│       │   │   └── 📄 screenshots/
│       │   └── 📂 pdfs/
│       │       ├── 📄 user-manual.pdf
│       │       └── 📄 admin-guide.pdf
│       │
│       └── 📂 src/
│           ├── 📄 index.ts
│           ├── 📂 components/
│           │   ├── 📄 api-explorer.tsx
│           │   ├── 📄 code-block.tsx
│           │   └── 📄 theme-switcher.tsx
│           │
│           └── 📂 utils/
│               └── 📄 api-drift-checker.ts
│
│
├── 📂 infrastructure/
│   ├── 📂 terraform/
│   │   ├── 📄 main.tf
│   │   ├── 📄 variables.tf
│   │   ├── 📄 outputs.tf
│   │   ├── 📄 provider.tf
│   │   ├── 📄 backend.tf
│   │   ├── 📄 database.tf
│   │   ├── 📄 compute.tf
│   │   ├── 📄 storage.tf
│   │   ├── 📄 network.tf
│   │   ├── 📄 security.tf
│   │   ├── 📄 dns.tf
│   │   ├── 📄 email.tf
│   │   ├── 📄 monitoring.tf
│   │   └── 📂 modules/
│   │       ├── 📂 cluster/
│   │       │   ├── 📄 main.tf
│   │       │   ├── 📄 variables.tf
│   │       │   └── 📄 outputs.tf
│   │       ├── 📂 database/
│   │       │   ├── 📄 main.tf
│   │       │   ├── 📄 variables.tf
│   │       │   └── 📄 outputs.tf
│   │       ├── 📂 networking/
│   │       │   ├── 📄 main.tf
│   │       │   ├── 📄 variables.tf
│   │       │   └── 📄 outputs.tf
│   │       └── 📂 security/
│   │           ├── 📄 main.tf
│   │           ├── 📄 variables.tf
│   │           └── 📄 outputs.tf
│   │
│   ├── 📂 kubernetes/
│   │   ├── 📂 base/
│   │   │   ├── 📄 namespace.yaml
│   │   │   ├── 📄 service-accounts.yaml
│   │   │   └── 📄 rbac.yaml
│   │   │
│   │   ├── 📂 overlays/
│   │   │   ├── 📂 staging/
│   │   │   │   ├── 📄 kustomization.yaml
│   │   │   │   └── 📄 patch.yaml
│   │   │   └── 📂 production/
│   │   │       ├── 📄 kustomization.yaml
│   │   │       └── 📄 patch.yaml
│   │   │
│   │   ├── 📂 apps/
│   │   │   ├── 📂 backend/
│   │   │   │   ├── 📄 deployment.yaml
│   │   │   │   ├── 📄 service.yaml
│   │   │   │   ├── 📄 ingress.yaml
│   │   │   │   ├── 📄 hpa.yaml
│   │   │   │   ├── 📄 pdb.yaml
│   │   │   │   └── 📄 configmap.yaml
│   │   │   │
│   │   │   ├── 📂 frontend/
│   │   │   │   ├── 📄 deployment.yaml
│   │   │   │   ├── 📄 service.yaml
│   │   │   │   ├── 📄 ingress.yaml
│   │   │   │   ├── 📄 hpa.yaml
│   │   │   │   └── 📄 configmap.yaml
│   │   │   │
│   │   │   ├── 📂 workers/
│   │   │   │   ├── 📄 deployment.yaml
│   │   │   │   ├── 📄 service.yaml
│   │   │   │   └── 📄 hpa.yaml
│   │   │   │
│   │   │   ├── 📂 redis/
│   │   │   │   ├── 📄 statefulset.yaml
│   │   │   │   └── 📄 service.yaml
│   │   │   │
│   │   │   ├── 📂 postgres/
│   │   │   │   ├── 📄 statefulset.yaml
│   │   │   │   ├── 📄 service.yaml
│   │   │   │   └── 📄 backup.yaml
│   │   │   │
│   │   │   └── 📂 monitoring/
│   │   │       ├── 📄 prometheus.yaml
│   │   │       ├── 📄 grafana.yaml
│   │   │       └── 📄 loki.yaml
│   │   │
│   │   ├── 📂 network/
│   │   │   ├── 📄 network-policies.yaml
│   │   │   ├── 📄 service-mesh.yaml
│   │   │   └── 📄 ingress-controller.yaml
│   │   │
│   │   └── 📂 security/
│   │       ├── 📄 pod-security-policies.yaml
│   │       ├── 📄 secrets.yaml
│   │       └── 📄 vault-config.yaml
│   │
│   ├── 📂 docker/
│   │   ├── 📄 Dockerfile.backend
│   │   ├── 📄 Dockerfile.frontend
│   │   ├── 📄 Dockerfile.worker
│   │   ├── 📄 Dockerfile.docs
│   │   └── 📄 Dockerfile.mobile
│   │
│   ├── 📂 scripts/
│   │   ├── 📄 deploy.sh
│   │   ├── 📄 deploy-prod.sh
│   │   ├── 📄 backup.sh
│   │   ├── 📄 restore.sh
│   │   ├── 📄 seed-national-structure.ts
│   │   ├── 📄 seed-district-admin.ts
│   │   ├── 📄 migrate-schools.ts
│   │   ├── 📄 generate-test-data.ts
│   │   ├── 📄 import-zimsec-results.ts
│   │   ├── 📄 export-eternal-archive.ts
│   │   ├── 📄 setup-domains.sh
│   │   ├── 📄 provision-emails.sh
│   │   ├── 📄 send-parent-credentials.ts
│   │   ├── 📄 generate-blockchain-hashes.ts
│   │   ├── 📄 clean-logs.sh
│   │   └── 📂 security/
│   │       ├── 📄 secrets-scan.sh
│   │       ├── 📄 dependency-audit.sh
│   │       ├── 📄 container-scan.sh
│   │       ├── 📄 iac-scan.sh
│   │       ├── 📄 waf-test.sh
│   │       ├── 📄 rotation-verification.sh
│   │       ├── 📄 forensic-collection.sh
│   │       ├── 📄 security-baseline-check.sh
│   │       ├── 📄 compliance-report-generator.sh
│   │       └── 📄 security-health-check.sh
│   │
│   └── 📂 monitoring/
│       ├── 📂 prometheus/
│       │   ├── 📄 prometheus.yml
│       │   ├── 📄 rules.yml
│       │   └── 📂 alerts/
│       │       ├── 📄 backend-alerts.yml
│       │       ├── 📄 database-alerts.yml
│       │       ├── 📄 queue-alerts.yml
│       │       └── 📄 system-alerts.yml
│       │
│       ├── 📂 grafana/
│       │   ├── 📄 datasources.yml
│       │   └── 📂 dashboards/
│       │       ├── 📄 kubernetes.json
│       │       ├── 📄 backend.json
│       │       ├── 📄 database.json
│       │       ├── 📄 queue.json
│       │       ├── 📄 security.json
│       │       └── 📄 business.json
│       │
│       ├── 📂 loki/
│       │   └── 📄 loki-config.yml
│       │
│       └── 📂 alertmanager/
│           └── 📄 alertmanager.yml
│
│
├── 📂 scripts/
│   ├── 📂 deployment/
│   │   ├── 📄 deploy.sh
│   │   ├── 📄 deploy-prod.sh
│   │   ├── 📄 rollback.sh
│   │   └── 📄 health-check.sh
│   │
│   ├── 📂 database/
│   │   ├── 📄 backup.sh
│   │   ├── 📄 restore.sh
│   │   ├── 📄 migrate.sh
│   │   ├── 📄 seed.sh
│   │   └── 📄 validate-schema.sh
│   │
│   ├── 📂 data/
│   │   ├── 📄 seed-national-structure.ts
│   │   ├── 📄 seed-provincial-structure.ts
│   │   ├── 📄 seed-district-structure.ts
│   │   ├── 📄 migrate-schools.ts
│   │   ├── 📄 generate-test-data.ts
│   │   ├── 📄 import-zimsec-results.ts
│   │   ├── 📄 export-eternal-archive.ts
│   │   ├── 📄 generate-blockchain-hashes.ts
│   │   └── 📄 anonymize-data.ts
│   │
│   ├── 📂 automation/
│   │   ├── 📄 setup-domains.sh
│   │   ├── 📄 provision-emails.sh
│   │   ├── 📄 send-parent-credentials.ts
│   │   ├── 📄 generate-reports.ts
│   │   ├── 📄 send-notifications.ts
│   │   └── 📄 sync-psc-data.ts
│   │
│   └── 📂 maintenance/
│       ├── 📄 clean-logs.sh
│       ├── 📄 rotate-secrets.sh
│       ├── 📄 update-certificates.sh
│       └── 📄 performance-test.sh
│
│
└── 📂 .github/
    └── 📂 workflows/
        ├── 📄 ci.yml
        ├── 📄 cd-staging.yml
        ├── 📄 cd-production.yml
        ├── 📄 security-scan.yml
        ├── 📄 docker-scan.yml
        ├── 📄 dependency-vulnerability-scan.yml
        ├── 📄 iac-security-scan.yml
        ├── 📄 container-signing.yml
        ├── 📄 waf-test.yml
        ├── 📄 compliance-check.yml
        ├── 📄 security-chaos-engineering.yml
        ├── 📄 security-release-gate.yml
        ├── 📄 backup.yml
        ├── 📄 docs-deploy.yml
        └── 📄 mobile-test.yml
