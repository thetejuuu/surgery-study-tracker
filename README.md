# Surgery Revision Tracker

A lightweight, installable static web app for tracking 59 surgery topics.

## Features
- Taught-in-class and personally-read checkboxes
- All topics start unchecked (0% progress)
- Progress saved locally in each student's own browser using localStorage
- Search, specialty filter, and progress filters
- JSON export/import backup
- Reset progress
- Offline support through a service worker / PWA manifest

## Deploy to Vercel
1. Extract this ZIP.
2. Upload the **contents** of this folder to the root of your GitHub repository (`index.html`, `manifest.webmanifest`, `sw.js`, `README.md`).
3. In Vercel, open the existing `surgery-revision-tracker` project.
4. Go to **Settings → Git** and connect `thetejuuu/surgery-study-tracker` (if it is not already connected).
5. Ensure Production Branch is `main`.
6. Framework Preset: **Other**; Build Command: leave blank; Output Directory: leave blank / default (project root).
7. Save. Push/commit the files to `main`; Vercel will build and deploy automatically.

## Important: individual progress
Progress is stored only in localStorage on the browser/device being used. It is not shared or synced between classmates. Different students should use their own browser profile/device. Clearing browser data removes local progress, so use Export backup periodically.

## Clean starting state
The initial taught and read arrays are both empty. No class topics are pre-marked.
