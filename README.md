# Local Business Mock Websites

Starter workspace for building and publishing mock local-business sites.

## What This Repo Is For

- Build a mock site quickly for a business lead.
- Publish it to GitHub Pages.
- Share a live link in your pitch.

## Suggested Workflow For Each New Mock Site

1. Create a folder in `sites/` (example: `sites/harbor-dental/`).
2. Build that site inside the folder (`index.html`, `styles.css`, assets).
3. Add a card/link to the root `index.html` showcase.
4. Commit and push.
5. Send the GitHub Pages link to the lead.

## Local Preview

From this folder:

```bash
python3 -m http.server 8080
```

Then open: `http://localhost:8080`

## Publishing Setup

See [GITHUB_SETUP.md](./GITHUB_SETUP.md) for full one-time setup and push flow.
