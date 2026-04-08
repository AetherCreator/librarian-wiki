# Librarian Style Guide
Version: 1.0.0

## Article File Naming
- Slug: lowercase, hyphens, no spaces — `sourdough-fermentation.md`
- Path: `articles/{domain}/{slug}.md`
- Domain dirs: science, technology, history, culture, survival, economics, food, systems, meta

## Article Header Block
```
# {Title}
Domain: {domain}
Created: {YYYY-MM-DD}
Confidence: {high|medium|low}
Sources: {integer count}
```

## Required Sections (in order)
1. `## Summary` — 2-3 sentences. What IS this and why does it matter?
2. `## Core Knowledge` — Organized with `###` subheadings per distinct concept
3. `## Cross-References` — `[[slug]]` for existing, `[[RED: slug]]` for missing
4. `## Open Questions` — bullet list, minimum 2, must be genuine not rhetorical
5. `## Sources` — one per line: `- {Title} — {url} — {type}`

## Link Formats
- Existing article: `[[slug]]` renders as internal wiki link
- Missing article: `[[RED: slug]] — {one sentence why this matters}`
- External: standard markdown `[Title](url)`

## Confidence Ratings
- `high` — multiple independent quality sources agree
- `medium` — limited sources, some conflict, or single strong source
- `low` — single source, speculative, or no verifiable source

## Word Count Targets
- Minimum: 500 words (under = didn't go deep enough)
- Target: 800-2000 words
- Maximum: 3000 words (over = padding, split into subtopics)

## Quality Gates (automated checks)
1. All 5 sections present
2. ≥2 `[[RED:` links
3. ≥2 open questions
4. 500-3000 words
5. ≥1 source listed

Fail any gate → retry once. Fail twice → save as `quality: draft`, move on.
