# Bharath Purtipli — Personal Website

Built with [Hugo](https://gohugo.io/) + [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme, deployed automatically to GitHub Pages.

---

## Quick-start (first-time setup)

### 1. Create the GitHub repo
Create a **public** repo named `<your-username>.github.io` on GitHub.

### 2. Add PaperMod as a git submodule
```bash
git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod themes/PaperMod
git submodule update --init --recursive
```

### 3. Enable GitHub Pages
In your repo → **Settings → Pages**:
- Source: **GitHub Actions**

### 4. Update placeholders in `hugo.toml`
| Placeholder | Replace with |
|---|---|
| `<your-github-username>` | your GitHub username |
| `bharath.purtipli@tum.de` | your actual TUM email |
| `0000-0000-0000-0000` | your ORCID iD |
| Google Scholar URL | your Scholar profile URL |
| TUM profile URL | your TUM staff page URL |

### 5. Add your profile photo
Place a photo at `static/images/profile.jpg` (any square image works).

### 6. Push to `main`
```bash
git add .
git commit -m "initial site"
git push origin main
```
The GitHub Action will build and publish your site automatically. 🎉

---

## Editing content

| Page | File |
|---|---|
| Home / About | `content/about/index.md` |
| CV (timeline) | `content/cv/index.md` |
| Publications | `content/publications/index.md` |

### Adding a publication
Copy one of the `{{< pub ... >}}` blocks in `content/publications/index.md` and fill in your details.

### Adding a timeline entry
Copy one of the `{{< timeline-item ... >}}` blocks in `content/cv/index.md`.

---

## File structure

```
.
├── hugo.toml
├── content/
│   ├── about/index.md
│   ├── cv/index.md
│   └── publications/index.md
├── layouts/shortcodes/
│   ├── timeline.html
│   ├── timeline-item.html
│   ├── pub.html
│   └── talk.html
├── assets/css/extended/
│   └── custom.css          ← timeline + pub + talk styles
├── static/
│   └── images/profile.jpg  ← add your photo here
└── .github/workflows/
    └── deploy.yml
```
