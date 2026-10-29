# The Solution · FinWise

> Module 2 · Acquisition & Activation. The onboarding solution and the Aha moment that makes value land.

## Aha moment

Hypothesis: “I can see my real cash position and where my money went, without doing any bookkeeping.” In concrete terms, the user sees their own bank transactions auto-categorized into a cash flow view, with one insight they didn’t already know, such as “You spent $1,240 on software subscriptions last quarter” or “At this burn rate you have 7 weeks of runway.”

---

## Onboarding prototype

| Screen | Single job | One action |
|--------|------------|------------|
| 1 · “What matters most right now?” | Pick which insight to lead with and set industry defaults | Tap one goal: Know my cash / Get paid faster / Cut costs / Get tax-ready, plus an industry dropdown (pre-filled if possible) |
| 2 · Connect your bank | Get the real data the Aha depends on | Connect an account through a Plaid-style flow. Use one clear security line, not a wall of trust badges |
| 3 · Your money, at a glance (the Aha) | Show their cash position, auto-categorized spend, and one headline insight matched to their Screen 1 goal | Turn on a weekly cash summary email. This hands off to the habit moment |

**Optional Screen 2b** (fallback, not in the main path): if the user skips the bank connection, offer “Explore with sample data for a [their industry] business,” with a persistent “Connect your bank to see your numbers” banner. This keeps hesitant users moving instead of bouncing, but it is a weaker Aha.

**Cut from onboarding entirely** (each one can be deferred to a contextual prompt later):

- Product tour or feature carousel.
- Company profile fields: address, EIN, logo.
- Inviting teammates or an accountant. Prompt this after the Aha, when they have something worth sharing. → Reintroduced in M5 as the post-model invite trigger (the experiment) and in M6 as the paywall boundary (paid = multiplayer workspace).
- Chart-of-accounts setup.
- Notification preferences, other than the single weekly email opt-in.
- Billing details. The reverse trial means you don’t ask for these until the downgrade moment.

### Where personalization or pre-fill shortens the path

- **Sign-up:** Google or Intuit SSO pre-fills name, email, and sometimes business name, which removes form fields.
- **Screen 1:** infer industry from the email domain or a business name lookup, so the user only confirms it. Keep the quiz to 2 inputs maximum. Every extra question costs completion.
- **Screen 2:** a pre-filled bank search based on location, and the institutions small businesses most commonly use shown first.
- **Screen 3:** industry-based categorization rules, so transactions arrive already sorted (for example, a restaurant’s “Sysco” becomes Food Cost). The goal from Screen 1 decides which insight headlines the dashboard. Also badge premium features inline (“Forecast: Premium”) rather than adding an upsell screen.
- **Fallback:** sample data matched to their industry, so even the demo feels relevant.

[Onboarding prototype](https://lovable.dev/projects/4272b650-7a0d-47fe-b712-f835720c8971)

---

## Why this activates

Metrics to track:

- % of sign-ups reaching Screen 3.
- Median time-to-Aha. The target is under 5 minutes.
- Weekly email opt-in rate.
- Day-7 return rate.
- Trial-to-paid conversion, split by “connected bank” versus “sample data” (60% annual paid churn / 40% retained at 1 yr is the downstream retention context).
