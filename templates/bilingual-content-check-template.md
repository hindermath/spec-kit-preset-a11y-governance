# Bilingual Content Check (DE first, EN after)

## Spec-Kit Run Evidence

- Feature / Spec ID:
- Spec-Kit phase: [specify / plan / tasks / implement / review / release]
- Branch / commit / PR:
- Run date:
- Evidence owner:
- Reviewer:
- Standards / criteria checked: WCAG 2.2 Level AA, accessibility evidence, bilingual DE/EN delivery, CEFR B2 readability, didactic inline-comment governance
- Decision: [Applicable / N/A / Open]
- Evidence path:
- N/A rationale, if not applicable:
- Open follow-up owner and trigger:
- Re-evaluation trigger:
- Certification-readiness note: Use this record to document accessibility applicability, concrete WCAG success criteria, test method, assistive-technology context, and justified N/A decisions.

## Audit Evidence Matrix

| Checkpoint / control reference | Applicability | Evidence produced or linked | Result | Residual risk / rationale |
| --- | --- | --- | --- | --- |
| Spec-Kit run scope is identified | [Applicable / N/A / Open] | | [OK / Open / N/A] | |
| Standard-specific criteria are mapped | [Applicable / N/A / Open] | | [OK / Open / N/A] | |
| Evidence artefact path is recorded | [Applicable / N/A / Open] | | [OK / Open / N/A] | |
| N/A decisions are justified | [Applicable / N/A / Open] | | [OK / Open / N/A] | |
| Open findings have owner and trigger | [Applicable / N/A / Open] | | [OK / Open / N/A] | |

## Scope

- Feature or document:
- Reviewer:
- Date:
- Delivery pattern (inline `DE / EN` / synchronised `*.EN.md` companion /
  other — describe):

## Heading Discipline

- All user-facing headings follow the `DE / EN` bilingual pattern, except
  for tool names and proper nouns (e.g. `Homogeneity Guardian`):
- Heading order is logical (no skipped levels):
- Anchor collisions for repeated headings are handled (GitHub appends
  `-1`, `-2`, …):

## German Orthography

- All umlauts present where required: `ä`, `ö`, `ü`, `Ä`, `Ö`, `Ü`:
- `ß` present where required (no `ss` substitution):
- No ASCII fallbacks anywhere (`fur` for `für`, `nao` for `não`,
  `loeschen` for `löschen`, `groesser` for `größer`, …):
- Accented characters from quoted foreign terms preserved:

## Translation Equivalence

- German content present first; English content present after:
- Meaning aligned across both versions (no English-only or German-only
  facts):
- Terminology consistent within and across the document:
- Links and references valid in both versions:
- Code samples, command names, and identifiers identical in both
  versions:

## CEFR-B2 Readability

- Sentences short enough for B2 readers; jargon avoided where possible:
- Domain-specific terms defined on first use in both languages:
- ASCII diagrams, meaningful tables, and graphics carry a short
  DE-first / EN-second explanation underneath:
- Lists of more than seven items broken up or grouped:

## .EN.md Companion (if applicable)

- Companion file present at expected location (e.g.
  `docs/security/threat-model.EN.md`):
- Companion file updated in the same change as the German file:
- Cross-link added in both files (`Siehe / See:`):

## Cross-References

- Accessibility checklist entry:
- CLI accessibility review entry (if terminal-facing):

## Follow-Up

- Open findings:
- Required fixes and owners:
- Re-review trigger:
