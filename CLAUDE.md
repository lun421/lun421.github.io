# Project

## Overview

Personal portfolio website of Gavin, Kuan Lun Chen.

### Purpose

- Portfolio
- Resume
- Project showcase
- Activities
- Personal branding

### Target Audience

- Recruiters
- Professional connections
- Professors
- Potential collaborators

---

# Tech Stack

## Static Site Generator

- Hugo

## Theme

- PaperMod

## Languages

- Markdown
- HTML
- CSS

## Principles

- Keep the project lightweight.
- Prefer Hugo's built-in features.
- Avoid unnecessary dependencies.

---

# Commands

## Local Preview

```bash
hugo server -D
```

If Hugo is not in PATH:

```powershell
& "$env:LOCALAPPDATA\Microsoft\WinGet\Packages\Hugo.Hugo.Extended_Microsoft.Winget.Source_8wekyb3d8bbwe\hugo.exe" server -D
```

Open:

```
http://localhost:1313
```

---

## Production Build

```bash
hugo --destination docs --cleanDestinationDir
```

`publishDir = "docs"` is configured in `hugo.toml`.

---

## Clone Project

```bash
git submodule update --init --recursive
```

---

## Verification

There is no automated test suite.

Verify changes by:

1. Building the website.
2. Running the local preview.
3. Checking the affected pages manually.

---

# Folder Structure

## Configuration

- `hugo.toml`

## Content

- `content/`

## Layouts

- `layouts/`

## Assets

- `assets/`

## Static Files

- `static/`

## Generated Output

- `docs/`

## Theme

- `themes/PaperMod/`

---

# Coding Rules

- Follow the existing project structure.
- Keep implementations simple.
- Reuse existing components whenever possible.
- Avoid duplicated code.
- Keep changes focused on the requested task.
- Preserve existing architecture unless explicitly instructed otherwise.
- Prefer Hugo features over custom JavaScript.
- Do not introduce unnecessary dependencies.

---

# Design Principles

The website should remain:

- Clean
- Professional
- Minimal
- Responsive
- Easy to read
- Consistent across all pages

Avoid unnecessary visual complexity.

---

# Content Rules

Do not modify user-provided content unless explicitly requested.

This includes:

- Resume
- Biography
- Experience
- Projects
- Activities
- Publications
- Awards
- Contact information
- Blog posts

Formatting improvements are acceptable only when requested.

---

# Hugo Rules

- Follow Hugo best practices.
- Use Hugo templates appropriately.
- Reuse layouts and partials.
- Preserve front matter.
- Do not modify the PaperMod theme directly.
- Override behavior through the project's `layouts/` directory whenever possible.

---

# Performance

Prioritize:

- Fast loading
- Small bundle size
- Minimal JavaScript
- Optimized images
- Static generation

---

# Accessibility

When applicable:

- Use semantic HTML.
- Provide image alt text.
- Maintain readable layouts.
- Preserve keyboard accessibility.

---

# SEO

Whenever creating new pages:

- Include a title.
- Include a description.
- Follow existing SEO conventions.
- Keep URLs consistent.

---

# Workflow

Before making significant changes:

- Understand the existing implementation.
- Explain the proposed approach if architecture changes are involved.

After making changes:

- Summarize modified files.
- Explain important implementation decisions.

---

# Git Rules

- Do not modify Git history.
- Do not rename files unless requested.
- Do not manually edit generated files inside `docs/`.
- Keep commits focused on a single purpose.

---

# AI Instructions

When working on this project:

- Read the relevant files before making changes.
- Follow existing coding patterns.
- Minimize unnecessary modifications.
- Preserve project consistency.
- Ask before introducing major architectural changes.
- Do not rewrite unrelated code.
- Do not assume requirements that have not been stated.

---

# Project Decisions

Record important project decisions here.

Example:

- Theme selection
- Design changes
- Folder structure changes
- New conventions

---

# Future Plans

Record planned features here.

Do not implement planned features unless explicitly requested.

---

# Notes

Additional project-specific information can be added here as the project evolves.