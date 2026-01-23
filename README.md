# hungdn1701.github.io

Personal academic website of **Hung Dang** — Lecturer at PTIT, Backend Engineer & System Architect.

🌐 **Live site**: [hungdn1701.github.io](https://hungdn1701.github.io)

## About

This site showcases my teaching, research, and projects. Built with [Jekyll](https://jekyllrb.com/) using the [Chirpy theme](https://github.com/cotes2020/jekyll-theme-chirpy).

## Development

### Prerequisites

- Ruby 3.x
- Bundler (`gem install bundler`)

### Local Setup

```bash
# Install dependencies
bundle install

# Run development server
./tools/run.sh

# Build for production
./tools/test.sh
```

### Using GitHub Codespaces

This repo is configured for GitHub Codespaces. Just open in Codespaces and run:

```bash
./tools/run.sh -H 0.0.0.0
```

## Structure

```
├── _tabs/           # Navigation pages (about, teaching, etc.)
├── _teaching/       # Course pages
├── _data/           # Site configuration (contact, share)
├── _includes/       # Custom HTML partials
├── assets/
│   ├── img/         # Images
│   └── materials/   # Course slides & labs (PDF)
└── tools/           # Dev scripts
```

## Teaching

### Add a new course

1. Create `_teaching/course-name-vi.md` or `course-name-en.md`
2. Set front matter: `title`, `credits`, `semester`, `lang`, `year`, `archived: false`
3. Course appears automatically on Teaching page

### Archive a course

Set `archived: true` in front matter → moves to Archive section

### Upload materials

Add PDFs to `assets/materials/<course-name>-vi/` or `-en/`

## License

Content © Hung Dang. Theme licensed under [MIT](LICENSE).
