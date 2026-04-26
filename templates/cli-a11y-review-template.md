# CLI Accessibility Review

## Scope

- Command or workflow:
- Reviewer:
- Date:
- Target environments (macOS Terminal, iTerm2, Windows Terminal, tmux,
  screen, SSH on minimal TTY, screen reader, Braille display):

## Text-Mode Usability

- Output is meaningful in plain ASCII (no required Unicode glyphs that
  break in text browsers or older terminals):
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
