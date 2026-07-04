# Personal Website — Dr. Carlos Manuel Herrera Castillo

Academic website built with [Quarto](https://quarto.org), based on the Flatly theme.

## Site Structure

| File | Page |
|---|---|
| `index.qmd` | About / Home (bio, education, contact) |
| `research.qmd` | Research experience & technical skills |
| `publications.qmd` | Peer-reviewed articles & expected publications |
| `teaching.qmd` | Teaching, conferences, awards & memberships |
| `styles.css` | Custom CSS overrides |
| `_quarto.yml` | Site configuration (navbar, theme, footer) |
| `CV_CMHC.pdf` | CV linked from the navbar |

Extensions used: [`quarto-ext/fontawesome`](https://github.com/quarto-ext/fontawesome), [`schochastics/academicons`](https://github.com/schochastics/academicons).

## Setup

Requires [Quarto CLI](https://quarto.org/docs/get-started/) ≥ 1.5.

```bash
# Preview locally with live reload
quarto preview

# Build static site to _site/
quarto render
```

## Profile Photo

Add a headshot named `profile.jpg` to the project root. It is displayed on the About page using the `trestles` layout.

## Deployment

The rendered site is output to `_site/`. To deploy to GitHub Pages:

1. Push the repository to GitHub.
2. Run `quarto publish gh-pages` and follow the prompts.
3. The site will be published to `https://<username>.github.io/<repo>`.

Alternatively, connect the repository to [Netlify](https://www.netlify.com) and set the build command to `quarto render` with publish directory `_site`.
