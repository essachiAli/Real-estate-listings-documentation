# 🔵 Sprint 4: Communauté (Commentaires)

## 📋 Pré-requis Pédagogiques
- Sessions: Relations/Polymorphic.
- Labs: Blade Components for Comments.

## 1. Besoin
Objectif: Visitors comment on properties; Admins moderate.

## 2. 🔍 Analyse
Use Cases: Post/view comments; Moderation.
Diagram: Property-ContactInquiry (adapt for comments).

## 3. 🏗️ Conception
DB: ContactInquiry as Comment model.
UI: Comment section on property detail.

## 4. 💻 Réalisation (Tâches)
- [ ] Migrations: Comment model linked to Property/User.
- [ ] CommentController: Store/show.
- [ ] Service: CommentService (moderation logic).
- [ ] Views: Add comments to property.show.blade.php.
- [ ] Admin moderation queue.

Sprint Goal: Interactive community features. Burndown: 13 points. DoD: Spam prevention.