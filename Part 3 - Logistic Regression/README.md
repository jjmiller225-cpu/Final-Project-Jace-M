# Part 3: Logistic Regression and Predictive Analysis

## Overview

This section focuses on the predictive portion of our project. After identifying patterns through Tableau, we used logistic regression in Microsoft Excel to explore whether certain characteristics could help predict adverse food inspection outcomes.

The objective was to determine which factors were most strongly associated with critical violations and evaluate how predictive analytics might assist with inspection planning.

## Model Development

Our logistic regression analysis considered several factors, including:

- Previous inspection performance
- Establishment category
- Inspection type
- Historical compliance patterns

## Key Results

The analysis identified previous inspection performance as an important predictor of future outcomes.

Establishments with a prior adverse inspection had approximately 2.41 times the odds of experiencing another adverse outcome.

Restaurants also demonstrated higher estimated odds of adverse outcomes, while reinspections were associated with lower odds.

The model achieved approximately 70% overall accuracy at a classification cutoff of 0.50. However, its reported false-negative rate was 82.4%, meaning many inspections with adverse outcomes were not correctly identified.

## Business Implications

Our findings suggest that predictive modeling could help health departments prioritize establishments requiring closer attention.

The team recommended evaluating a lower classification threshold of 0.30 to potentially improve the identification of high-risk establishments. Additional validation would be necessary before applying this approach in practice.

## File Included

- Logistic Regression.xlsx — Regression calculations, model outputs, and classification results
