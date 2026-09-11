# Agent Scopes

Documented ownership boundaries for future multi-agent work on this repo. These are
scope notes only — no restructuring has been done to match them yet.

| Agent | Owns | Scope |
|---|---|---|
| `content-agent` | `about.html`, `projects.md` | Content only — no CSS or workflow files |
| `style-agent` | `styles.css`, `tailwind.config.js` | Styling only — no page content |
| `deploy-agent` | `.github/workflows/pages.yml` | Deployment config only |

## Current state vs. this scope table

- `about.html` does not exist yet — About currently lives inline in `index.html`.
- `styles.css` / `tailwind.config.js` do not exist yet — styling is inline in `index.html`; there is no build step or Tailwind pipeline in this repo.
- `.github/workflows/pages.yml` does not exist yet — Pages is currently configured directly via the GitHub Pages API (legacy build from the `master` branch root), not a GitHub Actions workflow.

Adopting this table for real (splitting files, adding Tailwind, switching to an
Actions-based Pages deploy) would be a separate, explicit change.
