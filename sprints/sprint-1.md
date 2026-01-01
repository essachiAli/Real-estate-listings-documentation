# 🟢 Sprint 1: Visiteur (Interface Publique)

## 📋 Pré-requis Pédagogiques
- Sessions: Laravel Routing/Controllers/Blade; Eloquent Basics.
- Labs: Tailwind Setup with Vite; AJAX for Search.

## 1. Besoin
Objectif: MVP for visitors to browse/search properties (read-only).

## 2. 🔍 Analyse
Use Cases: List/filter properties; View details; Search by keywords/price/location/type.
Diagram: Reference provided class diagram (Property, Category relations).

## 3. 🏗️ Conception
DB/Models: Property, Category, PropertyImage.
UI: Public layouts; Search page with filters.

## 4. 💻 Réalisation (Tâches)
- [ ] Setup Laravel + Git (branch sprint-1); Config Tailwind/Preline via Vite.
- [ ] Migrations/Seeders: Property, Category (factory 20 properties).
- [ ] PublicController: index (list), show (detail).
- [ ] Service: PropertyService (getPublicProperties with filters).
- [ ] Views: home.blade.php (grid); property.show.blade.php (details + images).
- [ ] AJAX search endpoint for dynamic filtering.

Sprint Goal: Functional public interface. Burndown: 13 points. DoD: 80% code coverage, UI tests.
