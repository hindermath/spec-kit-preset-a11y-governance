## Accessibility Tasks

- Add explicit `WCAG 2.2 Level AA` review tasks for every affected
  user-facing artefact.
- Add bilingual content tasks (`DE first, EN second`) for headings and
  prose changes; specify inline `DE / EN` headings or a synchronised
  `*.EN.md` companion document.
- Add CEFR-B2 readability review tasks for user-facing prose; ensure each
  domain term is defined on first use.
- Add a German orthographic correctness check (umlauts and `ß`; no ASCII
  fallbacks).
- Add CLI accessibility review tasks for terminal-facing output (text
  mode, screen reader, Braille, no colour-only signalling).
- Add code-block language-tagging audit tasks (no bare ` ``` `).
- Add alt-text and DE/EN explanation tasks for ASCII diagrams, tables,
  and meaningful images.
- Add didactic inline-code-comment review tasks for new or changed
  non-trivial logic.
- Add update tasks for existing comments when their referenced logic
  changes.
- Add agent-file parity tasks across `AGENTS.md`, `CLAUDE.md`,
  `GEMINI.md`, and `.github/copilot-instructions.md` when shared
  accessibility guidance changes.
- Add accessibility evidence-update tasks under `docs/accessibility/`.

## Audit Evidence Tasks

- Add tasks to create or update the Markdown evidence/checklist documents for this Spec-Kit run.
- Each task must name the target evidence file, the standard or governance checkpoint, and the expected decision: `Applicable`, `N/A`, or `Open`.
- Add tasks to fill evidence rows with reviewer, date, evidence path, residual risk, and follow-up where relevant.
- Add tasks to verify that no relevant checkpoint was silently omitted.
