# zoescollage.com

Zoe Xu — stylist and writer, Shanghai. A single-page site: hero stanza,
Words, the writing list, the lookbook, About and subscribe.

Deployed by **Cloudflare Pages** from this repository. Every commit to
`main` redeploys the live site automatically, usually within a minute.

## What's here

| Path | What it is |
|---|---|
| `index.html` | The entire site — all markup and CSS in one file |
| `assets/photos/` | Outfit photos `1.jpg`–`5.jpg` and the portrait `zoe-xu.jpg` |
| `assets/og.jpg` | The preview image shown when the link is shared |
| `favicon.svg`, `apple-touch-icon.png` | Browser tab and phone home-screen icons |
| `_headers` | Cache rules for Cloudflare Pages |
| `robots.txt`, `sitemap.xml` | So search engines can index the site |

Fonts (Instrument Serif, Newsreader, Courier Prime, Archivo) load from
Google Fonts. Everything else is self-contained.

## Changing a photo

Replace the file in `assets/photos/` keeping the **same filename** — for a
new hero shot, upload it as `1.jpg`. Save around 1000px wide and under
250 KB; most visitors arrive from RedNote and Instagram on a phone.

If you add a photo under a new name, its `<img src="...">` in `index.html`
has to be updated to match, and its `alt` text rewritten to describe the
outfit.

## Adding a piece of writing

Each entry in the writing section is one `<a class="entry sheet">` block in
`index.html`. Copy an existing block, then change: the numeral (`i.`, `ii.`,
…), the label, the `<h3>` title, the `meta` line, the excerpt paragraph, the
`href` to the Substack post, and the "Read the …" text. Entries are numbered
in order, so adding one at the top means renumbering the rest.

## Editing without a terminal

Open the file on github.com and click the pencil icon, or drag a new photo
straight into the `assets/photos` folder in the browser. Committing there
triggers a redeploy on its own.
