# Robin S. Högnäs — personal academic website

A plain HTML/CSS site. No build step, no JavaScript.

| File | Page |
|---|---|
| `index.html` | Home / academic profile |
| `research.html` | Research themes, grants, publications, presentations |
| `teaching.html` | Courses, supervision, mentoring |
| `future.html` | Future plans (placeholders to fill in) |
| `fun.html` | Fun things about me (placeholders to fill in) |
| `css/style.css` | Shared styles (colors are set at the top of the file) |
| `images/robin.png` | Profile photo |
| `cv.pdf` | CV linked from the menu |

## Editing
- Open any `.html` file in a text editor. Yellow dashed boxes (`<div class="placeholder">…</div>`) are placeholders: replace the whole `<div>` with your own `<p>…</p>` paragraphs.
- The menu and footer are repeated at the top and bottom of every page; if you change them, change them on all five pages.
- New CV: replace `cv.pdf` (keep the same name).
- Better photo: the current photo is small (87×115 px). Save a larger square-ish portrait as `images/robin.png` (or change the `src` in `index.html`).

## Preview locally
Double-click `index.html`, or run `python3 -m http.server` in this folder and open http://localhost:8000.

## Publish on GitHub Pages
1. Create a GitHub repository. Naming it `<your-username>.github.io` gives you the address `https://<your-username>.github.io`; any other name gives `https://<your-username>.github.io/<repo-name>`.
2. In this folder:
   ```
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Build and deployment → Deploy from a branch**, choose `main` and `/ (root)`, then Save. The site is live within a minute or two.
4. After later edits: `git add -A && git commit -m "Update site" && git push`.
