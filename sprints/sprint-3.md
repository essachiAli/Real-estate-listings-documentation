# 🟠 Sprint 3: Auth & Rôles (Sécurité RBAC)

## 📋 Pré-requis Pédagogiques
- Sessions: Auth with Breeze; Permissions.
- Labs: Middleware/Policies.

## 1. Besoin
Objectif: Secure access by roles (Visitor anon, Assistant CRUD, Admin approve).

## 2. 🔍 Analyse
Use Cases: Login; Role-based routes; Approval queue for admins.
Diagram: User-Role-Permission relations.

## 3. 🏗️ Conception
Auth: Breeze + Spatie Permission.
Guards: Web for roles.

## 4. 💻 Réalisation (Tâches)
- [ ] Install Breeze (Blade/Tailwind); Spatie Permission.
- [ ] Migrations: Roles (Admin, Assistant), Permissions.
- [ ] Middleware: Protect admin routes.
- [ ] AdminController: approve/reject actions on Property.
- [ ] Views: Login; Approval dashboard.
- [ ] Policies: Assistant can edit own properties only.

Sprint Goal: Role-secured system. Burndown: 13 points. DoD: Security audits.