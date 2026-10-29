# The Validation · FinWise

> Module 5 · Experimentation Methods. The experiment brief that tests the bet.

## Method

**Method:** A/B Test

**Why:** Trial workspaces are independent (no shared environment), so we can randomize cleanly at the user/workspace level with a single control vs one invite-trigger variant. Conversion reads inside the trial window (weeks, not months), trial volume (~300-600/mo) supports a standard split, and nothing here needs market-level, time-alternated, or real-time reallocation machinery. Per the reference card: when in doubt and conditions allow, start with a standard A/B test.

_____

## Hypothesis + primary metric

If we inject an Invite Your Accountant/Advisor trigger immediately after a trial user completes their first financial model for FinWise trial users, we expect multiplayer trial workspaces to convert at a higher rate as measured by trial-to-paid conversion rate.

**Primary metric (6-week read):** Invite acceptance rate: % of variant-arm activated trials where an invited collaborator joins the shared workspace. Target: 30%+ of activated trials send an invite, 15%+ end up with an accepted collaborator. This is the behavior the 6-week window can actually power, and it is the M4 leading indicator for conversion.

**Confirmatory metric (long read):** Trial-to-paid conversion rate, target: sustained absolute lift from ~2% toward 3%+ (at least +1pp). Power math: detecting 2% to 3% at 80% power and alpha 0.05 needs roughly 3,800 activated trials per arm (~7,650 total). At ~300-600 trials/mo, 6 weeks yields only ~450-900 trials, an MDE of roughly +3pp, so a 6-week conversion read would be noise. Conversion is therefore read on the accumulated split at the pre-registered per-arm sample size, aligned with the M6 billing-cycle 2-3 read.

**Analysis unit:** Intent-to-treat, variant vs control across all activated trials. Comparing inviter workspaces to non-inviter workspaces is self-selected (owners who invite are higher intent) and is reported only as a descriptive secondary cut, never as the headline result.

_Experiment: Accountant Invite After First Model Test, Lift trial-to-paid conversion toward the North Star (trials that import data and reach a first modeling output) by turning single-player activation into multiplayer collaboration._

_Testing One single change: a post-model Invite Your Accountant/Advisor trigger offering one-click shared-workspace invite at the moment the first modeling output lands. on Trial users who completed data import and reached their first modeling output (activated trials). Current experience: Single-player flow: after the first financial model the user lands back on the standard dashboard. Inviting an accountant/bookkeeper is deferred (cut from onboarding in M2) with no trigger at the value moment.._

_Predicted outcome: The variant arm sends and lands invites at target rates within 6 weeks, and on the long read converts above the 2% ceiling toward 3%+ while guardrails hold.. If successful: Roll the invite trigger to 100% of activated trials, then run a holdout to confirm the retention/revenue effect over months and test invite copy and timing as follow-ups.. If unsuccessful: Check whether invites were sent but not accepted (invite friction) vs accepted but still not converting (value hypothesis wrong); revisit the M1 collaboration bet before further onboarding tweaks.._

_____

## Guardrail + read date

- **Guardrail:** Weekly return rate (the M3 streak behavior) must not drop more than 5pp in the variant and notification opt-out must not rise more than 5%; avg session duration must not collapse further. (Import % is monitored as a sanity check only: the trigger fires after the first model, downstream of import, so it should be unable to move.)
- **Read date:** 6 weeks after launch for the invite-funnel read, no peeking before then; conversion confirmatory read at the pre-registered per-arm sample size, aligned with the M6 cycles 2-3 read

_____

## Practice read (not part of deliverable — landing-page A/B, n=20)

- **Support or refute:** Version B refutes the hypothesis on the primary metric: conversion B 60% (6/10) vs A 70% (7/10), -10pp. Engagement is essentially tied (B 57.9% vs A 56.3%, +1.6pp) and session duration favors B (avg 207s vs 180s, +27s). n=20 total, so nothing is statistically significant (p>0.05); the conversion gap does not clear any reasonable MDE.
- **Scenario:** Mixed Signal, because the primary metric (conversion) points to A while secondary engagement/duration lean B — the experiment is surfacing a real tension, not a win.
- **Recommendation:** Keep Version A (higher conversion) and do not ship B; the conversion loss with only n=20 is not offset by a marginal engagement gain.
- **Next steps:** Investigate why B holds attention longer but converts worse (CTA friction in the simplified design?), segment by traffic source, then iterate on B's call-to-action and retest with a larger sample and a pre-set read date.
