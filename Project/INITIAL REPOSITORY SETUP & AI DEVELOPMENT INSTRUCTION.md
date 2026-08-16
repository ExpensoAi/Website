EXPENSO AI WEBSITE

INITIAL REPOSITORY SETUP & AI DEVELOPMENT INSTRUCTION

Version: 1.0
Project: Expenso AI Official Website

---

1. OBJECTIVE

Prepare the existing Expenso AI Git repository for development of the official Expenso AI website.

The website will eventually provide:

- Official Expenso AI product information
- Feature documentation
- Premium information
- Help Center
- Troubleshooting
- AI Help Assistant
- Customer support
- Private support chat
- Community discussions
- Feature requests
- Feature voting
- Bug reports
- Product announcements
- Release notes
- User accounts
- Admin dashboard

IMPORTANT:

DO NOT build the complete website during this phase.

This phase is ONLY for:

1. Repository inspection
2. Documentation organization
3. Asset organization
4. Architecture audit
5. Technology assessment
6. Risk identification
7. Implementation planning

---

2. CRITICAL DEVELOPMENT RULE

DO NOT modify existing production code during the audit phase.

DO NOT:

- Delete files
- Rename important existing files
- Replace the existing architecture
- Upgrade dependencies unnecessarily
- Modify the Android application
- Modify the existing backend
- Modify database schemas
- Remove existing functionality
- Change existing APIs
- Change authentication
- Deploy anything

The objective is to understand the existing repository before development begins.

---

3. SOURCE OF TRUTH

The following directory contains the official project specifications:

/docs/

Read every document in "/docs" before producing the audit.

Required documents:

PROJECT_MASTER_SPEC.md
PRODUCT_REQUIREMENTS.md
UI_UX_DESIGN_SYSTEM.md
SITE_MAP.md
USER_FLOWS.md
TECHNICAL_ARCHITECTURE.md
DATABASE_SCHEMA.md
AUTH_SECURITY_PRIVACY.md
HELP_KNOWLEDGE_BASE.md
COMMUNITY_SPECIFICATION.md
SUPPORT_SYSTEM.md
ADMIN_PANEL_SPEC.md
WEBSITE_CONTENT.md
MASTER_AI_DEVELOPMENT_PROMPT.md

Treat these documents as the primary source of truth.

If any document contradicts another document:

1. Identify the conflict.
2. Explain it.
3. Do not silently choose a solution.
4. Mark it as requiring clarification.

---

4. EXISTING EXPENSO AI APPLICATION

The existing Expenso AI Android application is the primary product.

The website must complement the application.

The website must NOT change the core functionality of the Android application.

The website must visually match the existing Expenso AI application.

Important visual references include:

- Official Expenso AI logo
- Dark theme
- Deep black/navy background
- Electric blue
- Cyan
- White typography
- Gray secondary text
- Red financial liability/negative-value indicators
- Dashboard UI
- Credit Card UI
- Analytics UI
- AI UI

---

5. REPOSITORY INSPECTION

Inspect the entire existing repository.

Determine:

Project structure

Identify:

- Root directories
- Applications
- Backend
- Frontend
- AI engine
- Shared libraries
- Scripts
- Tests
- Documentation
- Assets

Technology

Identify:

- Programming languages
- Frameworks
- SDK versions
- Package managers
- Build systems
- Database technologies
- Authentication systems
- APIs
- Cloud services
- Storage systems
- AI services

Existing Expenso architecture

Determine whether the repository currently contains:

- Flutter application
- FastAPI backend
- AI engine
- Database
- Authentication
- Firebase
- Google Drive integration
- Existing APIs
- Existing deployment configuration

Do not assume these exist.

Verify them from the repository.

---

6. WEBSITE REPOSITORY DECISION

Determine whether the website should be:

OPTION A:

A separate repository/project.

OR

OPTION B:

A new "/website" application inside the existing Expenso repository.

Evaluate:

- Existing repository structure
- Shared backend requirements
- Shared authentication
- Shared APIs
- Deployment
- CI/CD
- Maintenance
- Security
- Developer workflow

Recommend one option.

Do NOT implement the recommendation yet.

---

7. DOCUMENTATION AUDIT

Verify that the "/docs" directory contains all required specifications.

Create a table in the audit:

Document| Exists| Complete| Conflicts| Notes

Identify:

- Missing documents
- Duplicate requirements
- Contradictory requirements
- Undefined requirements
- Technical gaps
- Security gaps
- Product gaps

---

8. ASSET AUDIT

Inspect:

/assets

Expected structure:

assets/
├── branding/
├── screenshots/
├── icons/
├── videos/
└── marketing/

Determine:

