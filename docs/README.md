# Developer Roadmap Data

This repository stores structured roadmap data for frontend, backend, DevOps, and introductory developer-learning paths.

It is a **content/data repository**, not a runnable application. There is no package manifest, build pipeline, web server, or executable source tree to install.

## Repository structure

```text
developer-roadmap/
├── data/
│   ├── backend-map.json
│   ├── devops-map.json
│   ├── frontend-map.json
│   └── intro-map.json
└── docs/
    └── README.md
```

The repository root intentionally contains folders only. `data/` contains the maintained roadmap documents, and `docs/` contains repository guidance.

## Content conventions

- Keep each roadmap focused on one learning domain.
- Use stable identifiers when roadmap nodes may be referenced externally.
- Keep labels, descriptions, links, and prerequisite relationships explicit.
- Avoid duplicate topics unless the roadmap context genuinely changes their meaning.
- Remove obsolete resources instead of accumulating dead links indefinitely.
- Do not add application scaffolding, build tooling, or empty folders unless the repository gains an actual runtime that requires them.

## JSON maintenance

When editing a roadmap:

1. Preserve valid JSON syntax and UTF-8 encoding.
2. Keep object shapes consistent with neighboring entries.
3. Validate internal identifiers and parent/child relationships.
4. Review outbound resource links for relevance and accuracy.
5. Keep formatting deterministic so reviews show meaningful content changes rather than noisy reformatting.

If executable scripts or application code are introduced later, place them inside a dedicated project folder rather than at repository root, and document each authored file and meaningful function in plain language.
