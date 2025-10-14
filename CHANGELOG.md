# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

### Phase 1: Database & Core (In Progress)
- [ ] Multi-location database schema
- [ ] Location management class
- [ ] Database migration script

### Phase 2-7: See ROADMAP.md

---

## [2.0.0-alpha] - 2025-01-XX

### Added - Multi-Location Support
- Multi-location architecture
- Location selector popup
- Location-specific settings
- Timezone support per location
- Phone validation per location

### Added - Smart Booking Flow
- 2-step booking process
- Real-time availability check
- Alternative time suggestions (±2 slots)
- Email confirmation with token
- Auto-confirm via email link

### Added - Enhanced Security
- Token-based email confirmation
- Token expiration (2 hours)
- Rate limiting for confirmation endpoint
- Enhanced permission system
- Location-based access control

### Added - Role System
- Custom role: `restaurant_location_manager`
- Super Admin role (all locations)
- Location assignment per user
- Permission checks per location

### Changed
- Refactored booking flow (1-step → 2-step)
- Email system (direct confirm → token-based)
- Admin dashboard (single → multi-location)

### Database Changes
- Added `wp_rb_locations` table
- Added `location` column to existing tables
- Added `wp_rb_booking_tokens` table
- Added indexes for performance

---

## [1.0.0] - 2024-XX-XX

### Initial Release
- Single location booking system
- Admin dashboard
- Email notifications
- Multi-language (Vi, En, Ja)
- Customer CRM
- Table management

---

## Migration Notes

### From v1.0.0 to v2.0.0
See [MIGRATION.md](docs/MIGRATION.md)

**Breaking Changes:**
- Database schema updated
- Existing bookings need location assignment
- Admin UI restructured
```

---

### 4. `LICENSE`
```
GNU GENERAL PUBLIC LICENSE
Version 2, June 1991
...
(Copy từ: https://www.gnu.org/licenses/old-licenses/gpl-2.0.txt)
