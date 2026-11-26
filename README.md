# Konbayan Activities

A Vue 3 website for Konbayan's cycling and coffee experiences in North Lombok. Visitors can browse activity details, read FAQs, and send booking requests through WhatsApp with their selections prefilled.

## What it does

- Presents cycling and coffee activities with schedules, inclusions, and pricing.
- Collects booking details and opens a formatted WhatsApp conversation; it does not confirm or process reservations on its own.
- Supports Indonesian and English text in the contact and booking flows.
- Displays a weekly activity board. A separate editor uses `json-server` for local development.
- Uses motion and responsive layouts for the public pages.

## Stack

Vue 3, Vue Router, Tailwind CSS, GSAP, and `json-server` for the local weekly-board data.

## Run locally

```bash
npm install
npm run dev
```

The site runs through Vue CLI. `npm run dev` also starts the local `json-server` expected by the weekly board at `http://localhost:3001`.

## Project structure

- `src/pages/` — home, activities, booking, contact, and weekly-board editor pages.
- `src/data/` — activity, FAQ, and site content.
- `src/utils/contact.js` — bilingual WhatsApp request formatting.
- `src/anim/` — motion helpers.

## Scope and limitations

The booking flow hands requests to WhatsApp. The weekly-board editor and its local `json-server` are development features; they are not a production booking backend or a server-authenticated admin system. Project photos, videos, fonts, and brand assets remain subject to their respective owners' rights.
