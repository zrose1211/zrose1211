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

The original group repository is private; this case study summarizes the project without redistributing group source code.

## College Football Outcome Predictor

**CMSE 201 — Computational Modeling and Data Analysis I | Fall 2024 | Individual project**

### Objective
Investigate which offensive, defensive and turnover statistics are associated with college football outcomes and compare two classification models.

### Methods
- Prepared a binary win target from 2023 season win-loss data.
- Used numerical features to compare logistic regression and decision tree classifiers.
- Evaluated accuracy, precision and recall with Python, pandas, scikit-learn and Matplotlib.

### Results reported in the original December 2024 presentation

| Model | Accuracy | Precision | Recall |
| --- | ---: | ---: | ---: |
| Logistic regression | 78% | 88% | 89% |
| Decision tree | 73% | 75% | 74% |

The presentation identifies nonstandard win-loss entries as a data-cleaning challenge and possible decision tree overfitting. These are the original reported metrics, not newly reproduced results. The original code and split have not been rechecked, and season-level statistics may contain information unavailable before a game. A future version would use pregame features and chronological validation.

### Data sources
- [CollegeFootballData](https://collegefootballdata.com/)
- [College Football Team Stats Seasons 2013 to 2023 (Kaggle)](https://www.kaggle.com/datasets/jeffgallini/college-football-team-stats-2019)
- [scikit-learn](https://scikit-learn.org/)

[Back to portfolio](README.md)
