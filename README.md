# Alaska Votes v0.3

GitHub-ready PWA test build.

## New in this build
- Landing dashboard with contest summary cards
- “Choose Your Contest” selector
- U.S. Senate, U.S. House, Governor, State Senate, State House and Ballot Measures
- All 40 State House districts and 10 State Senate districts on the 2026 ballot
- Money Trail promoted in navigation
- Where Do I Stand? matcher
- Congressional voting records
- Mobile navigation
- Installable PWA

## GitHub Pages
1. Upload all files to the root of your repository.
2. Keep `.github/workflows/pages.yml` exactly under the `.github` folder.
3. Go to Settings → Pages.
4. Choose GitHub Actions as the source.
5. Commit/push to `main`.

If the browser uploader refuses `.github`, create the file inside GitHub using:
`.github/workflows/pages.yml`

## iPhone testing
Open the Pages URL in Safari → Share → Add to Home Screen.

## Local testing
```bash
python -m http.server 8080
```
Then open `http://localhost:8080`.
