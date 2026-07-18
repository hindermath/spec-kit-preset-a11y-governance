# A11Y Governance Preset

Version: `0.4.0`
Status: published, standard governance preset
Priority: `40`
Requires: Spec-Kit `>=0.8.0` (uses the `wrap` and `append` composition
strategies introduced in 0.8.x).

## Zweck / Purpose

- inject accessibility, bilingual-delivery, and CEFR-B2 readability
  expectations into Spec-Kit
- make didactic inline-code-comment review explicit for new or changed
  non-trivial logic
- preserve the `Programmierung #include<everyone>` principle as a
  reusable preset instead of a local-only policy

## Installation / Install

```bash
specify preset add \
  --from https://github.com/hindermath/spec-kit-preset-a11y-governance/archive/refs/tags/v0.4.0.zip \
  --priority 40
specify preset info a11y-governance
```

```bash
specify preset add --dev /path/to/a11y-governance --priority 40
specify preset info a11y-governance
```

## Quellkapitel / Source Chapters

- `VII. Programmierung #include<everyone> — Inclusion & Accessibility By
  Default`
- `VIII. DE-First / EN-Second Bilingual Delivery`

## Standards und Regeln / Standards and Rules

- `WCAG 2.2 Level AA` baseline for every user-facing artefact
- `DE first, EN second` delivery; bilingual `DE / EN` headings or a
  synchronised `*.EN.md` companion
- `CEFR Level B2` readability target for user-facing prose
- German orthographic correctness (umlauts and `ß`, no ASCII fallbacks)
- Code-block language tagging discipline (no bare ` ``` ` fences)
- Didactic inline-code comments for non-trivial logic when learning
  comprehension or maintainability benefits
- Agent-file parity across `AGENTS.md`, `CLAUDE.md`, `GEMINI.md`, and
  `.github/copilot-instructions.md`
- A11Y coverage for `CLI`, `documentation`, `HTML`, `UI`, and generated
  templates

## Preset-Strategie / Preset Strategy

- append accessibility governance to `constitution-template`,
  `spec-template`, `plan-template`, and `tasks-template`
- provide a standalone agent-guidance addendum template for projects that
  maintain agent instruction files
- wrap `speckit.specify`, `speckit.plan`, and `speckit.tasks` with a
  shared accessibility workflow
- provide starter templates for A11Y review, bilingual content review,
  CLI accessibility review, and accessibility evidence

## Evidenzvorlagen / Evidence Templates

- Spec-Kit run evidence fields are embedded in the evidence templates to support
  audit-ready applicability, N/A rationale, reviewer, and follow-up records.
- `a11y-checklist-template` (WCAG 2.2 AA criteria coverage)
- `bilingual-content-check-template` (DE/EN headings, German
  orthography, CEFR-B2 readability, `*.EN.md` companion guidance)
- `cli-a11y-review-template` (text mode, `NO_COLOR`, screen reader,
  Braille)
- `a11y-evidence-template`
- `didactic-code-comment-check-template` (comment-needed review for
  non-trivial code logic)

Default evidence location: `docs/accessibility/`.

## Einsatz / When to Use

- any project that produces user-facing `CLI`, `documentation`, `HTML`,
  `UI`, or generated templates
- teams that want accessibility, bilingual delivery, and readability
  treated as first-class planning concerns
- learning, training, or reference projects where non-trivial code logic
  should remain understandable for apprentices and future maintainers

## Nicht verwenden / When Not to Use

- purely internal artefacts with no user-facing surface at all
- teams that do not want DE-first / EN-second guidance

## Sicherheit und Grenzen / Safety and Boundaries

- Installation adds governance prompts, templates, and wrapped Spec-Kit
  command guidance; it does not run accessibility tooling by itself.
- The preset does not grant repository, remote, merge, deployment, or
  provider-administration authority.
- WCAG, bilingual, readability, and evidence decisions remain auditable
  project decisions and must be recorded when declared `N/A`.

## Abdeckung / Coverage

- generated templates count as user-facing when humans are expected to
  read or edit them
- CLI output, review checklists, and bilingual delivery all belong to
  the preset's scope

## Versionshinweise / Release Notes

- `v0.4.0` adds audit-ready Spec-Kit run evidence fields so generated Markdown
  documents and checklists can record applicability, N/A rationale, reviewer,
  evidence path, residual risk, and follow-up per standards-relevant Spec-Kit
  run.
