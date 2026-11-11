# Photo Portfolio

A one-page Hugo portfolio, editable through [Pages CMS](https://app.pagescms.org).

## What's where

| File | What it does | Who edits it |
|---|---|---|
| `content/_index.md` | All the content: name, photos, captions, About text, links | The student, through Pages CMS |
| `static/images/` | Uploaded photos | The student, through Pages CMS |
| `.pages.yml` | Defines the Pages CMS form (which fields appear) | Template author |
| `layouts/index.html` | The page structure (the "theme") | Template author |
| `static/css/style.css` | The look | Template author |
| `.github/workflows/hugo.yml` | Builds and publishes the site on every save | Template author |

## How it works

1. Open this repository in Pages CMS and edit **My portfolio**.
2. Each save is a commit to this repository.
3. The workflow builds the site with Hugo and publishes it to GitHub Pages.

One-time setup for publishing: **Settings → Pages → Source: GitHub Actions**.

## Design notes

- The name stays visible at the top of every screen.
- Mobile first: one column on phones, two or three on wider screens.
- No JavaScript. Clicking a photo opens a full-size view using a plain link.
- Every photo has a caption field, so work is narrated rather than left to speak for itself.
