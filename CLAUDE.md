# CLAUDE.md

This file provides guidance for AI assistants working in this repository.

## Project Overview

A minimal static website hosted on GitHub Pages. The entire project is a single HTML file with no build tooling, dependencies, or frameworks.

- **Type:** Static site (GitHub Pages)
- **Stack:** Plain HTML5, no CSS, no JavaScript
- **Hosting:** GitHub Pages (served directly from the `main` branch root)

## Repository Structure

```
my-second-web-app/
└── index.html   # The entire website — entry point served by GitHub Pages
```

## Development Workflow

### No build step required

There is no package manager, bundler, or compilation step. To preview the site locally, open `index.html` directly in a browser.

### Making changes

1. Edit `index.html` directly.
2. Commit and push to the appropriate branch.
3. GitHub Pages automatically serves the updated `index.html` from the `main` branch.

### Branching

- `main` — production branch; GitHub Pages serves from here.
- Feature branches should be merged to `main` via pull request when ready to publish.

## Conventions

- Use HTML5 standards (`<!DOCTYPE html>`, semantic elements).
- Keep the `lang` attribute on `<html>` and `charset` + `viewport` meta tags in `<head>`.
- No external dependencies should be introduced without a clear reason and explicit user approval.

## Key Constraints

- There is no test suite, CI pipeline, linter, or formatter — do not assume any of these exist.
- Do not create a `package.json` or introduce a build process unless the user explicitly requests it.
- Do not add files beyond what the task requires; this project intentionally has minimal footprint.
