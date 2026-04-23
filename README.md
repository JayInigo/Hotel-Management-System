# Hotel Management System — Check-In Log

## Business App Idea
A Hotel Management System check-in log that allows hotel staff to record
site visits, client interactions, and property inspections. Staff can
capture photos, log GPS coordinates, and store room-specific details
for accountability and record-keeping.

## Collection Name & Fields
**Collection:** `hotel_checkins`

| Field | Type | Description |
|-------|------|-------------|
| businessName | string | Name of hotel/branch visited |
| note | string | Visit notes |
| roomType | string | Room category (Deluxe, Suite, etc.) |
| guestStatus | string | Check-In / Check-Out / Staying |
| photoUrl | string | Firebase Storage download URL |
| lat | number | GPS latitude |
| lng | number | GPS longitude |
| createdBy | string | Group identifier |
| proofLabel | string | e.g. GroupName-Hotel-0423 |
| createdAt | timestamp | Server timestamp |

## Steps to Run
1. Clone the repo
2. Run `flutter pub get`
3. Add your own `google-services.json` (Android) — not committed
4. Run `flutter run`

## Screenshots
- `screenshots/list_screen.png` — Log List with entries
- `screenshots/add_screen.png` — Add screen with photo + location
- `screenshots/firestore_doc.png` — Firestore document view
- `screenshots/storage_file.png` — Firebase Storage uploaded image