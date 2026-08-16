# Prompt: Release As Static Web App

```text
Convert or release this calculator as a pure static web app.

Requirements:
- React + TypeScript + Vite
- npm run build generates dist/
- no EXE
- no Electron
- no backend
- no database
- no login
- no analytics
- no external API calls
- all features work offline after build
- customer inputs remain in browser state/local browser storage only
- responsive for desktop and mobile browsers

Recommended:
- Set Vite base to "./" for local file usage.
- If direct file opening is required, inline built JS/CSS into dist/index.html.
- Document how to open dist/index.html in Edge or Chrome.

Important boundary:
A pure static file cannot provide real-time sync between desktop and phone.
Phone access requires either:
- copying the static files to the phone,
- hosting on an internal static file server,
- or adding a local HTTP service, which changes the architecture.

After completion, run:
- npm test -- --run
- npm run build
- project-specific audit scripts

Output:
- changed files
- whether core formulas changed
- test results
- static usage instructions
- remaining privacy/security boundaries
```
