# NFL Prediction Model 🏈

A long-term NFL forecasting and quantitative research side project, built while studying and learning Python.

## Mission

Build an NFL analytics and forecasting system from scratch, improving both programming skills and statistical reasoning along the way. The long-term ambition is to explore whether the project can eventually generate **modest, consistent revenue**—for example, through useful analytics software, research tools, or other legitimate products.

**This is a goal, not a claim of profitability.** Predictive accuracy does not automatically translate into profitable betting, and no model can guarantee returns.

## Current progress

Learning and implementing the foundations in Python (using Thonny):
- Read historical NFL schedules and game results with `nflreadpy`.
- Calculate a team's average point differential, accounting for home and away games.
- Compare two teams' historical averages.
- Generate and display random season/recent-performance weight combinations.
- Implement a weighted average for combining season-long performance with recent form.

Code is being developed locally as part of the learning process; not all features are necessarily committed to this repository yet.

## Roadmap

- [ ] Organize, test, and commit the existing Python functions.
- [ ] Calculate recent-form statistics using only games before each prediction date.
- [ ] Build a simple baseline model and compare it with weighted-average approaches.
- [ ] Evaluate candidate weights on historical training/validation periods.
- [ ] Test on a separate, later holdout period to reduce overfitting and data leakage.
- [ ] Measure prediction quality (e.g., accuracy, log loss, Brier score, calibration).
- [ ] Explore historical odds and value-bet hypotheses while accounting for bookmaker margin, costs, and variance.
- [ ] Build a small dashboard or useful analytics product.
- [ ] Investigate sustainable, lawful monetization only after demonstrating real value.

## Learning principles

- Write the code myself; use AI for hints, explanations, debugging, and review.
- Make one small, understandable improvement at a time.
- Prefer reproducible research and honest out-of-sample testing over impressive-looking backtests.
- Keep full numeric precision for calculations; round only for display.

## Project status

**Early learning / prototype stage.** No validated forecasting edge or revenue yet.
