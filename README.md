# GitHub Pages Redirect Setup

This folder gives you a clean launcher URL (GitHub Pages) that redirects to your Google Apps Script web app.

## 1) Create repo from this folder/project
- In Codex, click `Create git repository` (or init/push manually).
- Push to GitHub.

## 2) Enable GitHub Pages
- In GitHub repo: `Settings` -> `Pages`
- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/docs`

After it publishes, you get a URL like:
- `https://<your-user-or-org>.github.io/<repo-name>/`

## 3) Use it
- Generic launcher:
  - `https://<...>.github.io/<repo-name>/`
- Job-specific:
  - `https://<...>.github.io/<repo-name>/?jobId=7055538`
- Optional pretty path also works:
  - `https://<...>.github.io/<repo-name>/job/7055538`

## Notes
- Redirect target is configured in `docs/index.html` (`WEB_APP_BASE`).
- Update `WEB_APP_BASE` only if your deployment ID changes.
