# TALLY

> **One number. That's the whole app.** Tally tells you how much you've spent this month and stops there, because the categories were never the point.

---

## Status

- Phase 1 Exploration: draft 2026-06-23
- Phase 2 Execution: not started
- Phase 3 Validation: not started

Last updated: 2026-06-23

---

## 1. Overview

**Problem**

You've tried every budgeting app. YNAB asked you to envelope your salary on a Sunday afternoon. Mint died. Copilot wanted forty-eight categories. Monarch wanted a subscription. You opened a spreadsheet and gave up by row twelve. What you actually wanted, all along, was to know how much money you've spent so far this month, compared to what you have coming in, in one glance. That's it. Every app you've installed has buried that one number under categorization, goals, projections, and tabs you didn't ask for. The anxiety isn't fixed by more detail, it's fixed by a clear answer to a simple question, which no app on the market is willing to deliver without trying to be more than that.

**Target users**

Primary: adults with one or two accounts who don't have a real budgeting problem, just no visibility. They've quit at least one budgeting app for being too complex. They want anxiety relief, not financial optimization.

Not for: power budgeters, people building complex financial plans, or people in active debt management. Tally is the minimum viable spending dashboard.

---

## 2. Product experience

Tally connects to your bank in two taps and shows you one screen, forever. That screen has one big number at the top: how much you've spent this month. Below it, in smaller type, what you've spent in the same days of last month, and what you have left until your next paycheck.

There are no categories. There is no budget to set. There is no envelope. The app's premise is that the act of seeing the number daily is enough to change behavior for the people who haven't been seeing it at all. The dashboard updates automatically and the only interaction you ever need is opening the app.

Below the number is a single feed of recent transactions, plain text, no icons or merchant logos. You can tap one and flag it as not normal, which trains Tally over time to predict whether you're tracking with your usual spend or running hot. When you're running hot, the app surfaces that as a soft line under the big number, no notification, no alert.

Tally deliberately leaves things out. There is no investing tab, no credit score widget, no savings goal, no AI assistant. There are no notifications, ever, except a single weekly Sunday morning summary you can turn off. The bet is that the people who quit other apps quit because of the noise, not because they don't care. Tally is for the person who's ready to look, as long as looking takes three seconds.

In short: Tally shows you one number that tells you whether you're okay this month, and refuses to be anything more than that.

---

## 3. Hypotheses and success metrics

| #   | Hypothesis                                                                                                | Metric                                                                              | Target |
| --- | --------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ------ |
| H1  | A no-category, one-number app actually keeps people coming back where YNAB-style ones lose them.          | % of week 1 users still opening the app weekly at week 12.                          | 50%    |
| H2  | Daily exposure to the spend number is enough to nudge users toward lower spend without a budget tool.     | Median month-over-month spend change in month 2 vs month 1.                         | -5%    |
| H3  | Anxiety, not optimization, is the real job. Users will pay to keep the anxiety relief.                    | % of free trial users who convert to paid at month 2.                               | 15%    |

---
