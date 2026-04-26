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
- Tag every code block with a language (` ```bash `, ` ```powershell `,
  ` ```text ` for ASCII art / dialogues / directory trees). Bare
  ` ``` ` violates WCAG 4.1.1 (parsing).
- Keep accessibility guidance aligned across `AGENTS.md`, `CLAUDE.md`,
  `GEMINI.md`, and `.github/copilot-instructions.md`. Document any
  intentional deviation in the same change.
- Document every `N/A` decision with rationale.
- Surface required evidence artefacts under `docs/accessibility/`.
