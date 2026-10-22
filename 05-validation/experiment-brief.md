# The Validation · FinWise

> Module 5 · Experimentation Methods. The experiment brief that tests the bet.

## Method

**Method:** A/B Test

**Why:** Why A/B:

One intervention and one primary metric. The goal is to learn whether collaboration causes activation, not to optimize traffic in real time.
Not a multi-armed bandit: there's only one variant, and conversion feedback is slow (it arrives at trial end).
Not a holdout: a holdout is for measuring the long-term effect after shipping, so it's reserved for the 1-year retention follow-up.
Not geo or switchback: small businesses don't share supply, and regional splits add noise.

_____

## Hypothesis + primary metric

If we prompt trial account owners to invite a financial stakeholder to complete a core activation behavior together for new FinWise reverse-trial business accounts, we expect more accounts to reach the activation threshold, as measured by % of trial accounts that complete the core activation behaviors within 7 days of signup.

**Primary metric:** 7-day activation rate: % of trial accounts completing the core behaviors identified in Stage 1 (e.g., connect a bank account + categorize transactions + generate a first cash-flow report [ASSUMED]) within 7 days. Baseline 20% [ASSUMED]., target: +20% relative lift in 7-day activation (20% → 24%). This requires about 1,700 accounts per arm (95% confidence, 80% power).

_Experiment: Collaborative Activation Invite Test, Increase the share of trial accounts that reach meaningful value by bringing a second financial stakeholder (accountant, bookkeeper, co-owner) into the core activation behaviors. This feeds the North Star of weekly active paying accounts [assumed] by improving both trial-to-paid conversion (2%) and long-term retention (40% at 1 year)._

_Testing A collaboration prompt in onboarding: after the owner completes the first core behavior, FinWise suggests inviting their accountant, bookkeeper or co-owner with a pre-scoped task (e.g., "Review and approve these categorized transactions"), using role-based permissions and a one-click invite. This is the only change. on All new reverse-trial business accounts created during the enrollment window, randomized 50/50 by account. Excluded: accounts created by accountants on behalf of clients, and existing or returning accounts.. Current experience: Single-user onboarding. The owner completes setup alone. Inviting teammates is only possible from Settings and is never suggested during the trial.._

_Predicted outcome: Treatment raises 7-day activation from ~20% to ≥24% (≥+20% relative). Most of the lift comes from accounts where a collaborator accepts, with day-7 abandonment flat. Trial-to-paid conversion trends upward, but this test isn't powered to confirm it.. If successful: Ship to 100% and keep a 5% long-term holdout to measure the effect on conversion and 1-year retention. Next, test variations of the loop: invite timing, which role to invite, and collaborator-side onboarding.. If unsuccessful: Check the mechanism metrics. Low invite rate points to the prompt or timing, so iterate on the prompt. Invites sent but not accepted points to collaborator onboarding, so fix that experience. Collaborators active but no lift means collaboration isn't the lever, so return to the Stage-1 analysis and test a single-user activation intervention instead. If the guardrail is breached, roll back immediately.._

_____

## Guardrail + read date

- **Guardrail:** Day-7 trial abandonment (accounts with no session after day 1) must not rise more than 10% relative vs control. Invite friction must not cost us solo users. Secondary guardrail: invite-email spam complaints stay < 0.3%.
- **Read date:** Day 28 after launch: 21 days of enrollment to reach ~1,700 accounts per arm [ASSUMED trial volume ≥ ~1,150/week], plus a 7-day behavior window for the last cohort. No early peeking. A conversion follow-up read happens after the last cohort's trial ends (Day 35 for a 14-day trial [ASSUMED]).

_____
