# HAL 9000s Fantasy Football

Versioned operating material for the **HAL 9000s** ESPN fantasy-football team.

The repository preserves durable league knowledge, reusable prompts and scripts, and the changing state of each season. ESPN remains authoritative for live league state. Files here record the information needed to reason consistently across separate ChatGPT conversations.

## 2026 Structure

| Path | Purpose |
|---|---|
| `2026/reference/league-rules.md` | Confirmed ESPN league configuration and scoring |
| `2026/reference/nfl-reference.md` | NFL team normalization and confirmed bye weeks |
| `2026/reference/draft-strategy.md` | Draft-day policy retained as the record of the draft approach |
| `2026/reference/season-strategy.md` | Week-to-week roster-management policy |
| `2026/prompts/draft-activation.md` | Activation prompt used for the 2026 draft |
| `2026/prompts/weekly-activation.md` | Starts one self-contained conversation for each NFL week |
| `2026/scripts/bookmarklets/` | ESPN state-extraction tools |
| `2026/season/current-roster.md` | Latest confirmed HAL 9000s roster |
| `2026/season/transaction-log.md` | Durable record of executed moves and important decisions |
| `2026/season/weeks/TEMPLATE.md` | Template for a weekly closing record |

## Weekly Operating Flow

1. Create a separate Fantasy Football project conversation for the NFL week.
2. Paste the contents of `2026/prompts/weekly-activation.md`, replacing its week placeholder.
3. Supply fresh ESPN snapshots produced by the bookmarklets.
4. Use the conversation throughout the week for waiver, roster, injury, matchup, and lineup decisions.
5. Record only confirmed actions and durable conclusions in the repository.
6. At the end of the week, create `2026/season/weeks/week-NN.md` from the template and refresh the current roster.

## Source-of-Truth Order

When facts conflict, use this precedence:

1. Current ESPN live state
2. Current official NFL/team status and schedule information
3. Current reputable fantasy reporting and analysis
4. Repository season state
5. Older weekly conversation state
6. Preseason and draft assumptions

Never silently convert a recommendation or planned waiver claim into an executed transaction. The season files change only after ESPN state or the user confirms the action.

## Scope

This is an operational record, not a comprehensive fantasy database. Store information that improves future decisions or preserves what actually happened. Avoid copying transient news, speculative player notes, and entire conversation transcripts into source control.
