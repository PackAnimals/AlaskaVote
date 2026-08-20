# Alaska Votes

GitHub-ready PWA test build for Alaska's 2026 elections.

## What's included

- Selectable race menu
- U.S. Senate
- U.S. House
- Governor
- All 10 State Senate districts on the 2026 ballot
- All 40 State House districts
- Alaska ballot measures
- Senate candidate issue comparison
- Where Do I Stand? matcher
- Congressional voting records
- Money Trail and donor explorer
- Polling, endorsements and campaign tracker
- Mobile bottom navigation
- Installable PWA files

## GitHub Pages setup

1. Create or open your `alaska-votes` repository.
2. Replace the existing files with the contents of this package.
3. Keep the folder named exactly `.github`.
4. Commit to `main`.
5. Go to **Settings → Pages**.
6. Under **Build and deployment**, choose **GitHub Actions**.
7. The included workflow will deploy the static site.

If GitHub's browser uploader won't accept `.github`, create the workflow directly in GitHub using **Add file → Create new file** and name it:

`.github/workflows/pages.yml`

Then paste the contents of the provided `pages.yml`.

## Test on iPhone

Open the published GitHub Pages URL in Safari → Share → **Add to Home Screen**.

## Test locally

From this folder:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

## Important

This remains a test snapshot. Rapidly changing election data should eventually move into a live backend and all substantive public-facing claims should carry primary-source citations.
