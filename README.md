# Shaan Kirana Store Web App

Mobile-first, installable PWA for customer ledger management.

## Features
- Add and edit customers (name, phone, optional note)
- Debit (udhaar/samaan) and credit (payment) entries
- Automatic remaining due / advance calculation
- Customer transaction history
- WhatsApp pre-filled updates after every entry and statement summary
- Search, CSV export, JSON backup and restore
- Local browser storage and basic offline shell cache

## Run locally
Open `index.html` in a browser. Some PWA features require HTTPS, so deploy to GitHub Pages to install it from Chrome.

## Publish using GitHub Pages (mobile steps)
1. Upload the contents of this folder to the root of your `shaan_kirana_store` GitHub repository (not the ZIP itself).
2. In repository Settings → Pages, set source to `Deploy from a branch`, branch `main`, folder `/(root)`, then Save.
3. Wait for the Pages URL shown there, usually `https://YOUR-USERNAME.github.io/shaan_kirana_store/`.
4. Open the URL in Android Chrome. Use Chrome ⋮ → `Add to Home screen` or `Install app`.

## Important limitations
- Customer data is stored in that browser on that device. Clearing browser data or changing device can remove access; use Backup Data regularly and store the JSON somewhere safe.
- This is a local single-device ledger, not multi-user cloud sync.
- WhatsApp opens a pre-filled message using `wa.me`; the user must press Send. Fully automatic WhatsApp messages require a secure backend, Meta Cloud API credentials, approved template and compliant messaging setup.
- Not a replacement for formal accounting; verify balances and keep backups.
