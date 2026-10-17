# Race Split Taker

A stopwatch for timing teams at several distance markers. Drag runners into finish order, take a split as each one crosses, see estimated arrival and finish times, sync phones, save races, and export to Excel. Works offline once installed.

---

## Install it as an offline app

**iPhone / iPad (use Safari)**
- Open your app link in **Safari** while you have signal. Other iPhone browsers can't install it properly.
- Tap **Share** → **Add to Home Screen** → **Add**.
- Open the app **from the new Home Screen icon** once while still online. This saves the files for offline use.
- Test it: turn on airplane mode, close the app, and open the icon again.

**Android (use Chrome)**
- Open your app link in **Chrome** while you have signal.
- Tap the **⋮** menu → **Install app** (or **Add to Home screen**) → **Install**.
- Open it from the new icon once while online, then test it in airplane mode.

**Notes**
- Every phone installs it once, from the same link.
- Don't clear the browser's website data for the site. That deletes the saved copy and your saved races.
- Updates need signal. After a new version is uploaded, open the app twice with signal to switch to it.

---

## Setting up a race

- **Add names** — type a name and tap **Add** (or press Enter).
- **Predicted order** — drag the **☰** handle to put runners in the order you expect them to finish (top = first).
- **Remove a name** — tap the **×** next to it.
- **Markers** — add the points where you'll take splits (for example Mile 1, Mile 2, Finish). Tap a marker chip to remove it. Leave this empty for a single marker; you can add more during the race.
- **Continue** — goes to the Distances screen.
- **Distances (optional)** — choose **Miles** or **Kilometers**, enter the total race distance, and enter how far along each marker is. These are only used for the time estimates. You can skip this.
- **Ready screen** — check the line-up and markers. Tap **Start race** to start the clock, or **← Back to edit** to change anything.

---

## During the race

- **Clock** — runs from when you tap Start race.
- **Take split** — the big button, labelled like "Take split · 1st runner". Tap it each time a runner crosses the marker. On a computer, the spacebar does the same.
- **Put names in order** — drag **☰** on a name to match who actually crossed. Times stay with the place (1st, 2nd, ...), not with the name.
- **Edit a time** — tap an underlined time and type a new one (`1:05.30` or `65.3`).
- **Prediction check** — each runner shows ▲ (finished better than predicted), ▼ (worse), or ✓ (as predicted).
- **Estimates** — once a split is recorded, each runner shows **Arr** (estimated arrival at the marker you're on) and **Fin** (estimated final time). **~** means based on that runner's own average pace. **≈** means the runner has no split yet, so the group average is used. Estimates update with every split and aren't saved between races.
- **Marker tabs** — tap a tab to switch markers. A new marker starts with the previous marker's order, so you only fix what changed.
- **+ Marker** — adds another marker during the race.
- **Rename a marker / set its distance** — use the two boxes under the tabs.
- **Edit runners** — opens a menu where you can:
  - fix a name's spelling (tap the name, type, press Enter)
  - remove a runner with **×** (this also removes their times at every marker)
  - add a new runner, who joins at the bottom of each marker so you can drag them into place
- **Finish race** — stops the clock.

---

## After the race

- **Fix mistakes** — drag names, tap times to edit, and use **Edit runners** the same way as during the race.
- **Add a late runner** — in **Edit runners**, enter the name, choose where they go ("Between Sam and Alex"), and check the estimated time, which is filled from their neighbours and can be edited.
- **Merge duplicates** — in **Edit runners**, under **Merge duplicate runners**, pick the name to keep and the duplicate to merge in, then tap **Merge runners**. Times are combined. If both have a time at a marker, the kept runner's time wins.
- **Export to Excel** — makes an `.xlsx` with bold names, sized columns, and one column of times per marker, in finish order. It opens the phone's share sheet; choose Mail/Outlook (email it to yourself), Save to Files, or another app.
- **Copy table** — copies the same table so you can paste it into Excel or Google Sheets.
- **New race (same names)** — back to setup with your names and markers kept.
- **Start over** — clears the names too.

---

## Sharing between phones

- **Export code** (on the first screen, Ready screen, during a race, and after) — shows a **QR code** and a text code starting with `RST1:`. **Copy code** copies the text.
- **Import code** — on the other phone:
  - **Scan QR with camera**, or
  - **Paste** (or paste by hand) the text code, then tap **Import**.
- **New race** — if the phone has no race, or the code is a different race, it loads the whole race (names, markers, distances, splits) and the clock stays in sync.
- **Same race** — if the phone already has that race, importing only **fills in what's missing** (runners, markers, splits). Nothing already recorded is overwritten, so two phones can time different markers and swap codes to combine.
- Sync happens when you import, not live. Use **Refresh** in the export screen after taking more splits.
- **Scanner note** — scanning needs the `jsQR.js` file in the app folder (see Hosting). Without it, use Paste.

---

## Saving

- **Automatic** — the race saves on the phone after every split and edit. If you close the app mid-race and reopen it, the race comes back and the clock has kept counting.
- **Saved races** (on the first screen) — every finished race is kept, up to 30. For each one you can **Open** it, send it to **Excel**, or **Delete** it (tap twice).
- Saved data lives only on that phone. Export anything important.
