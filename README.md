# ihsanul-haq.github.io

Personal academic website for **Ihsan Ul Haq** — electrical engineer and
researcher working on AI for energy systems, smart grids, and intelligent
transportation systems.

Live at: https://ihsanul-haq.github.io/

## Structure

```
.
├── index.html   # single-page site: about, education, research, publications, projects, experience, skills, contact
├── style.css    # all styling
└── README.md
```

The site is a single static page with no build step — plain HTML and CSS,
deployed directly via GitHub Pages from the repository root.

## Updating content

- **Publications** — add a new `<li>` inside `.pub-list` in `index.html`
  (title, authors, venue/year, DOI and paper links). The list is numbered
  automatically and reversed, so newest entries go at the top of the list.
- **Projects** — grouped by research direction inside `#projects`. Add a
  new `.project-item` under the relevant `.project-group`, or add a new
  `.project-group` for a new research direction.
- **CV** — replace `Ihsan_Haq@CV.pdf` in the repository root; it's linked
  from the hero, publications note, and contact sections.
- **Profile photo** — expected at `assets/profile.jpg`; referenced by the
  `<img class="hero-photo">` in the hero section.
- **Certificates** — expected at `certifications/certificates.pdf`;
  linked from the Certifications section.
- **Permalinks** — every publication (`#pub-1` to `#pub-9`) and project
  (`#proj-<slug>`) has a stable anchor id, with a small "¶" link next to
  each title/entry that points to it. Copy these URLs to link individual
  entries from the CV or elsewhere.

## Local preview

Open `index.html` directly in a browser, or serve the folder locally:

```
python3 -m http.server 8000
```

then visit `http://localhost:8000`.

## Deployment

GitHub Pages serves this repository from the `main` branch root
automatically — no workflow or build step required. Pushing to `main`
updates the live site within a minute or two.
