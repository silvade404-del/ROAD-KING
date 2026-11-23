# ROAD KING - Tuk Tuk Diary PWA
Offline PWA for tuk-tuk drivers. Sinhala. Blue only.

## Files
- index.html - Full app (Home + all pages + Lock + Key System + Monthly Report)
- manifest.webmanifest - PWA install info
- sw.js - Service Worker for offline
- icons/ - Add icon-192.png and icon-512.png (blue ROAD KING logo)

## Key System
Format: RDK-PPPP-MMMM-DU-CCCC
CCCC = (PPPP x 7 + MMMM x 13 + D x 29 + 4317) % 10000
Secret = 4317 (do NOT show in UI)
1M = expires in 1 month, 1Y = expires in 1 year. Auto Deactivate on expiry.
One Key = One Phone.

## Daily Rule
Daily pages show ONLY today. Old entries move to Monthly Report by date.
Monthly Report has "සම්පූර්ණ මාසය" button - full month table: දිනය | ආදායම | වියදම | ඉතුරුව | පෙට්‍රල් + monthly totals.

## Deploy to GitHub Pages
1. Create repo, upload all files to main branch
2. Settings > Pages > Source: Deploy from branch, Branch: main, Folder: / (root)
3. Open https://<username>.github.io/<repo>/
