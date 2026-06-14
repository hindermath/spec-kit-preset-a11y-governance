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
- Plan review of didactic inline-code-comment need for new or changed
  non-trivial logic.
- Plan review of existing comments for accuracy whenever the commented
  logic changes.
- Plan agent-file parity updates across `AGENTS.md`, `CLAUDE.md`,
  `GEMINI.md`, and `.github/copilot-instructions.md` when shared
  accessibility guidance changes.
- Plan evidence updates under `docs/accessibility/` where relevant.

## Audit Evidence Planning

- Plan audit-ready Markdown evidence for this Spec-Kit run, including owner, reviewer, evidence path, and standard-specific applicability.
- Plan how each relevant checkpoint will be recorded as `Applicable`, `N/A`, or `Open`.
- Plan concrete evidence updates under the default evidence directory for this preset; do not leave checklist templates unfilled.
- Treat `Open` as temporary: assign an owner, follow-up, and re-evaluation trigger.
