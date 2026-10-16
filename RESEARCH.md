# NFL Quant Research — Research Protocol

## Objective
Develop a reproducible, honest NFL forecasting research platform as a student-led quant portfolio. Secondary long-term goals are to investigate whether the forecasts provide economically useful insights and whether the software can generate modest recurring income. Neither profitability nor career placement is guaranteed.

## Core research question
Can a blend of season-to-date team strength and recent form improve out-of-sample NFL game predictions compared with a simple baseline?

## Hypotheses to test
- H0: Adding a recent-form weighting does not improve predictive performance over the baseline.
- H1: Properly tuned recent-form weighting improves out-of-sample predictive performance.

## Method
1. Define a prediction target (start with home win probability; address ties and missing games explicitly).
2. Calculate team-level features from games **strictly before** each predicted kickoff.
3. Use chronological data splits: train for fitting, validation for choosing weights, and a later held-out test for final evaluation.
4. Compare against straightforward baselines, including historical home-team win rate and/or simple rating systems.
5. Assess log loss, Brier score, calibration, and accuracy; report uncertainty and sample sizes.
6. If researching betting markets, incorporate historical *timestamped* odds, implied probabilities, overround/vig, market movement, and out-of-sample performance. Do not infer profitability from accuracy alone.
7. Avoid data leakage, cherry-picking, repeated test-set tuning, and unsupported profitability claims.

## Experiment log template
| ID | Hypothesis | Seasons / cutoff | Features | Weights / seed | Baseline | Validation metric | Held-out metric | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| E001 | TBD | TBD | Season vs. recent differential | TBD | TBD | TBD | TBD | Not started |

## Engineering standards (progressively)
- Separate data ingestion, feature engineering, model training, evaluation, and presentation into functions/modules.
- Put code, tests, and experiment configurations under version control.
- Use deterministic seeds for experiments where randomness is involved.
- Track dependencies and data-source licenses; avoid committing private API keys.
- Add small automated tests for calculations and edge cases.

## Quant-career portfolio outcomes
- A clean, reviewable repository with explanations of assumptions.
- Reproducible notebooks/scripts, unit tests, and comparisons to baselines.
- A research report explaining both positive **and negative** findings.
- Evidence of Python, statistics, optimization, time-series evaluation, and scientific reasoning.

## Immediate next step
Link the existing `weighted_avg()` function to one generated season/recent weight tuple. Then create a historical recent-form feature using **only past games**. Continue one small coding exercise at a time.
