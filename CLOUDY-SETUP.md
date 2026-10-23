# Cloudy — Osiris UI rebrand

Cloudy is a UI/branding customization of the open-source Osiris intelligence dashboard. Original source: https://github.com/simplifaisoul/osiris. The original MIT LICENSE is retained.

## Run locally

1. Install Node.js compatible with Next.js 16 (Node.js 20.9+).
2. Run `npm ci` then `npm run dev`.
3. Open http://localhost:3000.
4. For production use `npm run build` and `npm start`.
5. Configure `.env` using `.env.example` for external integrations. Set `NEXT_PUBLIC_SITE_URL` to your real deployment URL when deploying.

## Scope

Changed branding, favicon/app icons, home header logo, main screen title, web metadata, PWA manifest and core theme styling. No intelligence API endpoints, data ingestion, map components or backend implementation were intentionally changed. The alternate Ghost theme remains available. Some original Osiris names remain in internal identifiers, source attribution, technical API strings and documentation to avoid breaking integration compatibility. External service-dependent features require their own configuration and testing.
