# Yiran Hu — Personal Homepage

Live site: https://zimablue307.github.io (GitHub Pages, published from the root of the `main` branch)

| File | Contents |
|---|---|
| `index.html` | Page content (bio, publications, experience, education, honors) |
| `style.css` | Styles (dark mode and mobile layout included) |
| `assets/avatar.jpg` | Profile photo |
| `assets/CV-Yiran-Hu.pdf` | Downloadable CV (2-page version) |

Plain static site — no build step.

## Preview locally

Open `index.html` in a browser, or start a local server:

```bash
cd /home/huyiran/career-plan/homepage
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Update the CV

Compile the 2-page CV in the CV repo first, then copy it over. Keep the file name unchanged so the download link keeps working:

```bash
cp /home/huyiran/career-plan/docs/CV/build/CV-2page.pdf /home/huyiran/career-plan/homepage/assets/CV-Yiran-Hu.pdf
```

## Commit and publish

```bash
cd /home/huyiran/career-plan/homepage
git add -A
git commit -m "Update homepage"
git push
```

The site updates 1–2 minutes after the push; deployment progress is shown on the repository's Actions tab.

## Where to edit (`index.html`)

- **Publications**: `<section id="pubs">`, one `<li>` per paper
- **Experience / Education / Honors**: `id="experience"` / `id="education"` / `id="honors"`
- **"Last updated" date**: the `<footer>` at the end of the file
