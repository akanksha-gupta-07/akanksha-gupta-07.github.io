# Dr. Akanksha Gupta — Personal Portfolio

A single-page personal portfolio site, hand-built with HTML + CSS + a sprinkle of JS. No build step, no dependencies — just open `index.html`.

## Files

- `index.html` — the entire site (HTML, CSS, and JS inline)
- `.nojekyll` — tells GitHub Pages to serve files as-is (no Jekyll processing)

## Preview locally

Just double-click `index.html`, or serve it with any static server:

```bash
# Python 3
python -m http.server 8080

# Node
npx serve .
```

Then open http://localhost:8080

## Deploy to GitHub Pages

### Option A — User site (lives at `https://<your-username>.github.io`)

1. On GitHub, create a new public repository named **exactly** `<your-username>.github.io` (e.g. `akanksha-gupta.github.io`).
2. In a terminal, from this folder:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. In the repo on GitHub: **Settings → Pages**. Under "Build and deployment", set **Source = Deploy from a branch**, **Branch = main**, **Folder = / (root)**, then **Save**.
4. Wait ~1 minute. Your site will be live at `https://<your-username>.github.io`.

### Option B — Project site (lives at `https://<your-username>.github.io/<repo-name>`)

1. Create any public repository (e.g. `portfolio`).
2. Push the files the same way as Option A, just to that repo.
3. **Settings → Pages → Source = Deploy from a branch → Branch = main → / (root) → Save**.
4. Site goes live at `https://<your-username>.github.io/portfolio`.

### Updating the site later

Edit `index.html`, then:

```bash
git add .
git commit -m "Update content"
git push
```

GitHub Pages rebuilds automatically within a minute.

## Custom domain (optional)

If you own a domain (e.g. `akankshagupta.com`):

1. Add a file named `CNAME` to the root with one line: your domain (e.g. `akankshagupta.com`).
2. In your DNS provider, point an A record to GitHub's Pages IPs:
   - 185.199.108.153
   - 185.199.109.153
   - 185.199.110.153
   - 185.199.111.153
3. In **Settings → Pages**, enter the custom domain and enable **Enforce HTTPS** once DNS resolves.

## What to edit

Everything is in `index.html`. Common edits:

- **LinkedIn link**: search for `id="linkedin-link"` and replace `href="#"` with your actual LinkedIn URL.
- **Hero tagline / headline**: search for `<h1>` inside the `.hero`.
- **Stats** (the four cards on the hero): search for `class="stat"`.
- **Experience entries**: search for `<article class="role">`.
- **Contact email / phone**: search for `akankshagupta1707@gmail.com` and `+919589363446` and replace if needed.

## Credits

Fonts: Inter and Space Grotesk via Google Fonts. No tracking, no analytics — clean and yours.
