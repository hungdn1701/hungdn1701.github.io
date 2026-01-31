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

Materials are organized by **phase** for each course. Add files to:

```
assets/materials/<course-name>-<lang>/
├── slides/
│   ├── week-01.pdf
│   ├── week-02.pdf
│   └── ...
└── resources/
    ├── week-01.zip    (labs, code samples, etc.)
    ├── week-02.zip
    └── ...
```

**Example for Service-Oriented Development:**
```
assets/materials/service-oriented-development-en/
├── slides/
│   ├── week-01.pdf  (Part 1: Theory)
│   ├── week-02.pdf
│   ├── week-03.pdf
│   ├── week-04.pdf
│   ├── week-05.pdf  (Part 2: Seminar)
│   ├── week-06.pdf
│   ├── week-07.pdf
│   ├── week-08.pdf
│   └── week-09.pdf
└── resources/
    ├── week-10.zip  (Part 3: Project)
    ├── week-11.zip
    ├── week-13.zip
    ├── week-15.zip
    └── week-16.zip
```

**How to add multiple slides/resources per week**: Edit the course markdown file and use `<br>` to separate links in the same cell:

```markdown
[Slides A - Introduction](/path/to/week-01-a.pdf)<br>[Slides B - Advanced](/path/to/week-01-b.pdf)
```

### Archiving and updating courses

When a semester ends, archive the course to preserve history:

1. **Archive the current course**:
   ```bash
   # In _teaching/service-oriented-development-vi.md
   archived: true
   ```

2. **Create a new course for next year**:
   ```bash
   # Clone and modify the archived version
   cp _teaching/service-oriented-development-vi.md _teaching/service-oriented-development-vi-2027.md
   
   # Edit the new file:
   # - Update semester: "Semester II, 2026–2027"
   # - Update year: 2027
   # - Update archived: false
   # - Clear or update material links as needed
   ```

3. **Copy and update materials**:
   ```bash
   # Copy old materials for reference
   cp -r assets/materials/service-oriented-development-vi assets/materials/service-oriented-development-vi-2026
   
   # Update the current course materials
   # assets/materials/service-oriented-development-vi/
   ```

This preserves all historical data while keeping the current course up-to-date.

## License

Content © Hung Dang. Theme licensed under [MIT](LICENSE).
