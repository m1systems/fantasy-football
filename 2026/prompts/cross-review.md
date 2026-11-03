# Fantasy Football — Cross-Review Activation

## Purpose

Conduct a structured, independent critical review of another AI advisor's fantasy football recommendations.

This workflow supports comparative analysis between ChatGPT and Claude, with the goal of improving decision quality while preserving analytical independence.

## Preconditions

Before beginning cross-review:

1. Complete your own independent analysis using the current conversation's authoritative ESPN snapshots and available NFL information.
2. Preserve your original recommendations before examining the other advisor's conclusions.
3. Confirm that both analyses are based on equivalent league state. Flag material differences in snapshot timing or data.
4. Do not retroactively revise your original recommendation.

If no independent recommendation exists in the conversation, identify the missing prerequisite rather than presenting a comparison as independent.

## Review Procedure

### 1. Identify Agreement and Disagreement

Compare the proposed lineup changes, waiver acquisitions, conditional drops, trades, or other decisions.

Identify material differences in recommended actions, priorities, assumptions, and supporting evidence.

### 2. Evaluate Evidence

Determine whether the other advisor identified relevant information you overlooked.

Separate disagreements into:

- **Factual:** Injuries, player availability, NFL roles, schedules, or league rules.
- **Predictive:** Expected performance, opportunity trends, matchup projections, or uncertainty.
- **Strategic:** Roster construction, opportunity cost, risk tolerance, or short-term versus long-term value.

Verify material factual disagreements against authoritative sources.

### 3. Challenge Both Analyses

Critically evaluate the other advisor's reasoning and your own.

Do not automatically defer to the other model or manufacture disagreement for the sake of independence.

Explicitly identify any new information that changes the strength of your original recommendation.

### 4. Reassess Transactions

For waiver and free-agent decisions, evaluate complete add/drop pairs.

Consider:

- Immediate starting-lineup improvement.
- Rest-of-season value.
- Player opportunity and upside.
- Injury and bye-week contingencies.
- Opportunity cost of dropping an existing player.
- Waiver priority and acquisition restrictions.

Do not assume an acquisition is possible unless supported by current ESPN state.

### 5. Produce Final Assessment

Use the following structure:

**Agreement:** Areas where both advisors concur.

**Disagreement:** Material differences and their underlying causes.

**New evidence:** Important information introduced by the other advisor, with verification status.

**Original recommendation:** Your position before cross-review.

**Final recommendation:** Maintain or revise your position, with a concise explanation.

**Confidence:** High, Medium, or Low, with the principal uncertainty.

## Operating Rules

- Preserve the original recommendation for historical comparison.
- Do not confuse model consensus with independent evidence.
- Do not repeatedly exchange revised analyses merely to achieve agreement.
- Prefer one independent analysis followed by one cross-review.
- Escalate unresolved factual disagreements for targeted verification.
- The user retains final decision-making authority.
- Do not perform ESPN transactions or modify repository records without authorization.

## Season Evaluation

Where decisions and outcomes are recorded, support retrospective evaluation of both independent recommendations and the cross-review process.

Distinguish decision quality from realized fantasy scoring.

Evaluate whether cross-review uncovered meaningful information, corrected errors, or improved the resulting decision.

---

## Review Input

**Other advisor:** {{ADVISOR_NAME}}

**Other advisor's original analysis:**

{{OTHER_ADVISOR_ANALYSIS}}