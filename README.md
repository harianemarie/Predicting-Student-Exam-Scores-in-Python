# Predicting Student Exam Scores

A regression problem: predicting an exam score out of 100 from study habits, personal
characteristics and educational context. Four algorithms are compared on identical
inputs, then one is taken through feature engineering, variable selection and
hyperparameter tuning to see how far it can be pushed.

The project ends where most modelling exercises stop short — on whether a model like this
should be used at all. See [Ethics](#ethics) below.

## Data

TODO — state the source, the number of students and the variables available.

## Models compared

Ordinary least squares, polynomial regression, piecewise/spline regression and a random
forest, all fitted on the same explanatory variables.

| Model | R² (test) | MSE (test) | Training time | Main hyperparameters |
|---|---|---|---|---|
| OLS | | | | |
| Polynomial | | | | |
| Spline | | | | |
| Random forest | | | | |

## Optimisation

**Feature engineering.** Three new variables built from the originals, each justified by
exploratory analysis rather than by trial and error. TODO — name them and say what each
is meant to capture; this is the part that shows judgement rather than technique.

**Variable selection.** Test error tracked across different combinations of inputs.

**Hyperparameters.** For two models, the key hyperparameters identified and tuned, with
test error plotted across the grid.

## Selected model

TODO — which model and why. Reported with R² on both the training and the test set, so
the gap between them is visible, and a predicted-versus-actual scatter plot.

Known weaknesses: TODO. Worth being specific — where in the score range the model drifts,
which students it systematically misses.

## Ethics

Three questions the project takes seriously rather than treating as an appendix:

- Should universities use a model like this to select applicants?
- Should students be told their predicted score?
- Should the model's variables be used to design interventions supporting student success?

TODO — summarise the position taken. The distinction between using a model to *understand*
what helps students and using it to *sort* them is where the argument lives.

## Repository

```
exam-score-regression/
├── analysis.py         # commented script
├── data/
├── figures/            # error curves, predicted vs actual
└── report.pdf
```

Python. TODO — list the libraries (scikit-learn, pandas, …).

## Context

Machine Learning, project 1 — Aix-Marseille University, Master in Economics (M1),
2025–2026. Group project.
