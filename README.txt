SUPPLY SCOUT — FLAT IPHONE PWA (v0.2)
====================================

NO NESTED FOLDERS. Everything is at the top level of this ZIP:
  index.html
  manifest.webmanifest
  sw.js
  icon-192.png
  icon-512.png
  README.txt

This is a static iPhone-friendly research PWA. No app-builder credits,
subscription, Python installation, or brokerage connection required.

INSTALL ON IPHONE WITH GITHUB PAGES
----------------------------------
1. In iPhone Files, tap the ZIP to extract it. Open the extracted folder.
2. Open github.com/tristanpeto123-eng/supply-scout in Safari, signed in.
3. Tap Add file > Upload files. Upload the FIVE app files (not the ZIP) into
   the repository root, alongside README.md, NOT into a subfolder:
   index.html, manifest.webmanifest, sw.js, icon-192.png, icon-512.png.
   Depending on iOS GitHub web interface, you may need to upload one by one.
4. Tap Commit changes. If GitHub refuses selecting multiple items in Safari,
   tap each one individually or use the iPhone Files upload picker.
5. Repository Settings > Pages > Build and deployment > Source:
   "Deploy from a branch" > Branch: main, Folder: /(root), Save.
   (Switch from 'GitHub Actions' if it was selected during earlier setup.)
6. Wait for GitHub Pages to build. Open the Pages URL shown in Settings > Pages.
   Typically this will be https://tristanpeto123-eng.github.io/supply-scout/
   but always use the URL shown by GitHub until verified.
7. In Safari on that website: Share > Add to Home Screen.

No running Python or uploading folders. This PWA can open offline once installed.
The fictional demo is included and clearly labelled. The historical casebook
is stored in your Safari browser's local storage and can be exported as JSON.

LIVE DATA IMPORTANT
-------------------
The 'Sync real evidence' button reads the public article archive here:
https://raw.githubusercontent.com/tristanpeto123-eng/supply-scout/main/data/archive.json

This archive can only gain articles when your GitHub Actions news-scanning
workflow succeeds. The latest GitHub Actions run was failing before any jobs
started when this package was built. This PWA does NOT silently fix the GitHub
workflow and does NOT generate or invent live news. It displays a clear error
if the archive does not exist, is empty or cannot be reached.

You can change the public JSON archive URL in Settings. The app accepts a JSON
array of article objects with theme, headline, url, domain, flags, and
first_seen_by_agent_at, or an object with articles or signals arrays.

BEFORE USE
----------
It is a research notebook and archive reader, NOT a predictive machine-learning
agent, not an automatic brokerage bot, and not investment advice. Current
research-priority scores count news and signal keywords, not the probability
of profitable trades. First-seen date != verified original publication date.
Manual casebook data only lives in this browser unless exported. GitHub Pages
is public, so do not upload secrets, personal investment accounts or API keys.
