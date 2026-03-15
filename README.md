# Shop-Way

> Navigate stores like you own them. Find any product on any shelf — without asking anyone.

---

## What is Shop-Way?

Shop-Way is a PWA (Progressive Web App) that helps customers navigate inside retail stores and find products on specific shelves — fast, independently, and without needing to flag down a store consultant.

The app works in a browser but is optimized for mobile, so it feels native on a phone. The MVP will be hosted on GitHub Pages.

---

## User Flow

```
Enter store address
       ↓
Select store on map
       ↓
View store layout (shelf map)
       ↓
Search for a product category (e.g. "mascara", "lipstick")
       ↓
Select a brand
       ↓
Get a route: store entrance → exact shelf
```

---

## Proposed MVP Tech Stack

### Frontend
- **React** — component-based UI, wide ecosystem, easy to deploy as a static site
- **TypeScript** — type safety, better DX
- **Vite** — fast build tool, ideal for GitHub Pages deployment
- **Leaflet.js** or **svg-pan-zoom** — for rendering interactive store floor plans and route overlays

### Backend
- **Python** — as requested
- **FastAPI** — lightweight, async, auto-generates OpenAPI docs; perfect for an MVP REST API
- **SQLite** — zero-config database for MVP; stores store layouts, product locations, brands

### Hosting
- **Frontend:** GitHub Pages (via `gh-pages` branch)
- **Backend:** Railway or Render (free tier, Python-friendly, easy deploys from GitHub)

### Data Format
- Store layouts stored as JSON (shelf coordinates, zones)
- Routes calculated on the backend as sequences of coordinates

---

## MVP Scope

- [ ] Store search by address
- [ ] Static store layout viewer (floor plan with labeled shelves)
- [ ] Product category search
- [ ] Brand selection within a category
- [ ] Route display from entrance to target shelf
- [ ] Mobile-first responsive UI

---

## Out of Scope for MVP

- Real-time inventory data
- User accounts / history
- Multiple stores per chain synced live
- Indoor GPS / AR navigation

---

## Project Status

**Stage:** Planning / MVP development in progress
