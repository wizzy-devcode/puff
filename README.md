# Puff — an air purifier for harmattan

This is a product landing page concept for a small air purifier made for dry season.
It's one self-contained HTML file with no frameworks, no build step and no images. The only outside resource is Google Fonts.

## What you can do

- **Switch modes.** Tap **Harmattan**, **Sleep** or **Fresh**, and the whole page changes together: the colours, the fan speed, the device's display, the description and the floating dust. On phones, the browser bar colour changes too.
- **See inside.** A bento grid of tiles explains the three filter layers, the backup battery, the filter-life ring, sleep mode and how to clean the filter.

## The inspiration

- **Subject:** harmattan season, when dust hangs in the air for weeks and the sky turns orange.
- **Look:** soft, toy-like product renders. The purifier is built entirely from CSS shapes, shadows and highlights, so it looks like moulded clay without any image files. The features sit in a bento grid of rounded tiles.
- **Interaction:** mode theming. One switch re-themes the whole page around the product.
- **Trends it uses:** tactile realism (also called claymorphism) and bento grids.

| Mode | Background | Accent | Text |
| --- | --- | --- | --- |
| Harmattan | `#f3d9bf` | `#b4501d` | `#3a2216` |
| Sleep | `#dcdaf3` | `#4b48c9` | `#1e1c3f` |
| Fresh | `#d2eddb` | `#1f7a4a` | `#11301f` |

**Typefaces:** Unbounded for headings and DM Sans for text, both from Google Fonts.

### Trend references
- Bubble, [Web Design Trends 2026: What's In, What's Out](https://bubble.io/blog/web-design-trends/) (tactile realism, bento grids)
- Digital Agency Bangkok, [10 Viral Website Design Trends 2026](https://digitalagencybangkok.com/10-viral-website-design-trends-2026/) (bento grid layouts)

## Files

```
puff/
├── index.html   the whole page: HTML, CSS and JavaScript
└── README.md    this file
```

## Put it online with GitHub Pages

1. **Create a repository.** On GitHub, click **New repository**, name it `puff`, set it to **Public**, and create it.
2. **Upload the files.** Choose **Add file → Upload files**, add `index.html` and `README.md`, then click **Commit changes**.
3. **Turn on Pages.** Go to **Settings → Pages** (under "Code and automation").
4. **Choose the source.** Under **Build and deployment → Source**, pick **Deploy from a branch**. Select `main` and `/ (root)`, then click **Save**.
5. **Open your site.** After a minute or two it will be live at `https://<your-username>.github.io/puff/`.

GitHub Pages is free for public repositories.

> **Command line instead?**
> ```bash
> git init
> git add .
> git commit -m "Add Puff page"
> git branch -M main
> git remote add origin https://github.com/<your-username>/puff.git
> git push -u origin main
> ```
> Then do steps 3–5 above.

> **Keeping several pages in one repository?** Upload this whole `puff` folder to the top level of that repo instead.
> The page will then live at `https://<your-username>.github.io/<repo-name>/puff/`.

## Make it yours

- **Fill in the placeholders.** `[PRICE]`, `[HOURS]`, `[dB]`, `[MONTHS]`, `[MONTH]`, `[CITIES]`, `[NAME]`, `[CITY]` and the customer quote are waiting for real information. Search the file for `[` to find them.
- **Mode colours** are grouped at the top of the `<style>` block under `.page[data-mode="…"]`. Each mode's display text and description are in the `MODES` list near the bottom of the file.
- **The "Pre-order" buttons** are placeholders. Point them at your own checkout, order form or WhatsApp link.
- **Puff is a fictional product.** If you use this for a real one, replace the features with its real specs.

## Built to be friendly

- The page works on phones, tablets and desktops.
- The mode switch uses real buttons with pressed states, and the device has a text description that updates with each mode.
- If someone has "reduce motion" turned on, the spinning fan, drifting dust and transitions are switched off.
