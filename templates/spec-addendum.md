## Accessibility Applicability

- Identify which user-facing artefacts this feature affects (CLI output,
  documentation, HTML, UI, generated templates, error messages,
  changelogs).
- Record the applicable `WCAG 2.2 Level AA` success criteria for each
  affected artefact type.
- Record whether bilingual `DE first, EN second` content or documentation
  is required, and whether headings must follow the bilingual `DE / EN`
  pattern or use a `*.EN.md` companion document.
- Record the readability target — default `CEFR Level B2` for user-facing
  prose, with domain terms defined on first use.
- Record whether code blocks, ASCII diagrams, or images need explicit
  language tags, alt text, or short DE/EN explanations beneath them.
- Record whether the feature adds or changes non-trivial code logic.
- Record whether didactic inline-code comments are required for learning
  comprehension or maintainability. If no code logic is affected, record
  `N/A` with a short rationale.
- Record whether accessibility evidence must be updated in
  `docs/accessibility/`.
- Record any justified `N/A` decisions with rationale. Silent omission is
  not allowed.

## Audit Evidence Applicability

- Record whether this Spec-Kit run requires an evidence document or checklist update.
- Use `Applicable`, `N/A`, or `Open` for each relevant standard or governance checkpoint.
- Document every `N/A` decision with a short rationale and re-evaluation trigger.
- Link the planned evidence path from the feature spec; silent omission is not allowed.
