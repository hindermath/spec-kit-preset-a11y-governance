# CLI Accessibility Review

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

- Command or workflow:
- Reviewer:
- Date:
- Target environments (macOS Terminal, iTerm2, Windows Terminal, tmux,
  screen, SSH on minimal TTY, screen reader, Braille display):

## Text-Mode Usability

- Output is meaningful in plain ASCII (no required Unicode glyphs that
  break in text browsers or older terminals):
- Every machine-readable JSON status has an equivalent concise text status;
  neither format is the sole source of required operational meaning:
- Status rows use stable ordering, explicit labels, and complete words rather
  than relying on column position, colour, icons, or animation:
- ASCII box-drawing tables have equal-width rows when used:
- No reliance on emoji or icon fonts for meaning:

## Colour Independence

- No information is conveyed by colour alone (statuses also use words
  like `OK`, `WARN`, `FAIL`):
- Output remains correct when `NO_COLOR=1` is set or `TERM=dumb`:
- Foreground/background colour combinations meet contrast where applied:

## Screen Reader and Braille

- Output remains usable with screen readers (VoiceOver, NVDA, Orca):
- Output remains usable on a Braille display (no decorative characters
  that flood the line):
- Status updates do not depend on cursor positioning, in-place rewrites,
  or animations as the only signal:
- Repeated status and resume attempts remain understandable without duplicate
  or contradictory announcements:

## Keyboard and Interaction

- All required interaction works without a mouse:
- Prompts are clearly labelled (no single-character prompts without
  context):
- Default answers and how to confirm/cancel are explicit:

## Errors and Help

- Error messages are understandable and actionable; they explain `what`,
  `why`, and `next step`:
- `--help` text follows the same accessibility rules as the rest of the
  output:
- Exit codes documented for the user:

## Bilingual Considerations

- Localised messages follow `DE first, EN second` where the project
  ships bilingual CLIs:
- German messages preserve umlauts and `ß` even on legacy Windows code
  pages (UTF-8 enforced):

## Cross-References

- Accessibility checklist entry:
- Bilingual content check entry:

## Follow-Up

- Open findings:
- Required fixes and owners:
- Re-review trigger:
