# 2026 ESPN League Rules — My 2026 League

> **Purpose:** Durable rules reference for the HAL 9000s live draft copilot.  
> **Authority:** League-settings screenshots supplied for the 2026 league. This document does not substitute ESPN defaults for settings that were not visible.

## League and Draft

| Setting | Value |
|---|---|
| League name | My 2026 League |
| League size | 10 teams |
| Scoring type | Head-to-Head Points, Point Per Reception |
| League format | League Manager |
| Public league | No |
| Auto-reactivate | No |
| Lineup protection | Off |
| Draft type | Snake |
| Draft date | September 6, 2026 at 12:00 PM PDT |
| Time per pick | 90 seconds |
| Draft order | Randomized one hour prior to draft time |
| Keepers for 2026 | No |
| Keepers for 2027 | No |

**Important:** The draft slot is **not durable league configuration** because the league randomizes draft order one hour before the draft. A practice-draft snapshot showed the HAL 9000s in slot 7 of 10, but that is workflow/test evidence, not the authoritative live-draft slot.

## Roster Configuration

- **Roster size:** 16
- **Total starters:** 9
- **Bench:** 7
- **IR:** 1

| Position | Starters | Maximum |
|---|---:|---:|
| QB | 1 | 4 |
| RB | 2 | 8 |
| WR | 2 | 8 |
| TE | 1 | 3 |
| FLEX | 1 | N/A |
| D/ST | 1 | 3 |
| K | 1 | 3 |
| Bench | 7 | N/A |
| IR | 1 | N/A |

The FLEX eligibility is not spelled out in the screenshots. Do **not** assume its eligible positions from ESPN defaults in live reasoning unless the live draft state or a later league source confirms them.

## Scoring

### Passing

| Event | Points |
|---|---:|
| Passing yard | 0.04 |
| Passing TD | 4 |
| Interception thrown | -2 |
| 2-point passing conversion | 2 |

### Rushing

| Event | Points |
|---|---:|
| Rushing yard | 0.1 |
| Rushing TD | 6 |
| 2-point rushing conversion | 2 |

### Receiving

| Event | Points |
|---|---:|
| Receiving yard | 0.1 |
| Reception | 1 |
| Receiving TD | 6 |
| 2-point receiving conversion | 2 |

### Kicking

| Event | Points |
|---|---:|
| PAT made | 1 |
| Total FG missed | -1 |
| FG made, 0–39 yards | 3 |
| FG made, 40–49 yards | 4 |
| FG made, 50–59 yards | 5 |
| FG made, 60+ yards | 6 |

### Team Defense / Special Teams

| Event | Points |
|---|---:|
| Kickoff return TD | 6 |
| Punt return TD | 6 |
| Interception return TD | 6 |
| Fumble return TD | 6 |
| Blocked punt/FG return TD | 6 |
| 2-point return | 2 |
| 1-point safety | 1 |
| Sack | 1 |
| Blocked punt, PAT, or FG | 2 |
| Interception | 2 |
| Fumble recovered | 2 |
| Safety | 2 |
| 0 points allowed | 5 |
| 1–6 points allowed | 4 |
| 7–13 points allowed | 3 |
| 14–17 points allowed | 1 |
| 28–34 points allowed | -1 |
| 35–45 points allowed | -3 |
| 46+ points allowed | -5 |
| <100 total yards allowed | 5 |
| 100–199 total yards allowed | 3 |
| 200–299 total yards allowed | 2 |
| 350–399 total yards allowed | -1 |
| 400–449 total yards allowed | -3 |
| 450–499 total yards allowed | -5 |
| 500–549 total yards allowed | -6 |
| 550+ total yards allowed | -7 |

**Visible-setting caveat:** The screenshots do not display explicit rows for **18–27 points allowed** or **300–349 total yards allowed**. Those ranges may score zero, but that is **not confirmed from the supplied screenshots**, so the copilot should not assert a value for them.

### Miscellaneous

| Event | Points |
|---|---:|
| Kickoff return TD | 6 |
| Punt return TD | 6 |
| Fumble recovered for TD | 6 |
| Total fumbles lost | -2 |
| Interception return TD | 6 |
| Fumble return TD | 6 |
| Blocked punt/FG return TD | 6 |
| 2-point return | 2 |
| 1-point safety | 1 |

