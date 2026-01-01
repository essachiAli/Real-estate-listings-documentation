### Product Backlog
| Epic | User Story | Acceptance Criteria | Points |
|------|------------|---------------------|--------|
| Visitor Interface | As a visitor, I want to browse/filter/search properties so I can find suitable listings. | Filters (price, location, type); pagination; detail view with images/contact form. | 8 |
| | As a visitor, I want to contact about a property so I can inquire easily. | Form submission; email notification; no auth required. | 5 |
| Back-Office CRUD | As an assistant, I want to create/update/submit listings for approval so I can manage inventory. | Form with fields (title, price, etc.); image upload; status tracking (draft/pending/approved). | 13 |
| | As an admin, I want to approve/reject listings so I ensure quality. | Review queue; notifications; update status. | 8 |
| Auth & Roles | As a user, I want to login/logout with roles so I access only relevant features. | RBAC: Visitors (anon), Assistants (CRUD), Admins (all); secure sessions. | 13 |
| Community | As a visitor, I want to view/comment on properties so I engage with listings. | Comment moderation; threaded replies; admin approval if needed. | 8 |
| | As an admin, I want to manage comments so I maintain quality. | CRUD for comments; spam filters. | 5 |
| API REST | As a developer, I want a REST API to expose data so the mobile app can consume it. | Endpoints for properties, auth; JSON responses; Sanctum tokens. | 13 |
| Mobile App | As a mobile user, I want an Android app to browse/contact so I access on-the-go. | Kotlin app; API integration; offline support basics. | 13 |
