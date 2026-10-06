# esharuhulla.github.io — what lives where

Last updated 7 October 2026.

## Read this first

There are **two copies of the site in this folder**, and only one of them is live.

### `UPLOAD-THESE/` — this is the live site

Flat HTML. No folders, no build step. **This is what you upload to GitHub.**

Go to <https://github.com/esharuhulla/esharuhulla.github.io> → **Add file** →
**Upload files** → drag in everything inside `UPLOAD-THESE/` → **Commit changes**.
The site rebuilds in about a minute at <https://esharuhulla.github.io>.

Files in it:

| File | What it is |
|---|---|
| `index.html` | About page |
| `research.html` | Thesis write-up |
| `projects.html` | PLAXIS work and analysis code |
| `publications.html` | ICCE 2026 abstract |
| `cv.html` | Short CV |
| `404.html` | Not-found page |
| `style.css` | All the styling |
| `CV.pdf` | The LaTeX CV, downloadable from every page |
| `profile.jpg` | Your photo |
| `thesis-troughs.png` | Three-way comparison, measured vs elastic vs FEM |
| `thesis-correction.png` | Width correction, R² 0.41 → 0.91 |
| `thesis-pinn.png` | PINN vs analytical, DLR Lewisham |
| `plaxis-pile.png`, `plaxis-raft.png` | FYDP displacement fields |

### The `.md` / `.yml` files at the root — Jekyll source, not currently used

`index.md`, `research.md`, `cv.md`, `_config.yml`, `_data/`, `_layouts/`, `assets/`,
`files/`. These are kept in sync with the live pages, but **nothing here is deployed**.
They exist so that if you ever switch the repo over to Jekyll, the content is ready.
Until then, ignore them — and never upload them instead of `UPLOAD-THESE/`.

## To change something

Edit the file in `UPLOAD-THESE/`, then re-upload that one file. Replacing a file with the
same name overwrites it.

Adding a project means copying one `<div class="entry">` block in `projects.html` and
editing the text inside. Same for a publication.

## What's on the site right now

- 2026 graduate, CGPA 3.40 / 4.00 over 181 credits
- Thesis: forward prediction of tunnelling-induced settlement — peak within 12%, trough
  1.6–2.1× too wide, width correction lifts mean R² from 0.41 to 0.91, PINN matches the
  analytical solution to 0.77%
- FYDP: PLAXIS 3D pile (1879.85 kN, 21.9 mm) and raft (2517.30 kN, 117.8 mm)
- DOHWA Engineering industrial training, October 2025

## Still to check

- **The ICCE 2026 author line** on `publications.html` reads "Abdullah Mahmud, Md. Esha
  Ruhulla". Confirm it matches the submitted version.
- **The status** still says *under review*. If it has been accepted, change
  `<span class="tag">Under review</span>` to `Accepted` in `publications.html`.
