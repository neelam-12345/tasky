# Tasky — Vercel deployment

This is the Vercel-ready standalone Tasky build.

## Deploy with Vercel

1. Create a GitHub repository and upload `index.html` and `vercel.json`.
2. Go to https://vercel.com/new and import the repository.
3. Framework Preset: **Other**.
4. Build Command: leave empty.
5. Output Directory: `.` (or leave the default for a static project).
6. Click **Deploy**.

## Important

This build is the standalone/demo version of Tasky. Accounts, tasks, linked devices and settings are stored in the browser using localStorage. No Python server or SQLite database is required, so it works directly on Vercel.

The original Python + SQLite backend cannot be hosted as a persistent database on Vercel's serverless filesystem. If you need real multi-user persistent accounts/tasks, connect the app to a hosted database such as PostgreSQL and deploy the API as serverless functions.