## Fractional and Negative Scoring

- **Fractional yardage scoring is enabled in practice by the configured yard multipliers:** 0.04 per passing yard and 0.1 per rushing/receiving yard.
- **Negative scoring is present:** interceptions thrown (-2), fumbles lost (-2), missed field goals (-1), high points allowed by D/ST, and high total yards allowed by D/ST.
- The screenshots do not separately expose a league-level toggle named “fractional scoring” or “negative scoring”; the configured point values above are the authoritative evidence.

## Player, Acquisition, and Waiver Rules

| Setting | Value |
|---|---|
| Observe ESPN Undroppable Players List | Yes |
| Player universe | NFL |
| Lineup changes | Lock individually at scheduled game time |
| Player acquisition system | Waivers |
| Season acquisition limit | No limit |
| Waiver period | 1 day |
| Waiver order | Reset each week to inverse order of standings |
| Lock transactions for eliminated teams during playoffs | No |

## Trade Rules

| Setting | Value |
|---|---|
| Trade limit | No limit |
| Trade deadline | December 2, 2026 at 9:00 AM PST |
| Trade review period | 1 day |
| Votes required to veto trade | 4 |

The screenshots do not explicitly label the review authority beyond the displayed veto-vote requirement. Do not add assumptions about commissioner-only review.

## Regular Season

| Setting | Value |
|---|---|
| Start of regular season | NFL Week 1 |
| Weeks per matchup | 1 |
| Regular-season matchups | 14 |
| Matchup tie breaker | No tie breakers |
| Home-field advantage | None |
| Bonus wins and losses | No |

## Playoffs

| Setting | Value |
|---|---|
| Playoff teams | 6 |
| Weeks in Round 1 matchup | 1 |
| Weeks in Round 2 matchup | 1 |
| Weeks in championship round | 1 |
| Playoff seeding tie breaker | Total Points For |
| Playoff home-field advantage | None |
| Playoff bracket reseeding | Off |
| Lock transactions for eliminated teams during playoffs | No |
| Consolation ladder | Yes |

The screenshots do not explicitly show which NFL weeks correspond to the three playoff rounds. With 14 regular-season matchups, a Week 15–17 playoff is plausible, but **that mapping is not stated in the screenshots and is therefore not treated as authoritative here**.

## Draft Implications

This is a **10-team, full-PPR, start-2-RB/start-2-WR/1-FLEX league with only 16 active roster slots**. That pushes the draft toward weekly lineup advantage rather than deep hoarding.

- Full PPR materially raises the value of high-volume receivers and pass-catching RBs.
- Only one QB and one TE start, so replacement value at those positions is usually stronger than at RB/WR; avoid paying for a positional run unless the player is a genuine tier difference.
- One FLEX adds value to RB/WR depth because a third strong RB or WR can become an every-week starter.
- Seven bench slots are enough for upside, but not enough to justify excessive backup QBs, TEs, D/STs, or kickers.
- D/ST has unusually meaningful yardage-allowed penalties in addition to points-allowed scoring. Even so, draft capital should remain modest because defensive performance is volatile and the position is streamable.
- Kicker scoring rewards distance (up to 6 points for 60+ yards), but kicker opportunity remains volatile; it is still a late-draft position.
- Weekly waiver priority resets to inverse standings, so there is no long-term value in “saving” waiver priority. Early-season roster churn and aggressive upside claims are more defensible.
- No acquisition or trade limit supports active in-season management, which reduces the need to solve every contingency in the draft.
- Because six of ten teams make the playoffs and playoff seeding ties use total points for, the draft should favor **ceiling plus weekly scoring power** over overly conservative bye-week optimization.

## Source Notes

Authoritative league configuration was transcribed from the supplied ESPN league screenshots:
`2026-leauge-settings-1.jpg` through `2026-leauge-settings-6.jpg`.

The supplied ESPN practice-draft snapshot confirms the draft-room workflow uses a visible pick queue, snake-order pick train, player NFL-team abbreviations, and displayed bye weeks. The practice snapshot is workflow evidence, not league-rule authority.
