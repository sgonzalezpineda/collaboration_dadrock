---
title: Use an 80-20 train-test split
status: accepted
id: 01a1d0b1-6dd5-70f1-9885-1a8b630e9859
---

## Context
We need to evaluate how well our model predicts unseen observations.

## Decision
Randomly allocate 80% of observations to training and 20% to testing, using a fixed random seed.

## Alternatives
A 70–30 split would provide a larger test set but fewer training observations.

## Consequences
Fit and tune models using only the training data; reserve the test data for final evaluation.
