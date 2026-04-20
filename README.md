# qbo-app-legal

Static site hosting the EULA and Privacy Policy for the Claude Vision
QuickBooks Online integration (operated by MTAG LLC, d/b/a Rackley
Consulting), required by Intuit before production credentials are issued.

## Deploy to GitHub Pages

1. Create a new public repo on GitHub, e.g. `craincorp/qbo-app-legal`.
2. In this directory:
   ```
   cd c:/projects/qbo-app-legal
   git init
   git add .
   git commit -m "Initial EULA and privacy policy"
   git branch -M main
   git remote add origin https://github.com/<your-org>/qbo-app-legal.git
   git push -u origin main
   ```
3. In the GitHub repo → **Settings** → **Pages** → set Source to `main` branch, `/ (root)` folder. Save.
4. Wait ~1 minute. Your site will be live at:
   ```
   https://<your-org>.github.io/qbo-app-legal/
   ```
5. Paste these URLs into Intuit's app submission form:
   - **EULA URL**: `https://<your-org>.github.io/qbo-app-legal/eula.html`
   - **Privacy policy URL**: `https://<your-org>.github.io/qbo-app-legal/privacy.html`

## Editing

- [index.html](index.html) — landing page linking to both docs
- [eula.html](eula.html) — End-User License Agreement
- [privacy.html](privacy.html) — Privacy policy

Both documents are deliberately minimal — the app is an internal tool for
MTAG LLC (d/b/a Rackley Consulting), not a marketplace product. If the
governing-law state is wrong, edit in place and push.
