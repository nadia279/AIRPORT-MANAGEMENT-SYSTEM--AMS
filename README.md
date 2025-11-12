# Airport Management System (Frontend-only)

Simple frontend implementation for the U Devs Frontend task (Airport Management System).

Theme: **black, white, light yellow**  
Tooling: **Vite + React** (no backend)  
State: Context API with `localStorage` persistence

## Features
- Splash screen
- Login & Register (frontend-only)
- Users CRUD (Create / Read / Update / Delete)
- Tickets (Flights) CRUD
- Booking system linking users to tickets
- Dashboard with counts
- Responsive layout
- All state managed via Context API (`AuthContext`, `UserContext`, `TicketContext`)

## How to run
1. Install dependencies:
```bash
npm install
```
2. Run dev server:
```bash
npm run dev
```
3. Open http://localhost:5173 (or printed Vite URL)

## Folder structure
```
/src
  /components   Reusable components (Layout, Modal)
  /context      AuthContext, UserContext, TicketContext
  /pages        Splash, Login, Register, Dashboard, Users, Tickets, Bookings
  styles.css    Theme styles
App.jsx
main.jsx
index.html
```

## Notes
- This is a frontend-only solution. Authentication is simulated in `AuthContext`.
- Data persists to `localStorage` under keys: `ams_auth`, `ams_users`, `ams_tickets`.
- The UI aims to be minimal but slightly styled (buttons, modals, confirm prompts).
- Colors: backgrounds use white/light-yellow; text is black.

## Acceptance checklist (from assignment)
- [x] Splash screen implemented
- [x] Routes for required pages
- [x] AuthContext, UserContext, TicketContext used
- [x] CRUD operations work (localStorage)
- [x] Booking interlink implemented
- [x] README included

