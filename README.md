# Conference Expense Planner

A React + Redux Toolkit single-page app for estimating the cost of a conference by choosing venue rooms. The venue selection is implemented; the add-ons, meals and cost summary sections are scaffolded but not yet built.

## Features

- Landing page with a "Get Started" button and an About Us section
- Navigation bar with links to the Venue, Add-ons and Meals sections
- Venue room selection from five room types, each with an image, name and price
- Quantity controls (+ / -) per room, with the Auditorium Hall limited to 3 bookings
- Running venue total calculated from the Redux store

## Status

Work in progress. The following parts exist only as placeholders in the code:

- Add-ons and Meals sections (`avSlice.js` and `mealsSlice.js` have no data or reducer logic yet)
- The "Show Details" cost summary (`TotalCost.jsx` renders an empty layout)

## Tech stack

| Area | Technology |
| --- | --- |
| UI | React 18 |
| State management | Redux Toolkit, React Redux |
| Build tool / dev server | Vite 5 |
| Linting | ESLint (react, react-hooks, react-refresh plugins) |

## Project structure

```
src/
├── App.jsx              # Landing page and layout
├── ConferenceEvent.jsx  # Venue / add-ons / meals selection
├── TotalCost.jsx        # Cost summary (placeholder)
├── AboutUs.jsx          # About Us text
├── store.js             # Redux store
├── venueSlice.js        # Venue rooms, prices and quantity reducers
├── avSlice.js           # Add-ons slice (placeholder)
└── mealsSlice.js        # Meals slice (placeholder)
```

## Getting started

Requires Node.js and npm.

```bash
npm install
npm run dev
```

Then open the local URL printed by Vite. Other scripts: `npm run build`, `npm run lint`.

---

Learning project based on IBM Skills Network starter code (Apache 2.0, see `LICENSE`).
