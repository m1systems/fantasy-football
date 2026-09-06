# 2026 Draft Strategy — HAL 9000s

> **Purpose:** Durable operating policy for the live ESPN draft copilot.  
> **Scope:** Decision rules and workflow only. Current rankings, injuries, projections, ADP, live availability, current rosters, current pick/clock, queue contents, and intervening teams are live-state inputs and do not belong here.

## Strategic Objective

Build the strongest weekly scoring lineup while preserving enough bench optionality to absorb injury, role changes, and bye weeks. Optimize for **value over rigid positional quotas**, but continuously account for the league's actual lineup constraints:

- 10 teams
- full PPR
- 1 QB
- 2 RB
- 2 WR
- 1 TE
- 1 FLEX
- 1 D/ST
- 1 K
- 7 bench
- 1 IR

The league is shallow enough that replacement-level QBs, TEs, defenses, and kickers will normally remain more available than starting-caliber RB/WR production. The default draft posture is therefore to accumulate weekly RB/WR scoring and upside unless a QB/TE presents a clear tier/value advantage.

## Roster-Construction Philosophy

### Core principles

1. **Draft value, not a script.** Use tiers and roster need together; do not force a position merely because a nominal round has arrived.
2. **Prioritize scarce weekly touches/targets.** Full PPR rewards reception volume, route participation, and stable opportunity.
3. **Fill the FLEX with strength.** Treat the FLEX as another weekly RB/WR starter during the draft, not as an afterthought.
4. **Bench for upside.** Bench spots should mostly buy contingent or emerging value, not duplicate low-ceiling veterans.
5. **Avoid low-leverage redundancy.** A second QB/TE is justified only by exceptional value, strategic need, or material uncertainty at the starter.
6. **Do not draft around byes.** Bye weeks break close ties; they do not override a meaningful talent/value gap.
7. **Exploit replaceability.** D/ST and K are late picks. Do not spend useful RB/WR bench capital to secure them early.

## Position Priorities by Draft Phase

The phases below are behavioral, not fixed round numbers.

### Foundation phase

Goal: secure difference-making weekly starters.

- Prefer high-confidence RB/WR volume and ceiling.
- An elite TE or QB is acceptable when the player creates a genuine positional edge and is not being selected primarily because a run has started.
- Keep both RB and WR paths open; do not force “zero RB,” “hero RB,” or any other doctrine independent of the live board.

### Starter-completion phase

Goal: complete the high-leverage weekly lineup.

- Ensure the roster is progressing toward two playable RBs, two playable WRs, and a strong FLEX.
- Fill QB/TE when the available tier/value says to do so.
- Compare the expected weekly edge of the best QB/TE against the opportunity cost of the best remaining RB/WR.

### Depth-and-upside phase

Goal: use bench spots on players who can become materially more valuable.

Prefer:

- RBs one injury/role change away from major touches;
- WRs with expanding routes/targets, strong underlying roles, or breakout paths;
- unusually discounted starters;
- one carefully chosen contingency at QB/TE if needed.

Avoid filling the bench with low-ceiling players whose best-case role is merely “usable during a bye.”

### Finalization phase

Goal: finish mandatory positions without sacrificing better upside too early.

- D/ST and K belong here by default.
- Do not draft a second D/ST or K.
- If the live platform forces all starting slots to be filled, do so as late as practical.

## Starter Versus Bench Allocation

The 16-player active roster implies 9 starters plus 7 bench players. A default bench shape should be **RB/WR heavy**.

Preferred default:

- starting QB: 1
- starting TE: 1
- D/ST: 1
- K: 1
- remaining 12 active roster slots: primarily RB/WR, including the FLEX
- backup QB/TE: only when value or risk justifies the opportunity cost

The copilot should not mechanically enforce a fixed RB/WR count. It should ask: **Does this bench player have a realistic path to becoming a weekly starter or high-value trade/waiver hold?**

## Positional Scarcity

Scarcity is dynamic and should be measured against:

