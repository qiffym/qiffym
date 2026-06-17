# AGENTS.md

## Cursor Cloud specific instructions

This repository (`qiffym/qiffym`) is a **GitHub special profile README repository**. Its
only content is `README.md`, which GitHub renders on the owner's profile page. There is:

- **No application code**, package manager, or lockfile.
- **No dependencies** to install (so the startup update script is intentionally a no-op).
- **No build step, no tests, and no lint configuration.**

The "product" is simply the Markdown in `README.md`. To verify a change works, preview how
GitHub will render it rather than running a build/test.

### Preview the README the way GitHub renders it

Use GitHub's own Markdown API (the `gh` CLI is pre-authenticated), which renders GitHub
Flavored Markdown exactly as it appears on a profile:

```
gh api -X POST /markdown -f mode=gfm -f "text=$(cat README.md)"
```

For a visual preview, wrap that HTML in a page using `github-markdown-css` and serve it with
`python3 -m http.server`, then open it in a browser. Note: most of the current `README.md` is
inside an HTML comment (`<!-- ... -->`), so only the `## Hi there 👋` heading renders.
