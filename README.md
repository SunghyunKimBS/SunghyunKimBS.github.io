# Personal Academic Homepage

Built on the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme.

## What's here (skeleton — fill in the TODOs)

- `_config.yml` — site title, name, URL/baseurl → search for `TODO`
- `_data/socials.yml` — email, Google Scholar ID (already set), ORCID, GitHub, LinkedIn
- `_data/cv.yml` — CV content (education, experience, awards, publications, skills)
- `_pages/about.md` — bio / homepage text
- `_bibliography/papers.bib` — publications (BibTeX). Add entries here to auto-populate `/publications/`
- `_news/` — short announcements shown on the homepage
- `_projects/` — research project pages (shown on `/projects/`)
- `assets/img/prof_pic.jpg` — replace with your own photo

## Deploy on GitHub Pages (free)

1. Create a new GitHub repo.
   - If you name it `YOUR_USERNAME.github.io`, your site will be at the root (`baseurl:` should be blank).
   - If you name it anything else (e.g. `homepage`), set `baseurl: /homepage` in `_config.yml`.
2. Push this folder's contents to that repo (`main` branch).
3. In the repo's **Settings → Pages**, set the source to **GitHub Actions** (the included `.github/workflows/deploy.yml` handles the build).
4. Your site will be live at `https://YOUR_USERNAME.github.io` (or `.../REPO_NAME`) within a few minutes.

## Local preview (optional)

```bash
bundle install
bundle exec jekyll serve
# open http://localhost:4000/ (or the baseurl path you set)
```

Requires Ruby + Bundler. See the [al-folio Quickstart docs](https://github.com/alshedivat/al-folio/blob/main/docs/QUICKSTART.md) if you run into issues.

## Auto-updating citation counts

`.github/workflows/update-citations.yml` can periodically pull citation counts from your Google Scholar profile (ID already set in `_data/socials.yml`) — see the workflow file to enable/schedule it.
