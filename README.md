# Alaska Votes v0.6

GitHub-ready PWA test build.

## Included in this build
- Political spectrum now follows the selected contest
- Contest-specific candidate syncing
- Contest-specific primary summary
- Balanced Senate fundraising comparison
- Money Trail scoped to selected contest
- Donor Explorer scoped to selected contest
- Compare menus scoped to selected contest
- Statewide races, legislative districts and ballot measures
- Where Do I Stand? matcher
- Mobile PWA shell

## GitHub Pages
1. Replace your current repo files with this package.
2. Keep `.github/workflows/pages.yml` under the `.github` folder.
3. Commit to `main`.
4. GitHub Pages should redeploy automatically.

If the browser uploader refuses `.github`, create `.github/workflows/pages.yml` manually in GitHub.

## iPhone testing
Open the Pages URL in Safari → Share → Add to Home Screen.

## Local testing
```bash
python -m http.server 8080
```
Then open `http://localhost:8080`.
