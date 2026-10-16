# AuthorForge AI — GitHub Pages edition

Free browser-based book studio. **No paid AI required for writing.** Your drafts are saved locally in the browser; export backups often. Data does not sync between devices.

## Publish for hemjoshi007

1. Sign in at https://github.com/new and create a **public** repository named `authorforge-ai`. Do not initialize with a README.
2. Extract `authorforge-ai-github-pages.zip` locally. Upload **all files and the `.github` folder** into the repository root (not inside a nested folder), using **Add file → Upload files → Commit changes**. GitHub's web uploader may not preserve hidden files: if `.github/workflows/pages.yml` or `.nojekyll` is missing, use the manual Pages setup in step 3 instead.
3. In **Settings → Pages → Build and deployment**, select **GitHub Actions**. The included workflow should deploy on pushes to `main`.
4. Under **Actions**, inspect the Pages workflow until it succeeds. Open https://hemjoshi007.github.io/authorforge-ai/ . First deployment may take a few minutes.

If the workflow was not uploaded, use **Settings → Pages → Deploy from a branch → main / (root) → Save** instead. No GitHub Actions workflow is necessary for branch deployment.

## Important limits

- GitHub Pages is static hosting. It cannot run `server.py`, and **Generate via local server** will not work on this public Pages site. **Copy AI prompt** works with free AI chat tools, and you can paste results back into the editor.
- Do not upload any API keys, `.env` files, or private manuscripts to the public repository.
- GitHub Pages free hosting requires a public repository for GitHub Free personal accounts; site files will be public. The writing data saved in your browser is not uploaded to the repository.
- The public site is not a cloud account system: browser storage may be cleared, and drafts will not automatically sync across devices. Use the built-in backup regularly.
- Automatic Gemini/Groq/Ollama generation requires a separate trusted server, not this static site.
