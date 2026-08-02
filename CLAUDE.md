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

1. **Home (`index.md`)** — Eye-tracking portrait + intro paragraph (`#intro`), then `now` and `elsewhere` sections. tl;dr and current-role margin notes.
2. **Projects (`projects.md`)** — List of project cards; each card has an `id` + `data-rail` so it appears in the section rail.
3. **Writing (`blog.md`)** — Reverse-chronological post list. First stub: "What is agentic and what is not".
4. **CV (`cv.md`)** — Role/client centered; dates + tech stack live in margin notes beside each job.

## Design direction

**Mono-minimalist marginalia**: monospace for UI / nav / headings / code; serif for long-form post body only. Light default + dark via the nav toggle (`data-theme` on `<html>`). The page reads as an annotated working file.

- Type: system mono stack (`ui-monospace, "SF Mono", Menlo, Consolas, monospace`) for chrome; system serif (`ui-serif, Georgia, "Times New Roman", serif`) for post body.
- Palette: 2–3 colors per mode. Background, foreground, one accent.
- Layout: three-track grid on wide screens — `200px rail | 680px content | 220px margin notes`, ~1280px canvas, centered. Margin notes fold inline ≤1200px; single column ≤940px.
- **Section rail** (the signature element): auto-built in `default.html` from `main h2[id]` and `[data-rail][id]` elements — a pipeline-style trace whose nodes fill with accent as sections scroll past. Hidden when a page has <2 sections. Don't add a second animated flourish; this is the one.
- **Margin notes**: `<aside class="note">` floats into the right track (`.note-when` for the emphasized first line, `.note-stack` for a secondary line). Use them for metadata *about* adjacent content — dates, stacks, tl;drs, sidenotes — never decoration.
- No other animation beyond hover states and the existing eye-tracking portrait / blinking cursor. Respect `prefers-reduced-motion`.

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
PATH="/opt/homebrew/opt/ruby/bin:$PATH" bundle exec jekyll serve --livereload
```

Requires Homebrew Ruby (system Ruby 2.6 is too old) + `bundle install`. Gems live in `vendor/bundle` (gitignored). Local preview uses current Jekyll 4.x, not the `github-pages` gem (its old native deps won't build here); production is still built by GitHub Pages. Not needed for deploy — only for local iteration.
