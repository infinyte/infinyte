# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a GitHub profile repository (`infinyte/infinyte`) — the public-facing portfolio page for Kurt Mitchell, Software Architect at Infinyte Software Solutions LLC. The repo renders as the GitHub profile homepage.

## Structure

```
.github/workflows/snake.yml   # Auto-generates contribution snake animation every 12 hours
README.md                      # The GitHub profile page (primary artifact)
```

There is no build system, package manager, source code, or test suite. All work is editing `README.md` directly.

## GitHub Actions

The snake animation workflow (`.github/workflows/snake.yml`):
- Runs on schedule (every 12 hours), push to `main`, or manual trigger
- Generates `github-snake.svg` and `github-snake-dark.svg` from the contribution graph
- Pushes generated SVGs to the `output` branch
- Requires "Read and write permissions" under repo Settings → Actions → General

To trigger manually: GitHub Actions tab → "Generate Snake Animation" → Run workflow.

## README Conventions

- The file is HTML/Markdown hybrid — `<div align="center">` wrappers are used for centering
- Badge images use `shields.io` with `style=for-the-badge`
- Typing SVGs come from `readme-typing-svg.demolab.com`
- Snake animation references the `output` branch: `https://raw.githubusercontent.com/infinyte/infinyte/output/github-snake-dark.svg`
- GitHub stats widgets use `github-readme-stats.vercel.app` and `github-readme-streak-stats.herokuapp.com`
- Featured projects are organized in an HTML `<table>` by category
