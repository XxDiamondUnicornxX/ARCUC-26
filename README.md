# American Red Cross at UChicago — Website

A static website (plain HTML, CSS and JavaScript, with no build step) for the American Red Cross club at the University of Chicago.

## Pages

| File | Page |
| --- | --- |
| `index.html` | Home: hero, mission, ways to get involved, our story, photo gallery, join |
| `board.html` | Meet the Board |
| `mentoring.html` | Pre-Med Mentoring & Families |
| `service.html` | Community Service, Blood Drives, Sound the Alarm |

Styles live in `assets/css/styles.css`, and colors are defined at the top of that file. Photos live in `assets/img/`.

## Preview locally

Open `index.html` in a browser, or run a local server:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Publish (GitHub Pages, free)

1. Merge this code into the `main` branch.
2. On GitHub, go to **Settings → Pages**. Under **Build and deployment → Source**, choose **GitHub Actions**.
3. Every push to `main` now deploys automatically through `.github/workflows/deploy.yml`.
   The site will be at `https://<github-username>.github.io/<repo-name>/`.
4. Optional: to use a custom domain, add it under **Settings → Pages → Custom domain**.

## Things to fill in

Search the HTML for `TODO` to find placeholders:

- **Sign-up form link and club email**: the Join section of `index.html`, plus the footer on every page
- **Instagram link**: the footer on every page
- **Board members**: names, roles, class years and headshots in `board.html` (instructions are in a comment at the top of the grid)
- **Mentee and mentor form links**: `mentoring.html`
- **Next blood drive date, time and location**: `service.html`

The header and footer are copied into each page. If you change a nav link or footer link, update it in all four HTML files.

## Branding note

The Red Cross emblem is legally protected. This site uses a text wordmark instead of the emblem. To add the official club logo, get it through your Red Cross Club resources and follow the American Red Cross brand guidelines.
