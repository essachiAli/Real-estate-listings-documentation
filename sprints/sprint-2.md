# 🟡 Sprint 2: Publication (Back-Office CRUD)

## 📋 Pré-requis Pédagogiques
- Sessions: Forms/Validation; File Uploads.
- Labs: Image Processing with Intervention.

## 1. Besoin
Objectif: Assistants create/update listings; Submit for approval.

## 2. 🔍 Analyse
Use Cases: CRUD properties; Image upload; Status workflow (draft/pending).
Diagram: Property methods (create/edit/submitForApproval).

## 3. 🏗️ Conception
DB: Add status enum to Property.
UI: Admin dashboard forms.

## 4. 💻 Réalisation (Tâches)
- [ ] Branch sprint-2 from sprint-1.
- [ ] AdminController: CRUD actions.
- [ ] Service: PropertyService (create/update with validation).
- [ ] Views: admin/property/create.blade.php, edit.blade.php.
- [ ] Upload handling: Store images, set primary.
- [ ] Workflow: Submit button updates status to pending.

Sprint Goal: Back-office for listing management. Burndown: 21 points. DoD: Integration tests for CRUD.
