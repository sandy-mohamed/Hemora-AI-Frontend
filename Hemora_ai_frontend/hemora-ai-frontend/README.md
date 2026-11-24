# Hemora AI — Frontend Package

Complete frontend interface for **Hemora AI** (Multi-Agent System + PSO Blood Distribution).

## Features Included
- **Bilingual Support:** English (LTR) & Arabic (RTL) toggle.
- **Theme Support:** Clean Medical Light Mode & Deep Navy Dark Mode.
- **Interactive Showcase:** Animated blood bag inspector (FEFO priority) & Cross-Match Compatibility Matrix.
- **Role-Based Login Gate:** `Coordinator`, `Hospital`, and `Blood Bank` roles.
- **Command Center Dashboard:**
  - Live Greater Cairo Map (Leaflet) with animated PSO vs. Traditional routes.
  - Hospital Blood Request form & Blood Bank Add-Units form.
  - Blood Inventory & Expiry (FEFO) monitor.
  - PSO vs. Traditional comparison & convergence charts (Chart.js).

## Backend Integration Guide
Open `index.html` and search for `API_CONFIG` and `API_SERVICE`:
- `POST /api/v1/auth/login` — User & role authentication.
- `POST /api/v1/requests/dispatch` — Submit hospital blood request and receive PSO-selected blood bank + route.
- `POST /api/v1/inventory/add` — Add/update blood bank units and expiry dates.

Replace the mock promises inside `API_SERVICE` with `fetch()` calls to your backend server.
