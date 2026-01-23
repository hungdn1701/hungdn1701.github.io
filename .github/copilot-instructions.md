# Copilot Instructions for hungdn1701.github.io

## Project Overview

This is a personal academic/portfolio website built with **Jekyll** using the **Chirpy theme** (`jekyll-theme-chirpy`). It's deployed on GitHub Pages and serves as Hung Dang's professional site showcasing teaching, research, and projects.

## Architecture

- **Theme**: Chirpy gem-based theme (v7.4+) - most layouts/styles come from the gem, not local files
- **Content Structure**:
  - `_tabs/` - Main navigation pages (about, projects, publications, teaching)
  - `_data/` - YAML config for contact links and share options
  - `_includes/` - Custom HTML partials overriding theme defaults (footer, topbar)
  - `_plugins/` - Ruby hooks (e.g., `posts-lastmod-hook.rb` for git-based last-modified dates)
- **Collections**: Defined in `_config.yml` - `projects`, `teaching`, `talks`, `playbook` (output: true, sorted by order)

## Developer Workflow

### Local Development

```bash
./tools/run.sh           # Start Jekyll server with live reload
./tools/run.sh -p        # Run in production mode
./tools/run.sh -H 0.0.0.0  # Bind to all interfaces (for containers)
```

### Build & Test

```bash
./tools/test.sh          # Build site and run html-proofer validation
```

### VS Code Tasks

Use the pre-configured tasks: "Run Jekyll Server" or "Build Jekyll Site"

## Content Style Guide

**Consistency rules for all pages:**

- Use `##` for main sections (not `###` with emoji)
- Tables: simple format, no bold in cells, left-align
- Lists: use `-` for bullets, `**bold**` for labels
- No intro paragraphs on tab pages (info is on index/about)
- Keep content concise and scannable

**Academic year format:**

- Semester: `Semester I, 2025–2026` or `Semester II, 2025–2026`
- Year runs August (previous year) to June (current year)

## Content Conventions

### Front Matter for Tab Pages (`_tabs/`)

```yaml
---
layout: page
icon: fas fa-info-circle # FontAwesome icon class
order: 10 # Navigation order (lower = earlier)
title: About # Optional if filename matches
---
```

### Adding New Collections

1. Define in `_config.yml` under `collections:` with `output: true` and `sort_by: order`
2. Add default scope under `defaults:` for layout
3. Create corresponding `_<collection>/` directory

### Icons

Use FontAwesome classes (e.g., `fas fa-envelope`, `fab fa-github`). See `_data/contact.yml` for examples.

## Key Files

| File                             | Purpose                                            |
| -------------------------------- | -------------------------------------------------- |
| `_config.yml`                    | Site metadata, theme config, collections, defaults |
| `index.md`                       | Homepage content with bio and tech stack           |
| `_data/contact.yml`              | Sidebar contact icons configuration                |
| `_includes/footer.html`          | Custom footer override                             |
| `_plugins/posts-lastmod-hook.rb` | Auto-sets `last_modified_at` from git history      |

## Chirpy Theme Notes

- Run `bundle info --path jekyll-theme-chirpy` to locate theme gem files
- To override theme templates, copy files from gem to local `_layouts/`, `_includes/`, etc.
- Theme docs: https://github.com/cotes2020/jekyll-theme-chirpy/wiki
- PWA is enabled (`pwa.enabled: true`) - changes may need cache invalidation

## Teaching/Courses Structure

The `_teaching/` collection stores course pages. Each course file uses this front matter:

```yaml
---
layout: page
title: Course Name
order: 1 # Display order in course list
course_code: IT4xxx # Official course code
credits: 3 # Number of credits
semester: "Semester I, 2025–2026"
lang: vi # vi or en
year: 2026 # For archiving
archived: false # Set true when semester ends
---
```

### Quick tasks

| Task           | Action                                                      |
| -------------- | ----------------------------------------------------------- |
| Add course     | Create `_teaching/course-name-vi.md`, set `archived: false` |
| Archive course | Set `archived: true` in front matter                        |
| Add materials  | Upload PDFs to `assets/materials/<course>-vi/slides/`       |
| Link materials | `[Slides](/assets/materials/course-vi/slides/week-01.pdf)`  |

Course pages should include: Overview, Objectives, Schedule, Assessment, and Resources.

## Common Tasks

### Add a new navigation tab

1. Create `_tabs/newtab.md` with proper front matter (layout, icon, order)
2. Tab appears automatically in sidebar based on `order` value

### Add a new course

1. Create `_teaching/course-name.md` with course front matter
2. Course appears automatically on Teaching page

### Override theme component

1. Find original in theme gem: `bundle info --path jekyll-theme-chirpy`
2. Copy to local project maintaining directory structure
3. Modify local copy - Jekyll prioritizes local files over gem

### Configure contact/social links

Edit `_data/contact.yml` and `_config.yml` (social section)
