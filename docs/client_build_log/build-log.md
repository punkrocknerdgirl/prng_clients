# Client Build Log

## 2026-07-22 — Reusable Client Dashboard Foundation

- Approved the Kropf Transfer dashboard mockup as the v1 interface.
- Added reusable dashboard files to the `prng_clients` repository:
  - `dashboards/kropf/index.html`
  - `dashboards/kropf/theme-kt.css`
  - `dashboards/shared/layout.css`
- Separated shared layout styling from client-specific theme styling.
- Verified the dashboard works locally after moving the shared stylesheet.
- Committed and pushed the dashboard foundation to `main`.
- Chose one shared Airtable base for all clients, with client-specific records separated by `client_id`.
- Deferred automated QBO/Make data pulls. Initial dashboard updates will be manual.
- Set the security direction:
  - no live client financial data, credentials, or API keys in GitHub
  - use synthetic data for development
  - protect future client dashboards and data endpoints with Cloudflare Access using approved email addresses and one-time PIN login
  - protect both the dashboard page and its data/API endpoint
- Next step: inspect the existing front-end data structure and build the simplest safe manual-data workflow before adding Airtable, Make, or automation.
