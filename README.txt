RACE SPLIT TAKER - OFFLINE VERSION
==================================

FILES (keep them all together in one folder)
  index.html, qrgen.js, sw.js, manifest.webmanifest,
  icon-192.png, icon-512.png, apple-touch-icon.png
  jsQR.js   <- you add this one (see "QR scanner" below)

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
   Showing a QR code works as-is. Scanning needs the jsQR library, which could
   not be downloaded when this package was built. Add it once:
   - Download https://cdn.jsdelivr.net/npm/jsqr@1.4.0/dist/jsQR.js
   - Save it as jsQR.js in the same folder, then upload the folder again.
   Without it, Import still works by pasting the code.

UPDATING: change sw.js's CACHE name (currently rst-v2 -> rst-v3) when you replace files
so phones pick up the new version.

NEW IN THIS VERSION
  - Races save automatically on the phone. Reopening the app restores the
    current race (a running clock keeps counting while the app is closed).
  - Finished races are kept under "Saved races" on the first screen
    (up to 30). Open one to review it again or export it.
  - "Export to Excel" after a race makes an .xlsx with bold names and sized
    columns: one row per runner, one column of times per marker.
    "Copy table" copies the same table to paste into Excel/Sheets.
