# Hanyu Bai — Personal Website

A clean, single-page academic website. Plain HTML + CSS, no build step, no
frameworks. Edit the text, drop in your images, and push to GitHub Pages.

```
hanyubai-site/
├── index.html      ← all the content lives here
├── styles.css      ← all the styling (colours & fonts at the very top)
├── assets/
│   ├── portrait.svg   ← placeholder — replace with your photo
│   ├── paper.svg      ← placeholder figure used by each publication
│   └── CV.pdf         ← (add this yourself — see below)
└── README.md
```

---

## How to edit the content

Open **`index.html`** in any text editor. It is organised top-to-bottom into
clearly commented sections:

- **Sidebar** — name, title, affiliation, contact links, and the navigation menu.
- **About / Research / News / Publications / Education / Experience / Ventures /
  Honors / Service / Skills / Beyond Research** — one `<section>` each.

Common edits:

- **Change text** — just type over what is there.
- **Add a publication** — copy one `<article class="pub"> … </article>` block,
  paste it, and edit the title, authors, venue, and link.
- **Add a news item / award** — copy one `<div class="row"> … </div>` line.
- **Add an experience entry** — copy a `<div class="entry"> … </div>` block.
- **Update your links** — replace the `href="#"` placeholders on Google
  Scholar / GitHub / LinkedIn with your real URLs.

## Add your photo

Save your photo into `assets/` (e.g. `portrait.jpg`) and update the sidebar line
in `index.html`:

```html
<img class="portrait" src="assets/portrait.jpg" alt="Portrait of Hanyu Bai">
```

A portrait crop around **3:4** (e.g. 600 × 700 px) looks best.

## Add your CV

Drop your PDF in at `assets/CV.pdf` — the "Curriculum Vitae (PDF)" link already
points there. (Optionally add small figure thumbnails per paper the same way and
swap `assets/paper.svg` for them.)

## Change colours & fonts

Open **`styles.css`** — every colour, font, and width knob is at the top inside
`:root`. For example, to change the link/accent colour, edit one line:

```css
--accent: #0b4f9c;   /* try #7a1120 (maroon) or #00274c (Michigan blue) */
```

---

## Preview locally

Just double-click `index.html` to open it in your browser. (Everything works
from the file system; the fonts load from Google Fonts when you are online.)

## Publish free on GitHub Pages

1. Create a new GitHub repository named **`<your-username>.github.io`**.
2. Upload these files (or `git push`) so `index.html` sits at the repo root.
3. In the repo, go to **Settings → Pages**, set **Source** to the `main`
   branch, `/ (root)`, and **Save**.
4. Your site goes live at `https://<your-username>.github.io` within a minute.

To use a custom domain later, add it under Settings → Pages → Custom domain.
