# React Admin Dashboard

![CI](https://github.com/aayxshkumar/react-admin-dashboard/actions/workflows/ci.yml/badge.svg)

> Learning project from January 2024, built following a React admin-dashboard tutorial.

An admin dashboard UI built with React and Material UI, written while following a tutorial. All data is hard-coded sample data in the source; there is no backend.

## Features

- Home page with summary widgets (users, orders, earnings, balance), a circular sales progress chart, a revenue area chart and a latest-transactions table
- List page built on the MUI data grid, with view and delete actions (delete only updates local state); the users and products routes both render the sample user list
- Single item page with details, a spending chart and a transactions table
- "Add new" forms for users and products, with an image preview for the selected file
- Light and dark mode toggle, managed with React context and a reducer

## Tech stack

- React 17, React Router 6
- Material UI 5 (`@mui/material`, `@mui/icons-material`, `@mui/x-data-grid`)
- Recharts, `react-circular-progressbar`
- Sass
- Create React App (`react-scripts` 5)

## Getting started

Requires Node.js 22.

```bash
git clone https://github.com/aayxshkumar/react-admin-dashboard.git
cd react-admin-dashboard
npm ci
npm start        # dev server on http://localhost:3000
npm run build    # production build into build/
```

The `.npmrc` sets `legacy-peer-deps=true` so `npm ci` installs the dependency tree recorded in `package-lock.json`.

No environment variables are needed.
