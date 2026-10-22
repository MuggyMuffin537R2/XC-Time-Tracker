RACE SPLIT TRACKER - OFFLINE VERSION
==================================

FILES (keep them all together in one folder)
  index.html, qrgen.js, sw.js, manifest.webmanifest,
  THIRD-PARTY-LICENSES.txt,
  icon-192.png, icon-512.png, apple-touch-icon.png
  jsQR.js

1) HOST IT (needs internet once)
   Upload the whole folder to any free HTTPS host, e.g.
   - Netlify Drop (app.netlify.com/drop): drag the folder onto the page
   - GitHub Pages or Cloudflare Pages
   It must be https:// for offline mode and the camera to work.

2) INSTALL ON EACH iPHONE
   Open the link in Safari while online -> Share -> Add to Home Screen.
   Open it once from the new icon while still online so it can save itself.
   After that it works with no signal.

3) QR SCANNER
   jsQR.js is already included in this folder, so scanning works as-is.
   Keep jsQR.js in the same folder as index.html. Without it, Import still
   works by pasting the code.

UPDATING: change sw.js's CACHE name (currently rst-v11 -> rst-v12) when you replace files
so phones pick up the new version.

NEW IN THIS VERSION
  - Races save automatically on the phone. Reopening the app restores the
    current race (a running clock keeps counting while the app is closed).
  - Finished races are kept under "Saved races" on the first screen
    (up to 30). Open one to review it again or export it.
  - "Export to Excel" after a race makes an .xlsx with bold names and sized
    columns: one row per runner, one column of times per marker.
    "Copy table" copies the same table to paste into Excel/Sheets.

THIRD-PARTY LICENSES
  jsQR (jsQR.js) - Cosmo Wolfe and contributors - Apache License 2.0
  QRCode for JavaScript (qrgen.js) - Kazuhiko Arase - MIT License
  Full texts are in THIRD-PARTY-LICENSES.txt. Keep that file (and the notice
  comments at the top of jsQR.js and qrgen.js) with the app when you host it.
  The app also shows these credits: tap "Credits & licenses" at the bottom of
  the first screen.
