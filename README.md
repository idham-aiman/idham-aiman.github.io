# Hugo Portfolio Starter

This starter contains a minimal Hugo site and a simple custom theme designed to be portfolio-like,
with sections for **Writing**, **Drawing**, **Electronics**, and **Language Learning**.

## What is included
- `config.toml` — basic site configuration (placeholders).
- `content/` — sections and example posts.
- `themes/simple-theme/` — a minimal theme with layouts and CSS.
- `static/css/styles.css` — accessible CSS for direct editing.
- `.github/workflows/gh-pages.yml` — GitHub Actions workflow to build and deploy to `gh-pages` branch.
- Sample images and placeholders (none included; add your own in `static/images/`).

---

## Quick start (complete step-by-step for someone new)

### Option A — Deploy quickly using GitHub (no local install required)
1. Create a GitHub repository named `yourusername.github.io` (replace `yourusername` with your GitHub username).
2. Clone the repo locally or upload this project folder contents via the GitHub web UI:
   - If using the web UI: Upload the files and commit to the `main` branch.
   - If using git:
     ```
     git clone https://github.com/yourusername/yourusername.github.io
     cd yourusername.github.io
     # copy files from this starter into the repo folder, commit and push
     git add .
     git commit -m "Initial Hugo starter site"
     git push origin main
     ```
3. Wait a minute. The GitHub Actions workflow `.github/workflows/gh-pages.yml` will run on push, build the site with Hugo, and push the generated `public/` folder to the `gh-pages` branch.
4. Enable GitHub Pages in repository settings:
   - Go to **Settings → Pages**.
   - Select **Branch: gh-pages / (root)** as the source if not auto-selected.
   - Save. Your site should be live at `https://yourusername.github.io/` (or `https://yourusername.github.io/repo` if using different repo name).

### Option B — Build and test locally (optional, for preview)
1. Install Hugo on your machine: https://gohugo.io/getting-started/install/
2. From the project root:
   ```
   hugo server -D
   ```
   Visit `http://localhost:1313/` to preview.
3. When ready, push to GitHub `main` branch.

---

## Editing and adding content
- Add a new post to a section by creating a Markdown file in `content/<section>/`:
  - Example: `content/writing/2025-10-26-my-post.md`
  - Use front matter:
    ```
    ---
    title: "My new post"
    date: 2025-10-26
    summary: "Short summary"
    ---
    Post content here...
    ```
- Each section (`/writing/`, `/drawing/`, etc.) has its own page listing posts.

## Customization
- Edit site title/author/description in `config.toml`.
- Change CSS in `static/css/styles.css` or `themes/simple-theme/static/css/styles.css`.
- Replace placeholder text and images in `content/`.

---

## Notes
- This starter uses a minimal custom theme so you can edit templates easily in `themes/simple-theme/layouts/`.
- If you want a different theme later, you can replace the theme folder and update `config.toml`.

