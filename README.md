# Alaska Votes

Mobile-first, installable PWA for researching Alaska's 2026 U.S. Senate race.

## Fastest way to test with GitHub Pages

1. Create a new GitHub repository named `alaska-votes`.
2. Upload **all files and folders** from this package to the repository root.
3. Commit them to the `main` branch.
4. In GitHub, open **Settings → Pages**.
5. Under **Build and deployment → Source**, choose **GitHub Actions**.
6. Open the **Actions** tab. The included `Deploy to GitHub Pages` workflow will publish the site.
7. When deployment finishes, GitHub will show the public URL.

Typical URL:

`https://YOUR-GITHUB-USERNAME.github.io/alaska-votes/`

## Test on iPhone

1. Open the GitHub Pages URL in Safari.
2. Tap **Share**.
3. Tap **Add to Home Screen**.
4. Launch **Alaska Votes** from the new icon.

The PWA uses standalone display mode and includes a basic service worker for offline caching.

## Test on Android

Open the site in Chrome and choose **Install app** or **Add to Home screen**.

## Vercel alternative

Import the GitHub repository at Vercel. This is a static site; no build command is required. Vercel will redeploy automatically whenever `main` changes.

## Files

- `index.html` — current Alaska Votes application
- `manifest.webmanifest` — PWA metadata
- `service-worker.js` — offline/app caching
- `icons/` — install icons
- `.github/workflows/pages.yml` — automatic GitHub Pages deployment
- `vercel.json` — optional Vercel configuration

## Current limitations

This is a test build. Election data is currently embedded in the front-end snapshot rather than loaded from a live database/API. Before public launch, add primary-source citations to every substantive policy/voting-record claim and move rapidly changing election, polling, and campaign-finance data into a maintained data layer.

## Recommended next architecture

For production:

- Front end: this PWA, later optionally refactored to React/Vite
- Database/API: Supabase/Postgres
- Federal campaign finance: FEC data
- Congressional votes: official House/Senate/Congress.gov sources
- Alaska election results: Alaska Division of Elections
- Native packaging: Capacitor for iOS + Android

## Local testing

Because service workers require HTTP/HTTPS rather than `file://`, run a tiny local web server from the repo directory:

```bash
python -m http.server 8080
```

Then open:

`http://localhost:8080`

