# Alessandra Este — UX research portfolio

A small static site: plain HTML and CSS, no build step, no dependencies.

```
index.html                     Home: hero, stats, case-study cards, toolkit
about.html                     Bio, experience, education, tools
work/                          One page per case study
_templates/case-study.html     Copy this to start a new case study (not published)
assets/css/style.css           All styling; colours and fonts are at the top
assets/img/                    Favicon and any case-study images
```

## Preview locally

```bash
cd ux-portfolio
python3 -m http.server 8000
# open http://localhost:8000
```

## Add a case study

1. Copy `_templates/case-study.html` to `work/<short-name>.html` and fill in the `[BRACKETS]`.
2. Copy one `<a class="card">` block in `index.html` and point it at the new page.
3. Update the "Next case study" links at the bottom of the neighbouring pages.

## Publish on GitHub Pages

1. Create a new **public** repository on GitHub (e.g. `ux-portfolio`, or `<username>.github.io` for a root URL).
2. From this folder: `git init`, `git add .`, `git commit -m "Initial portfolio"`, then add the remote and `git push -u origin main`.
3. In the repo: **Settings → Pages → Deploy from a branch → `main` / root**.
4. The site appears at `https://<username>.github.io/<repo>/` within a couple of minutes.
5. Optional: add a custom domain under the same Pages settings.

## Before you share the link

- Confirm that the figures, quotes and descriptions are cleared to be public by your employer.
- Quotes are attributed by role only. Keep it that way unless you have permission to name people.
- Put the live URL on your CV and LinkedIn.
