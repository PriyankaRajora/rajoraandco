# Changelog — rajoraandco.com

All notable changes to this project are documented here.
This file is automatically updated when a pull request is merged into `main`.

---

## [2026-03-27] — Deployment Fix

**Branch:** `claude/fix-deployment-issue-7p2qH`
**Merged by:** PriyankaRajora

### Changes
- Removed duplicate workflow file `azure-static-web-apps.yml` that referenced a non-existent secret (`AZURE_STATIC_WEB_APPS_API_TOKEN`), causing deployment failures on every push to `main`.
- Fixed `output_location` from `"."` to `""` in `azure-static-web-apps-ashy-beach-03042b600.yml` — correct setting for a static HTML site with no build step.

### Hosting
- **Platform:** Azure Static Web Apps
- **Resource:** `ashy-beach-03042b600`
- **Workflow:** `.github/workflows/azure-static-web-apps-ashy-beach-03042b600.yml`
- **Deploys on:** Push to `main` branch

---

## [2026-03-27] — Initial Setup

**Committed by:** PriyankaRajora

### Changes
- Uploaded initial website files for [rajoraandco.com](https://www.rajoraandco.com)
- Added `staticwebapp.config.json` to route all paths to `index.html` (SPA-style routing)
- Added Azure Static Web Apps CI/CD workflow

---
