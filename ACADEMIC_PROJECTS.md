# Academic Projects

Selected coursework from the B.S. in Computational Data Science program at Michigan State University.

## 2025 NFL Draft Selection Analysis

**CMSE 202 — Computational Modeling and Data Analysis II | Spring 2025 | Group project**

### Objective
Evaluate Tennessee's roster needs using 2024 NFL team statistics and rank 15 draft prospects for the first overall selection in the 2025 NFL Draft.

### Methods
- Cleaned and merged offensive and defensive team statistics using pandas.
- Compared team performance using regression, exploratory plots and support vector machine classifications.
- Combined consensus average draft position (60% of the composite score) with position-adjusted prospect statistics (40%) to rank candidates.

### My contributions
- Located the datasets, cleaned the records and merged the Tennessee Titans data.
- Assigned position and statistic weights and implemented the composite ranking formula.
- Helped refine the notebook, results and project documentation.

### Results
The final saved notebook ranks Cam Ward (QB, Miami) first, with a composite score of 1.0000. Travis Hunter and Abdul Carter rank second and third, respectively.

This is a historical draft decision-support case study, not a calibrated probability model. The weighted ranking relies heavily on consensus draft position, and its team classifications are exploratory rather than independently validated predictors. A multi-year evaluation and weight sensitivity analysis would be useful extensions.

The original group repository remains private. [Public portfolio edition: notebook, datasets and rankings](https://github.com/zrose1211/nfl-draft-selection-analysis). The public copy preserves the group-project attribution and distinguishes my contributions.

## College Football Outcome Predictor

**CMSE 201 | Fall 2024 | Individual project**

[View the portfolio notebook](academic/college-football/college_football_classification.ipynb)

The original project explored classification of college football team performance using 2023 season statistics. The target is a winning season (win rate greater than 50%), not an individual game outcome.

### Methods and recorded results

A 70/30 train-test split (random seed 42) was used to compare logistic regression with a depth-five decision tree. The original notebook records 40 test observations.

| Model | Accuracy | Winning-season precision | Winning-season recall | Winning-season F1 |
| --- | ---: | ---: | ---: | ---: |
| Logistic regression | 77.5% | 71% | 89% | 79% |
| Decision tree | 72.5% | 70% | 74% | 72% |

### Limitations
The recorded input schema shows only one numeric column before target creation; the original numeric-only selection may have used the exported row index rather than intended football statistics. These historical results are retained for transparency and are not a validated pregame forecast. The portfolio notebook preserves the original modeling code with condensed documentation; the original CSV is required to rerun. Future improvements include explicit numeric conversion, identifier exclusion, feature availability checks and chronological validation.

Data: [College Football Team Stats Seasons 2013 to 2023](https://www.kaggle.com/datasets/jeffgallini/college-football-team-stats-2019).

## NBA Game Outcome Prediction

**CSE 482 | Fall 2026 | Group project — in progress**

Predict home-team wins using recent team performance and rest. The first report analyzes regular-season records from 2022–23 through 2025–26 and compares logistic regression, random forest and a majority-class baseline. This is distinct from the player-level scoring project.

The first-report evaluation is complete; final project work and public release of the group notebook are pending.

[Back to portfolio](README.md)
