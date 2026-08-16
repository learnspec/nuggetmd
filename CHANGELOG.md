# Changelog

All notable changes to the NuggetMD specification are documented here.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
Versioning follows [Semantic Versioning](https://semver.org/).

---

## [0.3.0] — 2026-08-17

### Changed
- **`###` sub-sections are positional.** Their role now comes from their order
  within the nugget — 1st = concept, 2nd = why it matters, 3rd = check — and the
  heading text is free, in any language. Parsers take the first three `###`
  headings in document order and never match on the label.
- Validation follows: the "missing `### Concept` / `### Why it matters`" errors
  become "fewer than two `###` sections", and the warning on non-canonical
  labels becomes a warning on **more than three** sections.

### Why
The fixed English labels (`### Concept`, `### Why it matters`, `### Check`) made
a nugget written in any other language invalid — a French author writing
`### Pourquoi c'est important` silently lost that section. Accepting a list of
localised aliases was rejected: it cannot be bounded (which languages? which
spellings? maintained by whom?). Position carries the role just as reliably and
needs no vocabulary at all.

### Compatibility
Backward compatible: v0.2 files use the canonical labels in the canonical order,
so they parse identically. The one behaviour change is a file that ordered its
sections differently from its labels — e.g. `### Check` written before
`### Why it matters` — which is now read by position.

---

## [0.1] — 2026-05-15

### Added
- Initial draft of the NuggetMD specification as part of the LearnSpec suite.
