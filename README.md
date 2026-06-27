# Academic Homepage (GitHub Pages)

A clean, responsive, single-page academic homepage built with plain HTML + CSS.
No build step, no dependencies — just static files that GitHub Pages serves directly.

## Files

| File         | Purpose                                              |
| ------------ | ---------------------------------------------------- |
| `index.html` | Page content (about, research, publications, etc.)   |
| `styles.css` | All styling (light + dark mode, responsive layout)   |
| `profile.jpg`| Your photo (optional — add it yourself)              |
| `cv.pdf`     | Your CV (optional — add it yourself)                 |

## Customize before publishing

Open `index.html` and replace the placeholders:

- `your-email@mails.tsinghua.edu.cn` → your real email (appears twice)
- `https://github.com/your-username` → your GitHub profile URL
- Add a square photo named `profile.jpg` (if missing, your initials show instead)
- Add `cv.pdf` if you want the CV button to work
- Edit the About / Research / Publications text as you like

## Publish to GitHub Pages

You have two common options.

### Option A — Personal site at `https://<username>.github.io`

1. Create a new GitHub repository named **exactly** `<username>.github.io`
   (replace `<username>` with your GitHub username, e.g. `feixuecai.github.io`).
2. Push these files to the `main` branch:

   ```bash
   git init
   git add .
   git commit -m "Add academic homepage"
   git branch -M main
   git remote add origin https://github.com/<username>/<username>.github.io.git
   git push -u origin main
   ```

3. Wait ~1 minute, then open `https://<username>.github.io`.
   (Pages is enabled automatically for this special repo name.)

### Option B — Project site at `https://<username>.github.io/<repo>`

1. Create any repo (e.g. `profile`) and push the files.
2. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   pick `main` / `root`, then **Save**.
3. Your site appears at `https://<username>.github.io/<repo>/`.

## Preview locally

Just open `index.html` in a browser, or run a tiny local server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```
