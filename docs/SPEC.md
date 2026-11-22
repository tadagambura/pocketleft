# PocketLeft: Spec

**What can I safely spend before payday?** · #6 of 33 · Wave 1: Daily keepers · Used: Daily · Easy · Revenue potential: High · Money & Work · Source: ChatGPT + Perplexity (merges PocketLeft, Payday and Payday Plan)

## One-liner

Enter your income dates, bills and savings target, and PocketLeft tells you what you can safely spend today, this week and until payday. Ask 'can I afford £60 tonight?' and get a straight answer.

## Problem / audience

- **Who it's for:** Young workers, students and parents paid weekly, fortnightly, monthly or irregularly, especially anyone who runs short before payday.
- **The problem it solves:** Your bank balance isn't what you can spend: rent, bills and savings are still to come out.
- **Example:** Before a £45 night out, a user checks and sees it still leaves enough for rent, travel and food before Friday's payday.

## MVP features (ship with only these)

1. Income schedule: weekly, fortnightly, four-weekly, monthly or irregular
2. Fixed bills and a savings target
3. Safe-to-spend today, this week and until payday
4. 'Can I afford £X?' check
5. Payday countdown and upcoming-bill alerts

## Not in MVP

- Envelope budgets
- Multiple incomes and accounts
- Forecasts and a bills calendar
- Home-screen widget showing today's number

## Monetisation

| Model | Detail |
|---|---|
| Free | Safe-to-spend and payday countdown, with ads |
| Premium | £2.99/month or £19.99/year: recurring bills, forecasts, multiple incomes, widgets |
| Ads | Light, never on the main number |

Prices are starting points; test before committing. **Portfolio premium promise:** free has ads; the moment you pay you get no ads, cloud backup and storage, and sync across your devices, plus this app's extras.

## Retention: The Progression Loop

| Stage | Design |
|---|---|
| Cue | Payday, bill dates, and today's number on the widget each morning |
| Tiny win | Glance at today's number or log a spend |
| Progress | On-track days this pay cycle |
| Share | Limited (money is private); grow through search and content |
| Next step | Each payday starts a fresh cycle with a recap of the last one |
| Cadence | Daily glance, per pay cycle |

Follow the portfolio guardrails: no guilt-trip notifications, no fake urgency, progress is
never wiped, at most one notification a day by default.

## Animation and tone

**Calm.** Smooth, reassuring motion only: gentle ticks, numbers easing into place. No characters, jokes or drama.

- Today's number eases to its new value; a soft green check when on track

**Line we don't cross:** Never alarming: no flashing red or panic animations about money.

## AI

**Light.** Natural-language 'can I afford it?' ('Can I do £60 tonight and £30 on Saturday?'). Same rule: AI understands the question, code does the maths. (Portfolio rule: plain code first, code does the maths,
cheapest model, shared budget cap, premium-gated.)

## Platform & data

- **Platform:** Expo app.
- **Data:** On the device only. No bank connection in version one.
- **Backend:** AI proxy for the premium natural-language check. Premium backup and sync use the shared portfolio backend (see the master repo's HOSTING.md).
- **Stack:** shared portfolio foundation (Expo, PostHog, RevenueCat, AdMob, shared Progression Loop module).

## Growth engine

- **Content pillars:** Payday-to-payday budgeting; Can I afford it?; Simple budgeting methods; Money mistakes
- **Shareable output:** Limited (money is private); grow through search and content

## Risks

The money maths must be correct and clearly not financial advice. The separate Payday repo is retired into this one.

## Launch checklist

- [ ] Name checked on the App Store, Play Store and a trademark search
- [ ] MVP features done and tested
- [ ] Progression Loop wired (cue, tiny win, progress, milestone, next step)
- [ ] Privacy policy and terms
- [ ] Landing page
- [ ] Analytics wired (D1/D7/D30 retention)
- [ ] Payments / ads wired
- [ ] Added to growth-engine as an app config
