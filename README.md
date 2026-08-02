# Distill

Aha moments from books, stored forever.

Single file: `index.html`. No build step, no dependencies, no keys in the code.

## Live site
GitHub Pages serves `index.html` from the root of `main`.
Every push to `main` redeploys automatically, usually within a minute.

## Setup (once)
1. **Settings → Pages** → Source: *Deploy from a branch* → `main` / `/ (root)` → Save
2. Wait ~1 min, then open `https://<your-username>.github.io/<repo>/`
3. On your phone: Share → **Add to Home Screen**
4. Open it from the home screen icon → **Settings** → Copy SQL → run it in your
   Supabase project's SQL editor → paste your Project URL + anon public key → Connect

Your Supabase credentials are typed into the app at runtime and stored on your
device. They are never in this repo, which is why it's safe for the repo to be public.

## Editing
Change `index.html`, commit, done. You can edit straight from github.com on a phone:
open the file → pencil icon → Commit changes.

Your data lives in Supabase, not in the page, so shipping a new version never
touches your aha moments.
