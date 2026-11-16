# CampusEngage

A responsive React + Vite campus club management demo based on the supplied screenshots. The interface uses a warm orange / cream / terracotta palette in place of the original blue accents.

## Run locally

Requirements: Node.js 20+ and npm.

```bash
npm install
npm run dev
```

Open the local URL printed by Vite (usually http://localhost:5173).

## Production build

```bash
npm run build
npm run preview
```

The production site is generated in `dist/`.

## Deploy

### Vercel
1. Extract the ZIP and push the `campusengage` folder to a Git repository.
2. Import the repository in Vercel.
3. Framework preset: **Vite**; Build command: `npm run build`; Output directory: `dist`.

### Netlify
1. Import the repository in Netlify.
2. Build command: `npm run build`; Publish directory: `dist`.

You can also upload the generated `dist/` folder to any static hosting provider.

## Demo access

The sign-in screen is a front-end demo. Choose **Member** or **Team Leader** and click Sign in. The ID/password fields are illustrative; no server authentication is performed.

## Included interactions

- Role switching between member and team leader views
- Navigation between dashboards and portal sections
- Create, edit, and delete tasks
- Accept tasks and submit them for review
- Create events and register interest
- Search clubs and toggle joined status
- Submit feedback and save leader responses
- Update workload status
- Browser `localStorage` persistence for demo data

## Production note

This ZIP is a deployable front-end prototype. It stores demo changes in the visitor's browser using `localStorage`; it does not include a hosted database, real user accounts, email notifications, or server-side authorization. Before using it with real students, connect a backend (for example Supabase or Firebase), implement secure authentication and role-based access, and move all shared data to that backend.
