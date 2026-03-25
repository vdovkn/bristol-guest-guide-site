# Bristol Guest Guide Site

Static one-page guest guide for **8 Cornwallis Avenue, Bristol**.

## Files

- `index.html` contains all of the editable guest-guide content.
- `styles.css` contains the layout, colors, responsive styles, and print stylesheet.
- `script.js` adds copy-to-clipboard buttons and highlights the current nav section.
- `assets/images/` contains the Bristol illustrations and Wi-Fi QR image pulled from the source guide.
- `.nojekyll` makes sure GitHub Pages serves the site as plain static files.

## How to update content later

1. Open `index.html`.
2. Edit the visible text directly in the relevant section.
3. To change a link, update the `href` on the matching button or text link.
4. To swap an image, replace the file in `assets/images/` and keep the filename the same, or update the `src` in `index.html`.
5. Refresh the page in a browser to check the result.

## GitHub Pages deployment

This project is set up as a plain static site, so it can be deployed directly from the repository root with GitHub Pages.

1. Push the `bristol-guest-guide-site` folder to a GitHub repository.
2. If this folder will be the whole repository, keep these files at the repo root.
3. Push the repository to GitHub on the `main` branch.
4. In GitHub, go to `Settings` -> `Pages`.
5. Under `Source`, select `Deploy from a branch`.
6. Choose the `main` branch and the `/ (root)` folder.
7. Save, then wait a minute or two for the site to publish.

## Suggested first commit

If you want this folder to become its own repository, a clean starting point is:

```bash
git init
git add .
git commit -m "Create Bristol guest guide site"
```

## Notes

- The page intentionally excludes key safe codes, alarm codes, and other security-sensitive access details.
- `robots.txt` plus the page-level `noindex` meta tag help discourage indexing, though no public page can be treated as private.
- There is a print stylesheet included in `styles.css`.