- remaining tier quality;
- number of teams that still need the position;
- number of selections before the HAL 9000s' following pick;
- expected replacement options if the current tier disappears.

A position is not “scarce” merely because several players were just selected. A run matters only when it threatens to remove a tier that the HAL 9000s actually need.

## FLEX Strategy

The FLEX should usually be treated as an additional RB/WR starting slot.

- Full PPR tends to strengthen target-heavy WRs and receiving RBs.
- Do not reserve the FLEX for one position in advance.
- When two players are close, prefer the one with the stronger combination of weekly volume, ceiling, and lineup flexibility.
- FLEX depth increases the value of having a fourth/fifth playable RB/WR because injuries and matchups can be absorbed without relying immediately on waivers.

The league screenshots do not explicitly state FLEX eligibility. Until ESPN live state confirms eligible positions, the copilot should avoid asserting that TE or any other position is FLEX-eligible.

## QB Timing

Default posture: **do not chase QB solely because opponents do.**

Move on QB when one or more of the following is true:

- a clear elite/tier advantage is available at fair value;
- the next QB tier is likely to be exhausted before the following HAL 9000s pick;
- the RB/WR alternatives are flat enough that QB offers the better expected lineup edge;
- the roster already has sufficient RB/WR foundation.

Because only one QB starts in a 10-team league, replacement supply is an important counterweight to runs.

## TE Timing

TE should be handled by tiers.

- A genuine difference-maker can justify an earlier selection.
- Once the premium tier is gone, avoid panic drafting merely to “fill TE.”
- Compare the TE's projected weekly edge over later options with the RB/WR value being passed.
- A backup TE should usually require an unusually strong value case or a fragile starting situation.

## D/ST and K Timing

### D/ST

The league's defense scoring is meaningful: sacks/turnovers score, low points/yards allowed are rewarded, and high points/yards allowed can go negative. That can create weekly volatility and matchup sensitivity.

Policy:

- draft one D/ST late;
- do not sacrifice a useful upside RB/WR several picks early merely to secure a defense;
- plan to use waivers/streaming if the drafted defense loses matchup value.

### Kicker

Long field goals are rewarded progressively, including 6 points for 60+ yards, but opportunity is volatile.

Policy:

- draft one kicker late;
- favor a stable offense plus a kicker with demonstrated range when the live ranking/value is otherwise close;
- never build kicker depth.

## Upside, Floor, and Contingency

### Early picks

Bias toward durable roles and high-volume outcomes. Ceiling matters, but early picks should not require multiple uncertain events to become useful.

### Middle picks

Mix reliable starters with asymmetric upside. Prefer players whose role can grow.

### Late picks

Bias heavily toward optionality and ceiling. A late player who can become a weekly starter is more valuable than a known low-ceiling reserve.

### Contingency

React to roster-specific fragility:

- injury-prone or uncertain RB room -> add more RB contingency;
- volatile young WR room -> preserve at least one stable weekly option;
- late QB/TE -> consider a second option only if the opportunity cost is low.

## Reacting to Positional Runs

When a run begins:

1. Identify whether the run threatens a tier, not just a position.
2. Count how many teams between the current and following HAL 9000s picks plausibly need that position.
3. Estimate whether the desired tier will survive.
4. If a tier cliff is likely and the player is fairly valued, take the player before the cliff.
5. If the run is causing competitors to overpay and alternatives remain, exploit the value pushed down at other positions.

**Never chase the last player of a weak tier simply because the room is drafting the position.**

## Reasoning About Teams Between HAL 9000s Picks

The bookmarklet is intended to supply the teams selecting before the HAL 9000s' following pick. Use those teams as a short-horizon demand model.

For each intervening team, estimate:

- open starter needs;
- thin positions;
- whether they already roster a QB or TE;
- whether they have enough RB/WR depth for FLEX;
- recent position selections;
- bye-week concentrations;
- whether a candidate player fits an obvious roster hole.

Then classify each HAL target:

- **high snipe risk** — multiple intervening teams have a strong need;
- **medium snipe risk** — one plausible team or a general value target;
- **low snipe risk** — intervening teams are largely filled at the position or better alternatives exist.

