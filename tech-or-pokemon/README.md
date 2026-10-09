# Tech or Pokémon? — GitHub Pages upload

This folder is a complete, prebuilt website. No install or build step is needed.

## Add it under your existing profile site

1. Open the repository that publishes your personal site, usually `YOUR-USERNAME.github.io`.
2. Upload this whole `tech-or-pokemon` folder into its existing publishing directory. For branch publishing that is the repository root or `docs/`, depending on Settings → Pages.
3. Commit the files. Keep your existing Pages configuration and homepage.
4. Open `https://YOUR-USERNAME.github.io/tech-or-pokemon/` once the deployment completes. If you use a custom domain, use that domain plus `/tech-or-pokemon/`.

If your profile site uses a custom build workflow, ensure that workflow copies this folder unchanged into the final published artifact.

## Use it as the entire site instead

Upload the **contents** of this folder (including `index.html`, `assets/`, `licenses/`, and `.nojekyll`) to the root of a suitable repository. Under Settings → Pages choose **Deploy from a branch**, select the branch you uploaded to (usually `main`), and select **/(root)**. Save.

For `YOUR-USERNAME.github.io`, the site URL is `https://YOUR-USERNAME.github.io/`. For a repository named `tech-or-pokemon`, it is `https://YOUR-USERNAME.github.io/tech-or-pokemon/`.

## Preview locally

From the parent directory run:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000/tech-or-pokemon/`. Use an HTTP server rather than double-clicking `index.html`, because browsers restrict JavaScript modules opened through `file://`.

## Included

- Both original question banks: Engineering and Data (24 names each)
- 20 rounds per game, with 10 technologies and 10 Pokémon
- Original responsive design, scoring, rematches and local personal bests
- All 48 question images, local fonts and compiled JavaScript/CSS
- Faiss and Kyverno use initials because their original icon URLs returned 404

The editable source is supplied separately in `tech-or-pokemon-source.zip`. To change questions or styling, edit that source and rebuild; upload the new `dist/` contents.

The export has no backend or authentication. GitHub Pages for a personal account publishes the website publicly even when the source repository is private. Publishing from a private repository requires an eligible paid plan. This is separate from the original Sites app's workspace access.

Official configuration guide: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

Personal bests stay in each visitor's browser and do not transfer from the old Sites domain. Question text and branding are preserved from the original app; descriptions have not been independently fact-checked.
