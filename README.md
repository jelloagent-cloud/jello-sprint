# Jello Editing — Sprint 02

Live race page for Sprint 02 (12 Oct – 12 Nov 2026). Prize: iPhone 18 Pro.

- `index.html` — the whole page ("Sprint 02 Lanes"): glass "Enter the race" start, coloured lanes seen from above,
  one car per editor, click a car to follow it, batch rows open the ClickUp task.
- `vercel.json` — sends `/api/*` to the existing leaderboard site (leaderboard-dusky-eight.vercel.app), which reads
  ClickUp live. No ClickUp token lives in this repo; points rules and overrides stay in `leaderboard-app/api/leaderboard.js`.
- Not indexed by search engines (`noindex`). Anyone with the link can open it.

Deploys: every commit to `main` deploys on Vercel automatically.
If the page shows "Preview" instead of "Live", the leaderboard site hasn't been deployed with the sprint API yet
(run `npx vercel --prod` in `leaderboard-app`).
