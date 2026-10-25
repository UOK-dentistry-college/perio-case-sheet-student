# Perio Case Sheet — Student App

A digital version of the **periodontal case sheet** used by 4th-year students at the **College of Dentistry, University of Karbala**. Fill the sheet on your phone, let your supervisor time and score the case, and keep everything as a signed record. No paper, no account, no internet needed after the first load.

> Works together with the **Perio Supervisor** app (the doctor's side).

**Open the app:** [`https://UOK-dentistry-college.github.io/perio-case-sheet-student/`](https://UOK-dentistry-college.github.io/perio-case-sheet-student/)

---

## Install it on your phone (works offline afterwards)

**iPhone / iPad (Safari only)**
1. Open the link above in **Safari**.
2. Tap **Share** → **Add to Home Screen** → **Add**.
3. Always open the app from the **home-screen icon**, not from Safari.

> **iPhone note:** Safari and the home-screen icon keep their data separately. Install first, **then** enter your cases. Anything entered in a Safari tab will not appear in the installed app.

**Android (Chrome)**
1. Open the link in Chrome.
2. Tap the menu **⋮** → **Install app** (or **Add to Home screen**).
or
**Android (the app)**
1. Go to [`realeses`](https://github.com/UOK-dentistry-college/perio-case-sheet-student/releases), and download the lataest APK version.
2. after the download is completed open the APK file and install it.

**Computer (the app)**
1. Go to [`realeses`](https://github.com/UOK-dentistry-college/perio-case-sheet-student/releases), and download the lataest EXE version.
2. after the download is completed open the EXE file and install it.
---

## How a case works

1. **Set your name and group** once. They are saved on the device and pre-filled for every new case.
2. **Fill the case sheet** (patient details, chief complaint, medical history, habits, examination, BOP chart, bone loss, diagnosis, calculus index, infection control and behavior). Required fields are checked before you can continue.
3. **Show the Start QR** to your supervisor. They scan it with the Supervisor app and start the timer.
4. When the supervisor finishes grading, they show you a **score QR**. Tap **Scan score**, check it, then **Apply score**.
5. The app **verifies the doctor's signature**. A score that was changed, or that belongs to another case, is rejected.
6. **Save** the case. It appears in your history.

## History, bundles and backup

- **Cases** tab: search by patient or student, **Filters** (dates are picked from a calendar, and you can filter by the **doctor who graded** the case), **Sort by**, and **Select** several cases at once.
- **Bundles**: group cases (for example by day or by group) and open them together.
- **Export PDF** of a case sheet.
- **Backup** saves your cases to a file; **Import** restores it. Make a backup regularly. Your data lives only on your phone.

---

## Privacy and responsibility

- Everything is stored **only on your device**. Nothing is uploaded.
- Case sheets contain **patient information**. Keep your phone locked, and share backups and PDFs only with people allowed to see them.
- If you clear your browser data or delete the app, the cases are lost unless you made a backup.
- This is a training and documentation tool for the college. It is **not** a certified medical record system.

## For developers

The app is a single static `index.html` with every library inlined. Files:

| File | Purpose |
|---|---|
| `index.html` | The whole app |
| `manifest.json` | Install name, icons, colors |
| `sw.js` | Offline cache. Change `VERSION` each time you upload a new `index.html` |
| `icons/` | App icons |

**Host on GitHub Pages:** push these files to the repository root → *Settings → Pages → Deploy from a branch → `main` / `(root)`*. HTTPS is required for the camera and for installing, and GitHub Pages provides it.

## License

MIT License. © 2026 Karrar Abdul Manaf Asker and the College of Dentistry, University of Karbala. See [`LICENSE`](LICENSE).