- Which assets already exist
- Which assets are missing
- Which screenshots are available
- Which logo versions exist
- Which assets need optimization
- Which assets need new versions

DO NOT redesign the logo.

DO NOT replace existing official branding.

---

9. EXISTING CODE REUSE

Identify components and systems that can potentially be reused.

Examples:

- Authentication
- API clients
- Database models
- User management
- Notification system
- Firebase configuration
- Google authentication
- Backend services
- AI provider architecture
- Shared types
- Existing design tokens

For every reusable component explain:

Component:
Location:
Purpose:
Can be reused:
Required changes:
Risk:

Do not duplicate functionality unnecessarily.

---

10. EXISTING BACKEND ANALYSIS

Inspect the current backend if available.

Determine:

- Framework
- API structure
- Authentication
- Database connection
- User model
- Existing endpoints
- Existing services
- CORS configuration
- Deployment
- Environment variables
- Existing API versioning

Determine whether the backend can support the new website.

Identify required additions.

Do not implement backend changes during this audit.

---

11. DATABASE ANALYSIS

Inspect existing database architecture.

Determine:

- Database type
- Schema
- Existing users
- Authentication relationships
- Existing tables
- Migration system
- ORM
- Indexes
- Backup system

Compare the existing schema against:

DATABASE_SCHEMA.md

Identify:

- Reusable tables
- Required new tables
- Conflicting fields
- Migration requirements
- Security concerns

DO NOT modify the database during the audit.

---

12. AUTHENTICATION ANALYSIS

Determine the existing authentication system.

Check whether it supports:

- Google Sign-In
- Email authentication
- Sessions
- User profiles
- Roles
- Admin permissions
- Account deletion
- Password recovery

Compare with:

AUTH_SECURITY_PRIVACY.md

Identify missing capabilities.

---

13. ROLE SYSTEM

Determine whether the existing system supports:

Guest
User
Premium User
Moderator
Support Agent
Admin
Super Admin

If the existing system has different roles, document the differences.

Do not change the role system during the audit.

---

14. API ANALYSIS

Document existing APIs.

For each API identify:

Endpoint
Method
Purpose
Authentication
Request
Response
Used By
Potential Website Reuse
Required Changes

Determine whether API versioning exists.

Preferred structure:

/api/v1/

---

15. SECURITY AUDIT

Perform a preliminary security review.

Check for:

- Secrets committed to repository
- API keys
- Passwords
- Database credentials
- Unsafe environment configuration
- Missing authentication
- Missing authorization
- Insecure file uploads
- Public private data
- Weak admin protection
- Missing rate limiting
- Unsafe CORS
- Missing security headers

DO NOT expose secrets in the audit document.

If a secret is found:

Report:

CRITICAL SECURITY ISSUE

A secret appears to be committed in:
[redacted path]

DO NOT display the secret value.

Recommended action:
Rotate/revoke the credential and move it to secure environment configuration.

---

16. PERFORMANCE AUDIT

Evaluate current infrastructure for:

- Build performance
- Page performance if website exists
- API latency
- Database queries
- Image optimization
- Caching
- CDN
- Server-side rendering
- Static generation

Provide recommendations.

---

17. SEO AUDIT

If a website already exists, inspect:

- Titles
- Descriptions
- Sitemap
- Robots
- Canonical URLs
- Open Graph
- Structured data
- Heading structure
- Accessibility

If no website exists:

State that SEO infrastructure needs to be implemented.

---

18. DEPLOYMENT AUDIT

Determine current deployment infrastructure.

Check for:

- Hosting
- Domain
- DNS
- SSL
- CI/CD
- GitHub Actions
- Environment configuration
- Staging
- Production

Do not deploy anything.

---

19. AI INTEGRATION AUDIT

Determine existing AI architecture.

Check:

- AI providers
- API abstraction
- API keys
- AI engine
- Prompt architecture
- Knowledge retrieval
- Offline AI
- Existing AI provider configuration

Determine what can be reused for the website AI Help Assistant.

IMPORTANT:

Do not expose private AI API keys in the frontend.

---

20. WEBSITE AI HELP REQUIREMENTS

The future AI Help Assistant must use official Expenso AI documentation.

Preferred flow:

User Question
↓
Intent Detection
↓
Knowledge Retrieval
↓
Official Documentation
↓
AI Response
↓
Confidence Evaluation
↓
Answer
OR
Support Escalation

The AI must not invent:

- Product features
- Pricing
- Policies
- Security claims
- App behavior
- Unsupported functionality

---

21. COMMUNITY REQUIREMENTS

Verify whether existing infrastructure can support:

- Posts
- Comments
- Replies
- Voting
- Feature requests
- Bug reports
- Moderation
- Reports
- Notifications

