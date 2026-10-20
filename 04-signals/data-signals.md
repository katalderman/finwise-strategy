# The Signals · FinWise

> Module 4 · Data & Analytics. The data pattern you found and the indicators you'll steer by.

## The data pattern

The headline metric is trial-to-paid conversion stuck at ~2% (range 1.87–2.08%, mean 1.99% over 13 months), but the real pattern behind it is an activation ceiling on top of an engagement cliff: modeling usage swings wildly (10.8% to 58.3%) and import climbs to a ~45% ceiling without moving conversion, while avg session duration collapses from ~14 min to ~5 min mid-2024, because single-player modeling alone does not convert — the buying trigger is collaborative (owner + accountant in a shared workspace).

_Metric patterns: Conversion, Ceiling — holds 1.87–2.08% (mean 1.99%) across all 13 months, never breaks out. Modeling usage, Cliff after growth — climbs 10.8% to ~58% twice, then sudden drop to 36.0% in Oct 2024; swings never move conversion. Import usage, Ceiling — rises then flatlines and holds at ~44–45% (import caps out). Session duration, Cliff — collapses ~12–14 min to 5.1 min Jun–Aug 2024, the sharpest drop in the dataset. Sessions/user, Ceiling — U-shaped dip to 3 then recovers and holds at the 9 cap._

_Correlation test: Confirmed._

_____

## Leading indicators

- **Get Started Import Feature Usage %:** First half of the North Star: no import = no real-data Aha (the M2 bank-connect drop-off); lifting import directly grows trials reaching first modeling output.
- **Financial Modeling Feature Usage %:** Second half of the North Star: first modeling output is the Aha felt; worth experimenting on first because the M3 weekly streak habit depends on repeated modeling reviews.

_____

## Lagging indicators

- **Trial-to-Paid Conversion Rate (sustained lift above the 2% ceiling):** Confirms the import-to-modeling strategy actually monetized at scale; 1-yr paid retention (~40%) follows once collaborative value lands.

_____

## Pre-work (design inputs, from M1 growth-bet)

- **Growth hypothesis:** FinWise's biggest growth problem is an inability to monetize activated users, evidenced by trial-to-paid conversion frozen at ~2% even when financial-modeling engagement spikes, because a B2B financial tool cannot be justified in a single-player vacuum — the buying trigger and retention hook rely on multiplayer collaboration (owner + accountant/bookkeeper/partner in a shared workspace).
- **Funnel stage of biggest drop-off:** Activation (2% trial-to-paid; 60% churn within year one = value never landed in the reverse trial).
- **North Star (given by lab):** The number of trial users who import financial data and reach their first modeling output.
- **Testing which leading indicator vs conversion (Prompt 2):** Leading 2 — Financial Modeling Feature Usage %.
- **Prompt 2 used:** Using the same FinWise data, plot Financial Modeling Feature Usage % and Trial-to-Paid Conversion Rate on the same chart over the 13 month period.
- **Correlation verdict:** Confirmed — modeling and conversion move independently (modeling swings 10.8%→58% while conversion stays flat ~2%), which confirms the hypothesis that single-player modeling spikes don't break the 2% ceiling; the missing lever is collaborative (multiplayer workspace) activation.
