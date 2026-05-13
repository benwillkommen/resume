# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static single-page HTML/CSS resume for Ben Willkommen, hosted on GitHub Pages. There is no build system, framework, or dependencies — changes to `index.html` and `style.css` are deployed directly.

## Development

To preview locally, open `index.html` in a browser or serve it with any static file server:

```sh
python3 -m http.server 8080
```

## Structure

- `index.html` — the entire resume content, structured with `<section>` and `<article>` elements
- `style.css` — all styling, including CSS animations (`instaFade`, `quickFade` with `delayTwo`–`delayFive`) and responsive layout
- `.agents/skills/` — 20 imported resume-writing skills (ATS optimizer, bullet writer, tailor, etc.)

## Resume Skills

A set of Claude Code skills for resume work is available via `/skill-name`. Key ones:

- `resume-tailor` — tailor resume content to a specific job description
- `resume-ats-optimizer` — optimize for applicant tracking systems
- `resume-bullet-writer` — rewrite bullet points with stronger impact
- `resume-quantifier` — add measurable outcomes to experience bullets
- `tech-resume-optimizer` — targeted improvements for technical roles
- `job-description-analyzer` — extract key requirements from a job posting
- `cover-letter-generator` — generate a matching cover letter

## Deployment

The site is published via GitHub Pages from the `gh-pages` branch. Merge content changes to `master`, then merge `master` into `gh-pages` to publish.