Use this to decide between similarly valued players. Do not pass on a materially superior player merely because another target has higher snipe risk.

## Opponent Needs and Bye Weeks as Predictive Signals

Opponent roster need is stronger evidence than bye week.

Use this order:

1. starter vacancy / severe positional need;
2. obvious tier/value fit;
3. roster construction tendencies seen in the draft;
4. bye-week concentration as a tiebreaker.

Example logic:

- A team with no TE late in a TE tier is a stronger threat to take the TE than a team that already has one.
- If two WRs are close for an opponent and one would give that opponent three likely starters on the same bye, the other WR becomes slightly more likely.
- Do not assume rational optimization: managers may ignore byes or draft favorites. These are probability signals, not deterministic rules.

## ESPN Queue Workflow

Mock-draft testing established that manual player search can become the human bottleneck when the board moves quickly. The queue should therefore be treated as a **staging buffer**, not merely a favorites list.

### Queue operating policy

- Keep a short ordered set of immediately draftable targets before the HAL 9000s are on the clock.
- Add likely fallbacks **before** the current pick reaches HAL.
- Reorder or prune the queue after selections materially change value.
- Prefer 3–6 actionable names over a long stale list.
- When the copilot says `QUEUE:`, add those names immediately if time permits.
- If the timer becomes critical, select the highest acceptable queued player rather than spending the clock searching.

### Queue composition

At minimum, when practical:

- best current target;
- two fallbacks at comparable value;
- one player from a threatened positional tier;
- one upside/value player likely to survive only a short time.

The live draft snapshot confirms ESPN exposes a Pick Queue, and prior testing showed that queue preparation materially reduces search latency.

## Live Recommendation Decision Order

When live state arrives:

1. Validate current pick, clock, HAL roster, available players, and next/following picks.
2. Remove already drafted/unavailable candidates.
3. Identify the best value tier.
4. Apply roster need and starter/FLEX leverage.
5. Check positional scarcity and snipe risk before the following HAL pick.
6. Check bye concentration for HAL and relevant opponents.
7. Produce a compact decision; do not narrate the entire board unless asked.
8. When the clock is short, favor clarity and decisiveness over exhaustive explanation.

## Live Recommendation Format

Use this structure:

**PICK:** `Player — POS, TEAM`

**FALLBACKS:** `Player 2 — POS, TEAM`; `Player 3 — POS, TEAM`

**WHY:** One or two short sentences stating the value/tier and the roster or board reason.

**QUEUE:** Players to add immediately, in priority order, when queue action would reduce clock risk.

**WATCH:** One concise alert about a positional run, likely intervening-team need, snipe risk, or relevant bye-week pressure.

### Clock-pressure variant

When time is critically short:

**PICK:** `Player — POS, TEAM`  
**FALLBACKS:** `Player 2`; `Player 3`  
**WHY:** `<single sentence>`  
**QUEUE:** `<names or "none">`  
**WATCH:** `<single alert>`

No preamble.

## Durable / Live-State Boundary

This artifact intentionally does **not** contain:

- current player rankings or ADP;
- current injuries or depth-chart news;
- live available-player lists;
- current HAL roster;
- current opponent rosters;
- completed picks;
- current/following pick numbers;
- clock time;
- current queue;
- actual 2026 draft slot.

Those should be supplied by the bookmarklet and current ranking/news sources during the draft.

## Workflow Evidence

The supplied ESPN practice-draft snapshot and bookmarklet work establish:

- ESPN's draft is snake format in this league context;
- the draft board exposes team order, completed picks, NFL team abbreviations, player positions, and bye weeks;
- the room exposes a Pick Queue;
- the bookmarklet workflow is designed to paste structured state directly into the live ChatGPT conversation;
- prior mock testing showed that player-search latency is a practical failure mode, making queue pre-staging an important operational control.

The actual live league uses a **90-second pick clock**, so the strategy should be decisive without being as frantic as the accelerated mock-draft tests.
