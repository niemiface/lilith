# CLAUDE.md

This file provides guidance for AI assistants working on the `lilith` repository.

## Repository Overview

A minimal static website with a single HTML page. There are no frameworks, build tools, dependencies, or backend code.

## Repository Structure

```
lilith/
├── index.html     # The entire website — one HTML file
├── favicon.ico    # Site icon (PNG format, ~428KB)
├── favicon.gif    # Empty placeholder (0 bytes)
├── READ.ME        # Minimal project readme
└── CLAUDE.md      # This file
```

## Development Workflow

### Making Changes

There is no build step. Edit `index.html` directly and the changes are immediately reflected when the file is opened in a browser.

### Previewing

Open `index.html` in any browser. No local server is required for this simple static page.

### No Tests or Linting

There are no tests, linters, or formatters configured. There is nothing to run.

## Git Conventions

- The primary branches are `main` and `master`.
- Feature/task branches follow the pattern `claude/<description>-<id>` (e.g. `claude/add-claude-documentation-4R2gg`).
- Commit messages in this repo have been informal (e.g. "wtf", "testing editing"). Keep messages descriptive of what actually changed.

## Key Files

| File | Purpose |
|------|---------|
| `index.html` | The complete website. Contains all HTML for the page. |
| `favicon.ico` | Browser tab icon. PNG image stored with `.ico` extension. |
| `READ.ME` | Project readme (non-standard filename, no `.md` extension). |

## Notes for AI Assistants

- This is a **zero-dependency** project. Do not introduce package managers, build tools, or frameworks unless explicitly requested.
- The entire site is `index.html`. All content changes happen there.
- No CI/CD pipeline exists. Pushes go directly to the remote without automated checks.
- The `favicon.gif` file is empty — it appears to be an unused placeholder.
- The `.DS_Store` file appears in git history; it is a macOS artifact and should not be committed going forward (consider adding a `.gitignore`).
