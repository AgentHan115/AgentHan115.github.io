# Chuhan Wang — Personal Site

A single-page portfolio site: `index.html` + `assets/images/`. No build step — just static files.

## Deploy to GitHub Pages (AgentHan115)

1. Go to https://github.com/new and create a new repository.
   - Owner: `AgentHan115`
   - Repository name: e.g. `portfolio` (this becomes part of your URL, or use `AgentHan115.github.io` for a root domain — see note below)
   - Keep it **Public** (GitHub Pages on the free plan requires a public repo)
   - Do NOT initialize with a README (you already have one here)

2. Upload the contents of this folder (`index.html`, `assets/`, `README.md`) to the repo. Easiest way if you don't use git day-to-day:
   - On the new repo's page, click **"uploading an existing file"**
   - Drag in `index.html` and the whole `assets` folder
   - Commit directly to the `main` branch

   (Or, with git installed locally:)
   ```bash
   git clone https://github.com/AgentHan115/portfolio.git
   cd portfolio
   # copy index.html and assets/ into this folder
   git add .
   git commit -m "Initial site"
   git push
   ```

3. In the repo, go to **Settings → Pages**.
   - Under "Build and deployment" → Source, choose **Deploy from a branch**
   - Branch: `main`, folder: `/ (root)`
   - Save

4. Wait a minute or two — GitHub will give you a live URL:
   - If your repo is named `portfolio`: `https://AgentHan115.github.io/portfolio/`
   - If you instead name the repo exactly `AgentHan115.github.io`, your site lives at the root: `https://AgentHan115.github.io/` (cleaner for a personal site — worth considering if you haven't created the repo yet)

## Updating later

Any time you edit `index.html` or swap an image and push/upload the change to `main`, GitHub Pages redeploys automatically within a minute or two.

## Notes for next round

- The **Eye** section is a placeholder — once you send over your photo selects, they slot into the four groups (People / Places — Cafe / Little Things / Somewhere in Between) with the hover-reveal meta (location / time / device) already wired into the design system, just not built yet.
- Nav labels are `Path / Craft / Lab / Eye / Reach`, matching section ids `#path #craft #lab #eye #reach` in `index.html`.
