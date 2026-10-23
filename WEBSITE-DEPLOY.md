# Cloudy — Website Deployment Guide

Cloudy is a **Next.js website**, not a native desktop app. It contains server-side API routes, so do not use a static HTML export or upload the ZIP directly to a static file host.

## Deploy on Vercel (recommended)

1. Extract this ZIP and upload the contents of the `Cloudy` folder to a GitHub repository (keep `package.json` at the repository root).
2. Open https://vercel.com/new, import your GitHub repository, and select the **Next.js** framework preset.
3. Leave the build command as `npm run build` and install command as `npm ci`.
4. Configure any needed environment variables from `.env.example` in Vercel's project settings. Do **not** commit actual API keys.
5. Deploy. Vercel provides a public HTTPS website address, and you can attach your own domain later.

## Run locally

Requires a Node.js version supported by Next.js 16 (Node.js 20.9+).

```bash
npm ci
cp .env.example .env.local  # on Windows, copy .env.example .env.local
npm run dev
```

Open http://localhost:3000.

## Important limitations

- Features that depend on API keys, external feeds, geographic permissions, or external services need those services configured and available.
- Some server-side features may need a persistent server or hosting configuration; test those individually after deployment.
- This archive includes the website source code, not a pre-built hosted website.
- The project has not been live-deployed or end-to-end verified as part of packaging.
- Keep the upstream LICENSE and required notices intact.
