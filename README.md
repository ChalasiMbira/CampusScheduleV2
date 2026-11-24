# CampusSchedule

A mobile-first, offline-capable timetable Progressive Web App built with plain HTML, CSS and JavaScript.

## Run locally

Open `index.html` for a quick visual preview. For service-worker and install testing, serve this folder over localhost or HTTPS (for example, `python -m http.server 8000`) and open `http://localhost:8000`.

## Deploy with GitHub Pages

1. Create a GitHub repository named `campusschedule` (or another name).
2. Upload the contents of this folder to the repository root.
3. In repository Settings → Pages, choose **GitHub Actions** as the build/deployment source.
4. The included workflow deploys the static site after each push to `main`.

If the repository is a project site, the relative asset paths and PWA scope are configured to work from the repository subpath.

## Sample groups

- `IT-23-3`
- `CS-22-1`
- `EN-24-2`

All timetable entries are fictional sample data for testing only. They are not official or institution-approved. Each sample group has six classes on Monday, five on Tuesday, five on Wednesday, six on Thursday, five on Friday, two on Saturday and none on Sunday.

## Current features

- Group selection and local persistence on the device
- Weekly day strip and previous/next week controls
- Scrollable class cards with time, subject, lecturer and room
- Swipe left/right to move between days
- Online/offline indicator
- Service-worker app-shell caching for repeat/offline visits
- PWA manifest and install prompt
- Student feedback and petition form UI

## Important before public launch

- Replace sample timetable data with institution-approved data.
- The feedback form currently uses FormSubmit. Its destination address is visible in client-side JavaScript, and the first submission may require email activation. Do not collect sensitive information. For production, move submissions to a controlled backend with a privacy notice, retention policy, spam protection and access controls.
- Test install and offline behaviour on Android Chrome and iOS Safari.
- Add automated accessibility, browser and data-validation tests.

No student number, ID number, password or sensitive personal information should be requested.
