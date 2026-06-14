## Accessibility Governance Agent Guidance

- Treat `CLI`, `documentation`, `HTML`, `UI`, generated templates, error
  messages, and changelogs as user-facing artefacts that fall under
  accessibility review.
- Apply `WCAG 2.2 Level AA` wherever the criteria fit. Avoid
  colour-dependent signalling and symbols that screen readers or Braille
  displays cannot represent.
- Use `DE first, EN second` for shared guidance and learner-facing
  documentation. Headings follow the bilingual `DE / EN` pattern unless a
  synchronised `*.EN.md` companion is used. Tool names and proper nouns
  are language-neutral exceptions.
- Maintain full German orthography: umlauts (ä, ö, ü, Ä, Ö, Ü) and `ß`
  must never be replaced by ASCII fallbacks (`fur`, `loeschen`, `nao`).
- Aim for CEFR Level B2 in user-facing prose. Define domain terms on
  first use. Add a short DE/EN explanation under every ASCII diagram,
  meaningful table, or graphic.
- Review new or changed non-trivial logic for didactic inline-code-comment
  value when learning comprehension or maintainability is affected.
- Good didactic comments explain the `why`, trade-off, boundary condition,
  historical deviation, or proof limit. They do not repeat the obvious
  `what` of the code. Normal intensity is 1 to 3 lines before a
  non-trivial block.
- Tag every code block with a language (` ```bash `, ` ```powershell `,
  ` ```text ` for ASCII art / dialogues / directory trees). Bare
  ` ``` ` violates WCAG 4.1.1 (parsing).
- Keep accessibility guidance aligned across `AGENTS.md`, `CLAUDE.md`,
  `GEMINI.md`, and `.github/copilot-instructions.md`. Document any
  intentional deviation in the same change.
- Document every `N/A` decision with rationale.
- Surface required evidence artefacts under `docs/accessibility/`.

## Audit-Ready Spec-Kit Evidence

- When this preset applies, generated or updated Markdown evidence must include the Spec-Kit run, owner/reviewer, evidence path, applicability decision, N/A rationale where relevant, and open follow-up tracking.
- Do not treat an unfilled starter template as evidence. Evidence exists only after the current run has recorded concrete decisions, paths, and rationale.
