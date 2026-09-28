# Master Product Financials & Strategic Bets, Module 5 Lab

## Make your evaluation and funding decision
- **What assumption is doing the most work? If this number is 20-30% off, what changes?:** The upsell rate rising from 6% to 8% does. The case treats all 32 upsells as coming from the feature, which makes it look safe: at 20–30% off, you still get 22–26 upsells, $627K–$717K ARR, and a 3–3.4 month payback. But only the gap above the 6% baseline is incremental:

8% as planned: 8 upsells, $224K ARR, about 9.6 months payback.
20% off (6.4%): 1.6 upsells, about $45K ARR, about 48 months payback.
30% off (5.6%): below the 6% baseline, so the feature adds nothing.

A miss that looks survivable on the headline numbers actually wipes out the return.
- **What is the structural problem in this case? Look past the headline numbers for something that does not hold up on closer inspection.:** The return counts upsells that would have happened anyway. At the 6% baseline, 24 of the 32 upsells happen without the feature. The real gain is 2 points on 400 accounts: 8 upsells × $28K = $224K, not $896K, which overstates the return by 4×.

The payback has the same flaw. The case's 2.4 months is $180K ÷ ($896K / 12). On the incremental ARR it's $180K ÷ $18.7K per month = about 9.6 months. It comes to roughly 12–13 months once you include the two-quarter ramp to 8%. That still ignores 12% Enterprise churn (8 upsells drop to about 7 retained by Year 2) and gross margin.
- **Is the kill criterion complete and actionable? Does it name the consequence, or hand the decision back to the room?:** It's mostly actionable. It names the metric, the threshold (7%), the deadline (end of Q3) and the consequence (pause the feature and reallocate Q4 capacity before headcount is committed), so it doesn't hand the decision back to the room. It has three gaps:

The threshold isn't tied to the economics. 7% means 28 upsells against 24 at baseline, so 4 incremental upsells, $112K ARR and about 19 months payback. Passing the bar doesn't mean the bet worked.
It can't tell the feature's effect from noise. 4 accounts out of 400 is within normal variation, and with no holdout group any rise in upsells gets credited to the feature.
The timing and cost are vague. "End of Q3" isn't tied to the launch date, even though the case expects two quarters to reach 8%. The financial consequence isn't stated in dollars.
- **Your verdict: FUND / FUND WITH ONE CONDITION / DO NOT FUND. If a condition, name it; otherwise explain in one sentence.:** Restate the case and the kill criterion on incremental upsells only, measured against a holdout group of Standard accounts. The plan is at least 8 incremental Enterprise upsells a year ($224K ARR). If fewer than 4 incremental upsells are annualized two full quarters after launch, stop, and do not commit the Q4 capacity.

At $224K a year against a $180K build, the bet can still pay back in about a year. It just can't be funded on numbers that overstate the return by 4×.

## Write your business case
- **The strategic bet. What specific outcome are you backing, who does it serve, and what is the mechanism that connects the product decision to a financial result?:** Foremen report blockers by phone and text today, so median resolution takes 24 hours. A mobile app for them lifts weekly use from 15% to 60% of 400 accounts, and accounts whose field teams use the product churn less (10% vs 22%).
- **The assumptions. List the assumptions your case rests on, then rank them: which one, if wrong, most changes your conclusion?:** Adoption causes the lower churn. If the churn gap is 30% smaller, payback goes to 14.6 months; if half the gap is really healthy accounts adopting more, it goes to about 20.
The app reaches 60% adoption, which depends on Rock #2 (offline). At 45%, payback is 15.3 months.
Price, churn and build cost.
- **The expected return. What does the bet generate and when? Express it at unit level (per customer) and at scale (what volume hits target).:** Per account: $1,440 a year retained.
At scale: 22 accounts saved, $259K ARR a year.
Payback: about 13 months including the adoption ramp, or about 10 on full run-rate ARR.
Break-even: 53% adoption.
- **The kill criterion. Name the specific metric, threshold, timeline, and financial consequence that tells the team to stop. Actionable, not a conversation.:** Adoption gate: if fewer than 35% of accounts have at least half their foremen active weekly for 8 weeks by the end of the second full quarter after launch, the second $100K tranche isn't released and both engineers move to the next backlog item.
Churn gate: if the churn gap is under 6 points at 12 months, stop feature work on the app.

## Stress-test and finalize
- **Paste your finalized business case here.:** Business case: Rock #1, a mobile app for foremen

marks placeholder assumptions to replace with real data: $12K price per account per year, $220K build.

The bet

Foremen report blockers by phone and text, so median resolution takes 24 hours and only 25% of cases avoid duplicate reporting. A mobile app for foremen raises weekly use from 15% to 60% of 400 Standard accounts. Accounts whose field teams use the product churn less, so ARR that would otherwise churn is retained.

Assumptions, ranked

Accounts whose foremen use the app churn at least 10 points less (base case: 12 points), and the app is the cause. At a 9.6–8.4 point gap, even 60% adoption falls short of break-even (63–70% is needed). This gets checked with existing data before any build spend (Gate 0).
The app reaches 60% adoption, which depends on Rock #2 (offline). At 45% adoption, payback is 15 months.
Price and build cost ◆. If the build runs 20% over ($264K), payback is about 15 months.

Expected return

Per account: $1,440 a year retained. Build cost is $1,222 per adopting account, giving LTV:CAC of 11.8:1.
At scale: 22 accounts saved, $259K ARR a year.
Payback: about 13 months including the adoption ramp.
Break-even: 53% adoption.

Kill criterion

Gate 0, before build: compare churn over the last 12 months for today's 15% of accounts with active foremen against non-adopting accounts of similar size and tenure. If the gap is under 10 points, the $120K MVP isn't started.
Gate 1, end of the second full quarter after launch: if fewer than 35% of accounts have at least half their foremen active weekly for 8 weeks, the second $100K tranche is withheld and both engineers move to the next backlog item.
Gate 2, 9 months after launch: on renewals due in that window, if app users churn less than 10 points below matched non-users, the app is frozen in maintenance mode. No spending on the app beyond the $220K already committed.

I made three changes after the CFO review:

Gate 0 is new. It checks the churn gap against your existing data before any build money is spent.
The churn gate is stricter. The threshold is now 10 points instead of 6, which is the break-even level at 60% adoption.
The churn gate is earlier. It now runs at 9 months, measured on renewals, instead of 12.
