GYMLOG v1.0 — PERSONAL OFFLINE WORKOUT TRACKER

WHAT'S INCLUDED
- Mobile-first responsive workout tracker
- Your October 5-day split: Monday Upper A, Tuesday Lower A, Thursday Push, Friday Pull, Saturday Lower B
- Log weight, reps, set completion and optional RIR
- See the previous saved performance for each exercise
- Edit/add exercises and rep targets
- Workout history and body measurements
- JSON export and restore
- Weekly backup reminder while the app is open
- IndexedDB local storage; no account, analytics, cloud database or external libraries

IMPORTANT DATA / DEVICE NOTES
- Data is stored in the browser's local IndexedDB on the device where the app is used.
- Android and laptop data are separate. This build does not sync devices.
- Export a JSON backup regularly. Browser storage can be cleared by device/browser cleanup, uninstall or reset.
- The backup reminder is checked when the app is opened; browsers do not guarantee background reminders for a local PWA.

HOW TO RUN / INSTALL ON ANDROID
A PWA needs to be served from HTTPS (or localhost) to install and cache offline. The app itself uses no cloud database; static hosting only serves the app files.
1. Put index.html, manifest.webmanifest and sw.js on a static HTTPS host you control (for example, a static site host).
2. Open the HTTPS site in Chrome on Android.
3. Open Chrome menu > Add to Home screen / Install app.
4. Open GYMLOG from the home-screen icon.
5. Log workouts. Use Data & backup > Export backup regularly.

LAPTOP
Open the same HTTPS site in Chrome/Edge and use it there. It will have its own local database. Export/import JSON to transfer records manually.

DEVELOPMENT
The source is plain HTML/CSS/JavaScript. To modify, edit index.html and update the service-worker cache name in sw.js (e.g. gymlog-v1.1) so devices fetch the new files.
