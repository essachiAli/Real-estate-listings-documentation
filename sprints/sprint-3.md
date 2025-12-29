## 🟠 Sprint 3 : Auth & Rôles (Sécurité RBAC)

**Sprint Goal:** Secure the system with strict role separation.

### User Stories

| ID | User Story                                     | Points |
| -- | ---------------------------------------------- | ------ |
| A1 | As a user, I want to authenticate securely     | 5      |
| A2 | As an admin, I want full control over listings | 5      |
| A3 | As an assistant, I want limited CRUD access    | 5      |
| A4 | As a system, I want role-based access control  | 3      |

### Deliverables

* Authentication (login/logout)
* Roles: Admin / Assistant / Visitor
* Policies & middleware
* Admin validation of listings

**DoD**

* Assistants cannot publish
* Admin approval required
* Visitors blocked from back-office

---