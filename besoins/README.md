# Real Estate Agency System

## Project Overview

A modern web-based system for managing real estate property listings in a professional agency setting. The application ensures high data accuracy through mandatory admin approval, role-based access control, intuitive public browsing with advanced search/filtering, and simple inquiry submission.

## Key Features

### Property Listing Management
- Agents/assistants can create and update property listings.
- Listings remain **draft/inactive** until explicitly approved by an admin.
- Approved listings become publicly visible; rejected listings can be edited and resubmitted.

### Role-Based Access Control
Three distinct user roles with strict permissions:

| Role       | Responsibilities / Access                                                                 |
|------------|-------------------------------------------------------------------------------------------|
| **Admin**  | Full system oversight: approve/reject listings, manage users, access all data             |
| **Assistant** | Create, edit, and submit listings for approval; view own and approved listings            |
| **Visitor** (public) | Browse approved listings, use search/filter, view details, submit inquiries               |

### Public Search & Browsing
- Filterable property search by:
  - Price range
  - Location (city, neighborhood, etc.)
  - Property type (house, apartment, condo, land, etc.)
  - Bedrooms/bathrooms
  - Surface area
  - Other common criteria
- Detailed property view with photos, description, features, and contact form.

### Inquiry / Contact System
- Simple "Contact us about this property" form on each public listing.
- Submissions are tied to the specific property and notified to agency staff.

### Quality Control Workflow
- Mandatory review step: every new or updated listing requires admin approval before going live.
- Admin dashboard shows pending listings with approve/reject actions and optional feedback.

### User Experience
- Clean, intuitive backend interface built for non-technical staff.
- Responsive public frontend optimized for desktop and mobile browsing.

## Non-Functional Requirements
- **Security**: Role-based authorization (Laravel Policies/Gates), protected routes, CSRF protection, input validation.
- **Performance**: Efficient querying with Eloquent, indexed search fields, pagination on listings.
- **Accessibility**: Semantic HTML, ARIA labels, keyboard navigation support.
- **Maintainability**: Clean architecture, strict typing (PHP 8.3+), Laravel 12 conventions.

## Target Tech Stack (Recommended)
- **Backend**: Laravel 12 (PHP 8.3+)
- **Frontend**: Blade templates + Tailwind CSS 3 + Alpine.js (for interactivity without heavy SPA)
- **Database**: MySQL / PostgreSQL
- **Authentication**: Laravel Breeze or Jetstream (team features)
- **Authorization**: Laravel Policies + Gates
- **File Storage**: Listings photos via Laravel filesystem (local or S3)