# The Signals · FinWise

> Module 4 · Data & Analytics. The data pattern you found and the indicators you'll steer by.

## The data pattern

no. Neither chart shows the leading indicator moving with conversion, so I’d revise the hypothesis. There’s also a data issue that limits what this dataset can tell you at all.

What the two visualizations show
Data connection vs. conversion: connection rate swung 15 points (30.5% to 45.4%), and conversion didn’t follow. The monthly correlation is essentially zero (−0.05).
The other metrics: modeling usage swung from 10.8% to 58.3%, and sessions per user from 3 to 9. Conversion held at 1.87–2.08% through all of it, a flat ceiling.

The revised hypothesis

Even setting the data issue aside, the pattern is a useful warning. Large swings in usage didn’t produce any change in paying. So I’d revise:

Original: Getting more trial users to connect their data and reach their first forecast faster will raise trial-to-paid conversion.

Revised: Reaching value once is necessary but not enough. Trial users convert when they’ve acted on their own data repeatedly before the day-14 downgrade, so losing Pro feels like a loss.

What changes:

Data connection becomes a gate, not the lever. Keep tracking first-session connection rate as a health check, since users who never connect can’t convert.
The new leading indicator is repeat value: % of trial users who complete 2+ act-and-return loops before day 14, such as clearing a risk on day 1 and again in week 2.
Rule out the paywall itself. If repeat users still don’t convert, the ceiling is downstream: pricing, how much the Free tier already gives away, or how the downgrade is presented.

_Metric patterns: Conversion, Ceiling...It barely moves: every month sits between 1.87% and 2.08%, and it ends where it started (1.93% in Oct 2023, 2.04% in Oct 2024). There’s no drop and no growth. Conversion is stuck at 2% no matter what happens in the metrics below it.. Modeling usage, Cliff....The latest month is a sharp drop: 58.1% in Sep 2024 to 36.0% in Oct 2024, down 22 points in one month. Why flagged: the 13-month trend is actually growth, from a low of 10.8% in Nov 2023 to peaks near 58%. It’s also volatile: it rose to 58.3% in Apr 2024, fell to 39.3% in May, then climbed back. So it’s a growing but unstable metric that just went off a cliff. Check whether something changed in October (a release, a pricing change, a tracking change).. Import usage, Ceiling....After a cliff in Jan 2024 (42.7% to 30.6%, staying near 31% for three months), it recovered and has held at roughly 41–45% since July. The latest four months: 45.4%, 41.2%, 45.2%, 44.3%. More than half of trial users never import their data, and that share isn’t shrinking. This is the most important ceiling here, because importing is the gate to the Aha moment.. Session duration, Cliff....It climbed to about 14 minutes in Jan–Mar 2024 and held around 11–13 through June. Then it dropped sharply: 12.1 min in Jun 2024 to 7.0 in Jul, bottoming at 5.1 in Aug. It’s recovered partly, to 8.9 min in Oct, but nowhere near the earlier level.. Sessions/user, Doesn’t fit cleanly.....It’s a V shape. The first half looks like a slow leak: 9 sessions in Oct 2023 sliding to 3 by Jan 2024, with no single dramatic month. Then it recovers steadily back to 9 and holds there for Sep–Oct 2024, which could be the start of a ceiling. Two more caveats: the values are whole numbers, so small changes don’t show, and two months at 9 isn’t enough to call a ceiling yet.._

_Correlation test: Revised._

_____

## Leading indicators

- **First-session data connection rate: % of new sign-ups who connect a bank account or upload a CSV in their first session.:** No data means no forecast, so this is the gate to the North Star, and the bank-connect step is where M1 showed most trial users dropping off before they ever see their own numbers.
- **Time to first forecast: median minutes from sign-up to the user seeing their 30-day cash forecast (target under 3 minutes).:** It’s the cheapest lever to test first: SSO, pre-filled business details, a two-tap quiz, and cutting setup screens are all small changes with results visible within days, and every minute removed before Aha cuts the chance of abandonment.

_____

## Lagging indicators

- **Trial-to-paid conversion rate at the day-14 downgrade (baseline 2%), read alongside Day-60 paid retention.:** If more users reaching the forecast early leads to more users paying when the reverse trial ends, and those payers stay, the strategy worked; if conversion rises but retention doesn’t, users were pushed through the paywall without forming the habit.

_____
