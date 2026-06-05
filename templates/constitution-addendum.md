## Accessibility, Bilingual Delivery, and Inclusion

### Inclusion mandate

- `Programmierung #include<everyone>` is mandatory shared guidance and
  applies to every user-facing artefact: CLI output, documentation, HTML,
  UI, generated templates, error messages, and changelogs.
- Accessibility is not a finishing touch — it is a baseline.

### Accessibility baseline

- `WCAG 2.2 Level AA` is the default accessibility baseline wherever the
  criteria apply.
- Keep text-first usability visible for keyboard-only use, screen
  readers, Braille displays, and text browsers.
- Avoid color-dependent signalling. Avoid symbols that are unreadable on
  Braille displays or screen readers.
- Provide alternative text for all non-decorative images and diagrams.
- Maintain logical heading order. Each level-1 heading is unique and
  descriptive.

### Bilingual delivery (DE first, EN after)

- Shared guidance and learner-facing documentation use the order
  `German first, English second`.
- All user-facing headings MUST follow the bilingual format `DE / EN`.
  Tool names and proper nouns are language-neutral exceptions.
- For large normative documents, a synchronised `*.EN.md` companion file
  is acceptable instead of inline bilingual text — both versions must
  stay in sync in the same change.
- Maintain full orthographic correctness for German: keep all umlauts
  (ä, ö, ü, Ä, Ö, Ü) and `ß`. Never substitute ASCII fallbacks
  (`fur` for `für`, `nao` for `não`, `loeschen` for `löschen`).

### Readability target (CEFR-B2)

- Aim for `CEFR Level B2` readability in user-facing prose: short
  sentences, common vocabulary first, avoid unnecessary jargon.
- Define every domain-specific term on first use.
- Add a short CEFR-B2 explanation in German first and English second
  below every ASCII diagram, table that needs interpretation, or graphic
  that conveys meaning.

### Didactic inline-code comments

- New or changed non-trivial logic MUST be reviewed for didactic
  inline-code-comment value when learning comprehension or maintainability
  is affected.
- Comments explain the `why`, trade-off, boundary condition, historical
  deviation, or proof limit. They do not repeat the obvious `what` of the
  code.
- Normal comment intensity is 1 to 3 lines before a non-trivial block.
  Avoid blanket comment flooding.
- Didactic explanation blocks stay `German first, English second` and
  CEFR-B2 oriented when they are learner-facing.

### Code-block language tagging

- Every code block MUST carry a language tag (` ```bash `,
  ` ```powershell `, ` ```text ` for ASCII art / dialogues / directory
  trees).
- Bare ` ``` ` without a language tag violates `WCAG 4.1.1` (parsing) and
  is not allowed.

### Agent-file parity

- Shared accessibility guidance MUST stay aligned across the project's
  declared agent guidance surfaces. Common examples include `AGENTS.md`,
  `CLAUDE.md`, `GEMINI.md`, and `.github/copilot-instructions.md`.
  Document any intentional deviation in the same change.

### Evidence locations

- Accessibility evidence defaults to `docs/accessibility/`.
- Document every `N/A` decision with rationale; never silently omit.
