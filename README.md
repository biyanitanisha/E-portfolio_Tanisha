# Tanisha Biyani — GIS & Geoinformatics Portfolio

A single-page portfolio site rebuilt from the original Google Sites ePortfolio, covering:
- Home / hero intro
- About (academic background, technical skills, key interests)
- Projects (Indices Mapping, Dashboards & Visualization, Websites & Dashboards, Story Map, Geospatial Modelling)
- Field Exposure (Pashan Lake, Mayureshwar Supe, Mulshi)
- Let's Connect (email, LinkedIn, GitHub)

## Files

| File | Purpose |
|---|---|
| `index.html` | All page content and markup |
| `style.css` | Layout, typography, colors, cards, responsive rules |
| `README.md` | This file |

## Deploy to GitHub Pages (step by step)

### 1. Create a repository
1. Go to [github.com/new](https://github.com/new).
2. Name it something like `eportfolio` or `portfolio` (or use `biyanitanisha.github.io` if you want it at your root GitHub Pages URL — see note below).
3. Set it to **Public**, and click **Create repository**.

### 2. Upload the files
**Option A — via the GitHub website (no terminal needed):**
1. Open your new repository.
2. Click **Add file → Upload files**.
3. Drag in `index.html` and `style.css`.
4. Scroll down, add a commit message like "Initial portfolio upload," and click **Commit changes**.

**Option B — via Git command line:**
```bash
git clone https://github.com/biyanitanisha/YOUR-REPO-NAME.git
cd YOUR-REPO-NAME
# copy index.html and style.css into this folder
git add .
git commit -m "Initial portfolio upload"
git push
```

### 3. Turn on GitHub Pages
1. In your repository, go to **Settings → Pages** (left sidebar).
2. Under **Build and deployment → Source**, select **Deploy from a branch**.
3. Under **Branch**, choose `main` and folder `/ (root)`, then click **Save**.
4. Wait about 1–2 minutes. GitHub will show a green banner with your live URL.

### 4. Your live site
- If your repo is named `eportfolio` (or anything other than `<username>.github.io`), your site will be at:
  `https://biyanitanisha.github.io/eportfolio/`
- If you name the repo exactly `biyanitanisha.github.io`, your site becomes your root profile site:
  `https://biyanitanisha.github.io/`

### 5. Updating content later
Any time you edit `index.html` or `style.css` and push/upload again, GitHub Pages automatically redeploys within a minute or two — no extra steps needed.

## Notes on content

- **Images**: The hero and a few section images currently reference the original `googleusercontent.com` links pulled from your Google Site. These work for now since the Site is public, but Google can rotate or expire these URLs over time. For a permanent site, download the images you want to keep and add them to an `/assets` or `/images` folder in your repo, then update the `src` paths in `index.html` accordingly.
- **Story Map link**: The original Story Map page didn't have a direct public URL listed — add the link to your ArcGIS StoryMap in the card's `<a>` tag once you have it (search `Story Map — Jaipur's Historic Urban Core` in `index.html`).
- **Fonts**: The site loads Space Grotesk, Inter, and IBM Plex Mono from Google Fonts via CDN — no local font files needed, but an internet connection is required for them to load (they fall back to system sans-serif otherwise).
- **Favicon**: None is set up yet. If you want a browser-tab icon, add a `favicon.ico` (or `favicon.svg`) to the repo root and link it in the `<head>` of `index.html`:
  ```html
  <link rel="icon" href="favicon.ico">
  ```

## Customizing the design

Color tokens, fonts, and spacing all live at the top of `style.css` under `:root`. To change the accent color site-wide, edit `--accent` and `--accent-dark`. To swap fonts, update the `--font-display` / `--font-body` / `--font-mono` variables and the Google Fonts `<link>` in `index.html`'s `<head>`.
