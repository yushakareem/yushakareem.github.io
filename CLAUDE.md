# yushakareem.github.io

Personal site for Yusha Kareem. Hosted on GitHub Pages at `https://yushakareem.github.io`.

## Stack

- **Jekyll** (built natively by GitHub Pages — no Actions, no local build needed to deploy)
- Plain CSS, no JS framework. Vanilla JS only if a specific feature requires it.
- No build step the user has to run. Push to `main` → live in ~1 min.

## Site structure

```
/
├── _config.yml              # Jekyll config: title, baseurl, permalinks
├── _layouts/
│   ├── default.html         # Shared shell: <head>, nav, footer
│   └── post.html            # Blog post layout (extends default)
├── _includes/
│   └── nav.html             # Top nav: Home · Projects · Writing
├── _posts/
│   └── YYYY-MM-DD-*.md      # Blog posts in markdown
├── assets/
│   └── css/style.css        # Single stylesheet, light + dark via prefers-color-scheme
├── index.md                 # Intro / landing
├── projects.md              # Projects index
├── blog.md                  # Writing index (lists _posts)
├── 404.html
└── README.md
```

## Pages

1. **Home (`index.md`)** — Name, one-line tagline, short intro paragraph, links to Projects / Writing / GitHub / Email.
2. **Projects (`projects.md`)** — List of project cards. Placeholder cards for now.
3. **Writing (`blog.md`)** — Reverse-chronological post list. First stub: "What is agentic and what is not".

## Design direction

**Mono-minimalist hybrid**: monospace for UI / nav / headings / code; serif for long-form post body only. Light + dark via `prefers-color-scheme`.

- Type: system mono stack (`ui-monospace, "SF Mono", Menlo, Consolas, monospace`) for chrome; system serif (`ui-serif, Georgia, "Times New Roman", serif`) for post body.
- Palette: 2–3 colors per mode. Background, foreground, one accent.
- Layout: single column, ~640px content width, generous whitespace, no sidebar.
- No animations beyond hover states. No carousels. No hero video.
- One restrained "wow" element to consider later: subtle ASCII/typographic flourish on the home page — not now.

## Constraints / non-goals

- Don't add a JS framework (React, Next, Astro). If you reach for one, stop and reconsider.
- Don't add analytics, cookie banners, or trackers.
- Don't add a CSS framework (Tailwind, Bootstrap). One handwritten stylesheet.
- Don't add custom fonts via CDN until the design is settled — system fonts first.
- No custom domain. Stay on `yushakareem.github.io`.

## Deploy

Push to `main`. GitHub Pages auto-builds Jekyll. Enable in repo settings → Pages → Source: `Deploy from a branch` → `main` / `/ (root)`.

## Local preview (optional)

```sh
bundle exec jekyll serve
```

Requires Ruby + `bundle install` from a `Gemfile`. Not needed for deploy — only for local iteration.
