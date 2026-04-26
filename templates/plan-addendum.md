## Accessibility Planning Checks

- Plan accessibility review for every affected user-facing artefact (CLI
  output, documentation, HTML, UI, generated templates).
- Plan keyboard, screen-reader, Braille-display, and text-mode
  considerations where relevant.
- Plan bilingual `DE first, EN second` content work when user-facing text
  is added or changed; plan whether headings will use the inline
  `DE / EN` pattern or a synchronised `*.EN.md` companion document.
- Plan a `CEFR Level B2` readability pass on user-facing prose.
- Plan checks for German orthographic correctness (umlauts and `ß`); no
  ASCII fallbacks.
- Plan code-block language tagging audit (` ```text ` for ASCII art /
  dialogues / directory trees; never bare ` ``` `).
- Plan alt-text and short DE/EN explanations for ASCII diagrams, tables
  needing interpretation, and meaningful images.
- Plan agent-file parity updates across `AGENTS.md`, `CLAUDE.md`,
  `GEMINI.md`, and `.github/copilot-instructions.md` when shared
  accessibility guidance changes.
- Plan evidence updates under `docs/accessibility/` where relevant.
