# Didactic Code Comment Check

## Scope

- Feature:
- Reviewer:
- Date:
- Affected paths:

## Review Categories

Use one category per reviewed location:

- `CommentAdequate`: existing or added comment is useful and current.
- `CommentNeeded`: non-trivial logic needs a didactic comment.
- `NoCommentNeeded`: code is self-explanatory or purely mechanical.
- `UpdateExistingComment`: existing comment is stale or incomplete.
- `FollowUpHardening`: comment need points to a broader design or test gap.

## Checks

| Check | Result | Notes |
|---|---|---|
| Non-trivial logic identified |  |  |
| Learning or maintenance value assessed |  |  |
| Comment explains why, trade-off, boundary condition, historical deviation, or proof limit |  |  |
| Comment avoids repeating obvious code behavior |  |  |
| Comment intensity stays moderate (normally 1 to 3 lines before a non-trivial block) |  |  |
| Didactic explanation blocks stay German first, English second, and CEFR-B2 oriented |  |  |

## Follow-up

| Location | Category | Owner | Re-review trigger |
|---|---|---|---|
|  |  |  |  |

## N/A Rationale

Use this section when the feature does not add or change code logic.
