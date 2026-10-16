# Lab8ApiImplementation-client (front-end)

React + TypeScript + Vite UI for the **Lab8ApiImplementation** API (separate repo).

## Run locally

```bash
npm install
npm run dev          # http://localhost:5173
```

The API URL comes from `VITE_API_URL`. For local development it is set in `.env.development`
(`http://localhost:5079`), so start the API repo first.

## Build and deploy (e.g. Vercel, Netlify, Azure Static Web Apps)

1. On the hosting platform, set the environment variable
   `VITE_API_URL=https://<your-api-domain>` (no trailing slash needed).
   Vite reads it at **build time**, so rebuild after changing it.
2. Build command: `npm run build`, output folder: `dist`.
3. In the API's settings, add this site's URL to CORS:
   `Cors__AllowedOrigins__0=https://<your-frontend-domain>`.

To build locally for production, copy `.env.example` to `.env.production.local`, set the URL, and run `npm run build`.
