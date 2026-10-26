# ICRA 2027 Workshop: Explainable Robot Planning

Website for the half-day ICRA 2027 workshop *Explainable Robot Planning: From Task Decisions to Navigation, Motion, and Human Understanding*.

Plain static site (no build step): `index.html`, `css/style.css`, `img/`.

## Publish on GitHub Pages

1. Create an empty repository on GitHub, e.g. `icra2027-explainable-planning` (for a URL like `https://<user>.github.io/icra2027-explainable-planning/`), or `<user>.github.io` for a root URL.
2. Push this folder:
   ```bash
   git remote add origin git@github.com:<user>/<repo>.git
   git push -u origin main
   ```
3. On GitHub: Settings → Pages → Build and deployment → Source: *Deploy from a branch*; Branch: `main`, folder `/ (root)`. Save.
4. The site goes live within a minute or two at the URL shown on that page.

## Editing

- Content lives in `index.html`; each section has an `id` matching the navigation links.
- Important dates: edit the table in `#dates`.
- Submission link: replace the placeholder in the "Submission and selection" card in `#call`.
- Photos: see `img/README.md`.
- Remove the yellow proposal-status notice (`<div class="notice">`) once the workshop is accepted.
- To add accepted papers later, add a section (e.g. `id="papers"`) and a matching nav link.

## Local preview

```bash
python3 -m http.server 8000
```
Then open http://localhost:8000.
