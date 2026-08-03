# Distill

Insights from books, stored forever. Teaching happens in the Claude app.

Single file: `index.html`. No build step. No secrets in the repo — the Firebase
config is pasted into the app at runtime and stored on-device.

## Live site
GitHub Pages serves `index.html` from `main`. Every push redeploys in ~1 min.

## Setup (once)
1. **Firebase**: console.firebase.google.com → Add project → Build → Firestore
   Database → Create database (production mode). Rules tab → paste the rules
   shown in the app's Settings → Publish. Project settings → Your apps →
   Web (`</>`) → register → copy the `firebaseConfig` block.
2. **App**: Settings → paste the whole firebaseConfig → Connect.
   Do this once per device; insights sync realtime after that.
3. **Phone**: open the site in Safari → Share → Add to Home Screen → open from
   the icon → paste the config there too.

Sync is realtime (Firestore listeners): edits and deletes appear on other
open devices in about a second.
