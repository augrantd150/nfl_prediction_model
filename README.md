# NFL Quant Research Lab 🏈📈

**NFL forecasting · quantitative research · reproducible backtesting · Python**

A long-term NFL forecasting and quantitative research side project, built while studying and learning Python.

## Mission

Build an NFL analytics and forecasting system from scratch, improving both programming skills and statistical reasoning along the way. The long-term ambitions are (1) to explore whether the project can eventually generate **modest, consistent revenue**—for example, through useful analytics software, research tools, or other legitimate products—and (2) to build a credible, public **quantitative research / quant developer portfolio** that could help secure a quant internship or job.

**This is a goal, not a claim of profitability.** Predictive accuracy does not automatically translate into profitable betting, and no model can guarantee returns.

## Quant career objective

Use this project to demonstrate the skills valued in quantitative research and development: Python software engineering, probability and statistics, data pipelines, careful backtesting, optimization, out-of-sample evaluation, reproducibility, and clear research communication. Over time, add unit tests, documented experiments, visualizations, and well-explained results to make the work reviewable by prospective employers.

A sports forecasting project can strengthen an application, but it is **not a guarantee of a quant job**. Complement it with probability, statistics, linear algebra, algorithms, and—depending on the role—C++ and financial market fundamentals.

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
- [ ] Publish reproducible research reports, unit tests, and benchmark comparisons as a quant-job portfolio.
- [ ] Prepare a concise project write-up suitable for quant internship and job applications.

## Learning principles

- Write the code myself; use AI for hints, explanations, debugging, and review.
- Make one small, understandable improvement at a time.
- Prefer reproducible research and honest out-of-sample testing over impressive-looking backtests.
- Keep full numeric precision for calculations; round only for display.

## Research workflow

Every serious model experiment should document: (1) hypothesis, (2) data and as-of timestamps, (3) features, (4) train/validation/test periods, (5) baseline, (6) evaluation metrics, (7) limitations and next steps. Avoid tuning hyperparameters on the final test set, and never use information not available before kickoff.

Research milestones and conventions: [RESEARCH.md](RESEARCH.md). Record experiments with reproducible settings and data versions rather than treating a lucky backtest as proof of an edge.

## Project status

**Early learning / prototype stage.** No validated forecasting edge or revenue yet.
