# Airport Management System — Frontend (v2)

This is a clearer, more complete frontend-only implementation of the U Devs task: Airport Management System.
Theme: **black / white / light yellow** — Vite + React, Context API, localStorage persistence.

## What changed vs v1:
- Added custom `useLocalStorage` hook for robust state persistence.
- Reusable UI components: Input, Button, Badge, ConfirmModal.
- Search/Filter for Users & Tickets, validation, and confirmation dialogs.
- Clearer folder structure and improved README instructions.
- Minor demo data and better UX flows.

## How to run
1. Extract `airport-ams-v2.zip` and open the folder in terminal.
2. Install dependencies:
```bash
npm install
```
3. Start dev server:
```bash
npm run dev
```
4. Open the printed local URL (usually http://localhost:5173).

## Features checklist (from PDF)
- Splash screen ✔
- Frontend-only auth (AuthContext) ✔
- User CRUD ✔ (Add/Edit/Delete, search, validation)
- Ticket CRUD (Flights) ✔ (Add/Edit/Delete, search, validation)
- Booking interlink ✔ (book/unbook users to flights)
- Context API usage ✔ (AuthContext, UserContext, TicketContext)
- Responsive design ✔
- Routing ✔ (Splash, Login, Register, Dashboard, Users, Tickets, Bookings)
- Form validation, confirmation modals ✔

## Folder structure
/src
  /components  Reusable UI (Input, Button, ConfirmModal, Badge, Layout)
  /context     AuthContext, UserContext, TicketContext
  /hooks       useLocalStorage
  /pages       Splash, Login, Register, Dashboard, Users, Tickets, Bookings
  styles.css
  main.jsx, App.jsx

## Notes
- This is frontend-only. Authentication is simulated.
- Data keys in localStorage: `ams_auth`, `ams_users`, `ams_tickets`.
- To reset data, clear localStorage for the site in your browser devtools.

If you'd like: I can (A) convert this to Tailwind or Bootstrap, (B) add export/import CSV, or (C) prepare a GitHub-ready repo with commit-ready files.
