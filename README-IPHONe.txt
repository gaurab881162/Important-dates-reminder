IMPORTANT DATES REMINDER — iPHONE HOME SCREEN VERSION

This is a Progressive Web App (PWA) package. It is not a signed native iOS app.

WHAT'S INCLUDED
- Add/edit/delete birthday, anniversary and other dates
- Yearly recurrence and countdowns
- Search, type filter, JSON backup export/import
- App manifest, icons, and service worker for installability/offline caching

IMPORTANT LIMITATION ABOUT REMINDERS
The app's data stays in browser storage on the device. This version does NOT reliably schedule notifications for future dates while closed. iPhone Safari web apps do not provide a general-purpose local notification scheduler like a native iOS app. For dependable scheduled notifications, we should build the native SwiftUI version with UserNotifications, which requires Xcode on a Mac or cloud Mac; alternatively a hosted web-push backend can be developed with additional setup.

HOW TO MAKE IT INSTALLABLE ON IPHONE
A. Upload these files to an HTTPS static host (for example GitHub Pages or another HTTPS host). Keep the folder structure intact.
B. On your iPhone, open the hosted HTTPS address in Safari.
C. Tap Share -> Add to Home Screen -> Add.
D. Open it from the new Home Screen icon. Add a test date and use Export backup periodically.
E. The app can cache its files for later opening, but initial install requires internet.

HOW TO HOST WITH GITHUB PAGES (WINDOWS)
1. Sign in or create a GitHub account.
2. Create a new public repository, e.g. important-dates-reminder.
3. Upload index.html, manifest.webmanifest, service-worker.js, and the icons folder (not just the ZIP).
4. In repository Settings -> Pages, select deploy from the main branch and root folder; save.
5. Wait until GitHub Pages provides an HTTPS website URL.
6. Open that URL in Safari on iPhone and follow steps B-D above.

DATA / PRIVACY
Entries are saved to local browser storage; they do not sync between devices. Clearing Safari website data can remove entries. Export a backup before changing devices or clearing browser data.