Do not implement these systems during the audit.

Only identify requirements and architecture.

---

22. SUPPORT REQUIREMENTS

Determine whether existing backend infrastructure can support:

- Support tickets
- Ticket statuses
- Ticket assignment
- Support messages
- Private chat
- Attachments
- Notifications
- Agent roles
- Audit logs

Identify missing infrastructure.

---

23. PREMIUM INTEGRATION

Determine how the existing Expenso AI application handles Premium.

Inspect:

- Premium status
- Subscription information
- Google Play integration
- Purchase verification
- User identity
- Subscription backend

Do not modify Premium functionality.

Determine how the website could securely display relevant Premium information.

The website must never trust a client-side Premium flag.

---

24. RECOMMENDED WEBSITE ARCHITECTURE

Based on the audit, recommend an architecture.

The recommendation must cover:

Frontend
Backend
Database
Authentication
Storage
Search
AI
Community
Support
Admin
Deployment

Explain why each component is recommended.

---

25. IMPLEMENTATION ROADMAP

Create a proposed development sequence.

Minimum expected phases:

Phase 0
Repository Audit

Phase 1
Foundation

Phase 2
Design System

Phase 3
Public Website

Phase 4
Authentication

Phase 5
Help Center

Phase 6
Knowledge Base

Phase 7
AI Help Assistant

Phase 8
Support System

Phase 9
Private Support Chat

Phase 10
Community

Phase 11
Feature Requests

Phase 12
Bug Reports

Phase 13
Premium

Phase 14
What's New

Phase 15
User Account

Phase 16
Admin Panel

Phase 17
Moderation

Phase 18
Notifications

Phase 19
Search

Phase 20
SEO

Phase 21
Performance

Phase 22
Accessibility

Phase 23
Security Review

Phase 24
Database Review

Phase 25
Complete Testing

Phase 26
Production Deployment

---

26. RISK REGISTER

Create a risk table:

Risk| Severity| Probability| Impact| Recommendation

Include:

- Existing architecture conflicts
- Authentication conflicts
- Database migration risks
- Security risks
- AI hallucination
- Community abuse
- File upload risks
- Privacy risks
- Premium verification
- Scalability
- Performance
- Deployment

---

27. MISSING INFORMATION

Create a section:

INFORMATION REQUIRED BEFORE DEVELOPMENT

List anything that must be decided before implementation.

Examples:

- Website domain
- Hosting provider
- Exact pricing
- Premium feature list
- Email provider
- Support response policy
- Community moderation policy
- Authentication providers
- Database hosting
- AI provider
- Storage provider

Do not invent missing values.

Mark them:

"REQUIRES DECISION"

---

28. IMPLEMENTATION BACKLOG

Create a prioritized backlog:

P0 — Critical

Required before core website development.

P1 — High

Required for initial production release.

P2 — Medium

Can follow initial release.

P3 — Future

Optional future improvements.

---

29. DO NOT CODE YET

This phase must NOT implement:

- Homepage
- Help Center
- Community
- Support
- AI Assistant
- Database changes
- Authentication changes
- Admin panel

Only inspect and document.

---

30. REQUIRED OUTPUT

At the end of the audit, create:

/docs/IMPLEMENTATION_AUDIT.md

The document must contain:

1. Executive Summary
2. Repository Structure
3. Existing Technology Stack
4. Existing Expenso Architecture
5. Website Architecture Recommendation
6. Existing Components That Can Be Reused
7. Backend Analysis
8. Database Analysis
9. Authentication Analysis
10. API Analysis
11. AI Architecture Analysis
12. Premium Integration Analysis
13. Security Findings
14. Performance Findings
15. SEO Findings
16. Deployment Findings
17. Asset Audit
18. Documentation Audit
19. Missing Requirements
20. Architecture Risks
21. Recommended Technology Stack
22. Development Roadmap
23. Prioritized Backlog
24. Questions Requiring Decisions
25. Final Recommendation

---

31. FINAL RESPONSE FORMAT

After completing the audit, do NOT start implementation.

Return a concise summary containing:

Repository Status

Recommended Architecture

Existing Components We Can Reuse

Critical Problems

Missing Requirements

Recommended Technology Stack

Development Phases

Decisions Required

Ready for Implementation?

Answer:

YES

or

NO

If NO, explain exactly what must be resolved first.

---

32. FINAL INSTRUCTION

The most important requirement is:

DO NOT CODE THE WEBSITE DURING THIS PHASE.

Inspect first.

Understand the existing Expenso AI ecosystem.

Compare it against the documentation.

Identify risks.

Create the implementation audit.

Only after the audit is reviewed and approved should development begin.

END OF DOCUMENT