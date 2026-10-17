# Mero-Nepal-

Mero Nepal is a small static website (Nepali/English) that collects concise, sourced information about Nepal: geography, provinces, census data, local governments, and a short political history section. The repository now contains a single static site saved at index.html and a GitHub Actions workflow to deploy the site to GitHub Pages.

What I changed
- Replaced the short/incorrect README with this full README describing the project.
- Created index.html from the existing file mero_nepal_website_demo_politics(3).html so the website lives at the repository root as index.html (keeps the political history section and the Nepali / English language toggle intact).
- Added a GitHub Actions workflow to publish the site to GitHub Pages automatically on pushes to main.

Files added/updated
- index.html — the full static website (Nepali & English toggle preserved, including the political history section).
- .github/workflows/deploy-pages.yml — GitHub Actions workflow that uploads the repository contents as a Pages artifact and deploys it.
- README.md — (this file) replaced the previous content.

How to publish the site (two options)

Option A — Use the included GitHub Actions workflow (recommended)
1. The workflow .github/workflows/deploy-pages.yml is configured to run on pushes to the main branch. It uses the official Pages actions to upload the repository content and deploy it to GitHub Pages.
2. Commit and push to main (already done by me). The action will run and deploy the site. You can check Actions → Deploy static content to GitHub Pages for logs.
3. After first successful run, your site will be available at https://<your-username>.github.io/Mero-Nepal-/ (it can take a minute to provision). Replace <your-username> with the repository owner.

Option B — Serve from the main branch (manual)
1. In your repository on GitHub go to Settings → Pages.
2. Under "Source" choose the main branch and / (root) folder, then Save.
3. The site will be served from the repository root and the URL will be the same as above.

Notes & safety
- The political history section in the site is present for educational/contextual purposes. I did not modify or remove that content — you asked to preserve it.
- The language toggle (Nepali/English) remains in the site code and functions client-side.
- If you want the site to appear under a custom domain, add a CNAME file to the repo root or configure it in Settings → Pages.

If you want, I can also:
- Add a small CSS reset or split large inline data into a separate data file.
- Move the site into a `docs/` folder (alternative Pages source) or set up a gh-pages branch deploy instead.

---

(Automated update performed: index.html and workflow files were committed.)
