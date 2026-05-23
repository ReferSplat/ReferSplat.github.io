# ReferSplat Project Page

Project page for **ReferSplat: Referring Segmentation in 3D Gaussian Splatting** (ICML 2025 Oral).

- Paper: https://arxiv.org/abs/2508.08252
- Code: https://github.com/heshuting555/ReferSplat

Template adapted from [LangSplat](https://langsplat.github.io/) / [Nerfies](https://github.com/nerfies/nerfies.github.io).

## Layout

```
index.html
static/
  css/   bulma + carousel + slider + fontawesome + index.css
  js/    bulma carousel/slider + fontawesome + index.js
  images/  teaser.png, logo.svg     (drop method/result figures here)
  videos/  (drop demo .mp4 files here)
```

## Where to drop your own content

Open `index.html` and look for the commented blocks marked with `Placeholder` — those are ready to host a method/architecture figure and qualitative result figures/videos. Uncomment the block and replace the `src=` path.

Anything else you'd likely want to tweak:

| What | Line(s) in `index.html` |
|---|---|
| Author names / affiliations / homepage links | `<section class="hero">` block near the top |
| arXiv / PDF / code / dataset links | `publication-links` block |
| Abstract text | `<h2 class="title is-3">Abstract</h2>` block |
| Sections (Task / Method / Dataset / Results) | second `<section class="section">` after the abstract |
| BibTeX | `<section id="BibTeX">` near the bottom |

## Preview locally

```bash
cd /Users/shuaige/code/refersplat_website
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy to GitHub Pages

Two common options:

**Option A — dedicated `refersplat.github.io` org/user repo.** Anything pushed to `main` is served at the root.

```bash
git init
git add .
git commit -m "Initial ReferSplat project page"
git branch -M main
git remote add origin git@github.com:<org-or-user>/refersplat.github.io.git
git push -u origin main
```

Page will be live at `https://<org-or-user>.github.io/` within ~1 minute.

**Option B — project page under the existing code repo.** Push this directory to a `gh-pages` branch of `heshuting555/ReferSplat`:

```bash
git init
git checkout -b gh-pages
git add .
git commit -m "Project page"
git remote add origin git@github.com:heshuting555/ReferSplat.git
git push -u origin gh-pages
```

Then enable GitHub Pages on the `gh-pages` branch in the repo settings. URL will be `https://heshuting555.github.io/ReferSplat/`.
