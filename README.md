# Race Split Tracker

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
- Updates need signal. After a new version is uploaded, open the app with signal, close it fully (swipe it away), and open it again.

---

## Organizer or Helper

- The first screen has an **Organizer | Helper** toggle at the top.
- **Organizer** — runs the race: names, markers, distances, the clock, results, Excel export. Only the Organizer tab shows the race setup.
- **Helper** — times splits at one or more markers for an organizer, without needing the race clock. See *Helpers* below.
- Switching tabs is only possible from the first screen, not in the middle of a race or helper session.

---

## Setting up a race (Organizer)

- **Add names** — type a name and tap **Add** (or press Enter).
- **Predicted order** — drag the **☰** handle to put runners in the order you expect them to finish (top = first).
- **Remove a name** — tap the **×** next to it.
- **Team presets** — tap **Team presets** to save the current names as a named team, or load a saved team. Loading replaces the current names; then just drag them into your predicted order. Saving under an existing team name updates it. Delete a team by tapping Delete twice.
- **Markers** — enter the distance of each split point and choose **mi** or **km** for that marker, then tap **Add**. Markers are named automatically from the distance (for example "1 mi" or "1 km") and sorted by distance, so you can mix miles and kilometers in one race. Tap a marker chip to remove it. Leave this empty for a single marker; you can add more during the race.
- **Continue** — goes to the Distances screen.
- **Total distance (optional)** — choose **Miles** or **Kilometers** and enter the total race distance. It's only used for the finish estimates (the app converts between miles and kilometers for you). You can skip this.
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
- **Change a marker's distance or unit** — use the boxes under the tabs. The marker's name updates automatically.
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

## Helpers (timing without the race clock)

**Organizer**
- Finish the names, markers and distances first, then tap **Invite helpers (QR)** (on the Ready screen or during the race).
- Helpers scan the QR. Hold the screen steady; the code changes every second so each helper's phone can match your clock.
- You must press **Start race** on your phone so the app has a start time. Helpers can send results before or after.
- When a helper shows their results QR, tap **Import code → Scan QR with camera**. The splits fill in automatically, using each tap's exact time. A message tells you how well the clocks matched.
- Results are **fill-in only**: they never overwrite times you already have. If two helpers time the same marker, the first one imported wins for each runner.

**Helper**
- Open the app, choose the **Helper** tab, and tap **Scan organizer's QR**.
- **Pick your markers** — choose one or more. You can switch between them while timing.
- **Take split** — tap it each time a runner passes. Each tap saves the exact time privately; the clock time isn't shown. A **✓** appears next to the place number instead, and every runner after the leader shows how far **behind 1st** they were (the leader shows "Leader").
- **Drag ☰** to put the names in the order the runners came by. Times stay with the place (1st, 2nd, ...).
- **Undo last** removes the most recent tap. To delete a mistaken tap in the middle, tap its ✓ and choose **Delete** (later splits move up one place).
- **Send to organizer** shows a results QR. The organizer scans it. You can send again after taking more splits.
- **Change markers** adds or drops markers; **End session** clears this phone's helper times (tap twice).
- Helper sessions are saved on the phone, so closing the app doesn't lose your taps.

**Clock matching**
- Scanning matches clocks both ways: the helper's phone compares its clock when it scans the invite, and the organizer's phone compares again when it scans the results. Averaging the two cancels most of the delay. In testing the math this lands within about a tenth of a second, but real cameras vary, so treat helper times as accurate to roughly a fraction of a second.
- **Pasted text codes can't match clocks.** If you paste instead of scanning, the app assumes the phones agree. Keep phones on automatic date & time.
- If the organizer changes names or markers after inviting helpers, invite them again.

---

## Saving

- **Automatic** — the race saves on the phone after every split and edit.
- **Resume prompt** — if you close the app in the middle of a race, reopening it asks **Resume last race?** It shows how many runners and splits were recorded and what the clock would read now (the clock keeps counting while the app is closed). Tap **Resume race** to carry on, or **Discard race** (tap twice) to start over with your names and markers kept. Finished races and unfinished setups reopen on their own without asking.
- **Saved races** (on the first screen) — every finished race is kept, up to 30. For each one you can **Open** it, send it to **Excel**, or **Delete** it (tap twice).
- Saved data lives only on that phone. Export anything important.
