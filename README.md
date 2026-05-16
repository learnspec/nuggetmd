# NuggetMD

> **Status:** Draft (v0.1) — not yet stable. Part of the [LearnSpec](https://github.com/learnspec) suite.

**NuggetMD** is an open, Markdown-based format for micro-learning.

A `.nugget.md` file is valid Markdown — readable by humans, versionable in Git, and consumable by any compatible LearnSpec player. It hosts a collection of nuggets — short, self-contained concepts designed to be read in under 3 minutes each and reviewed over time via spaced repetition. NuggetMD sits between FlashMD (atomic facts) and LearnMD (full lessons): it captures applicable, *knowing-how* concepts.

## Specification

See [SPEC.md](./SPEC.md) for the full format specification. The shared design principles, universal frontmatter fields, and cross-format directives (`!import`, `!ref`, `!checkpoint`) are defined in the [LearnSpec Architecture Charter](https://learnspec.org/charter/).

## Related formats

| Format | Repo |
|---|---|
| LearnMD — instructional content | [learnspec/learnmd](https://github.com/learnspec/learnmd) |
| QuizMD — assessments | [learnspec/quizmd](https://github.com/learnspec/quizmd) |
| FlashMD — flashcards | [learnspec/flashmd](https://github.com/learnspec/flashmd) |
| NuggetMD — micro-learning | [learnspec/nuggetmd](https://github.com/learnspec/nuggetmd) |
| CurriculumMD — objective frameworks | [learnspec/curriculummd](https://github.com/learnspec/curriculummd) |
| MediaMD — media catalogue | [learnspec/mediamd](https://github.com/learnspec/mediamd) |
| DiagramMD — diagram syntax | [learnspec/diagrammd](https://github.com/learnspec/diagrammd) |
| GlossaryMD — glossaries | [learnspec/glossarymd](https://github.com/learnspec/glossarymd) |
| TrackMD — learning paths | [learnspec/trackmd](https://github.com/learnspec/trackmd) |
| BadgeMD — micro-credentials | [learnspec/badgemd](https://github.com/learnspec/badgemd) |
| CertMD — macro-credentials | [learnspec/certmd](https://github.com/learnspec/certmd) |

## Implementations

| Project | Type | Link |
|---------|------|------|
| neuroneo.md | Web player + API + MCP server | [neuroneo.md](https://www.neuroneo.md) |
| pylearnspec | Python parser & validator | learnspec/pylearnspec |

## License

[MIT](./LICENSE)
