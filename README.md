# Final-Project-Jace-M# Food Safety Risk Signals
### Montgomery County, Maryland · BUS 446 Business Analytics

**A public-health analytics case study about what inspection history can—and cannot—tell us.**

**Team:** Maxwell Blanc · Jace Miller · Ryan Winkler · Mikey Vang  
**Study period:** October 2022–October 2024  
**Tools:** Tableau · Microsoft Excel · Logistic regression

---

## The question
A health department has more places to inspect than it can visit at once. Can inspection history, facility type, and specific compliance checks help prioritize attention toward the locations most likely to need intervention?

This repository takes the reader through the analysis in five connected chapters. Each chapter provides its own quick-start notes and relevant files.

## The risk in numbers

| Indicator | Team-reported finding |
|---|---:|
| Establishments studied | 4,160 |
| Adverse outcomes | About 31% |
| Restaurants: adverse-outcome rate | 36.2% |
| Cold-holding noncompliance | 19.9% |
| Rodent and insect noncompliance | 15.5% |
| Prior adverse result: odds ratio | 2.41 |
| Model overall accuracy at 0.50 | About 70% |
| Model false-negative rate at 0.50 | 82.4% |

> **Why the last two numbers matter:** A model can report respectable overall accuracy while failing to identify most adverse inspections. In food safety, overlooked risks carry consequences; sensitivity and review capacity need attention alongside accuracy.

## Three findings that shape the recommendations

**Facility category matters.** In the team's analysis, public middle schools (40.5%), restaurants (36.2%), and carry-out locations (33.2%) showed high observed adverse-outcome rates. Those descriptive comparisons depend on the composition of inspections.

**Two safety issues stand out.** Cold holding (19.9%) and rodent/insect conditions (15.5%) were the leading reported noncompliance issues. Cold-holding issues were more common during summer.

**History adds a signal, but model performance needs context.** A prior adverse inspection was associated with an odds ratio of roughly 2.41. The model's reported false-negative rate at a 0.50 cutoff, however, argues for threshold analysis before real-world deployment.

## From analysis to action
1. Prioritize timely follow-ups for establishments with previous adverse outcomes.
2. Focus seasonal prevention on refrigeration and ongoing pest-management checks.
3. Evaluate a 0.30 dispatch threshold **as a proposal**, checking sensitivity, false positives, and inspector capacity before adoption.

## Data provenance and reproducibility

- **Source:** [Montgomery County Food Inspection dataset via Data.gov](https://catalog.data.gov/dataset/food-inspection)
- The team's final report describes **11,854** records, but the supplied cleaned Excel worksheet contains **11,835 data rows**. These counts should be reconciled before making a final exact-sample claim.
- The adverse-outcome label is a project-created binary grouping (corrected critical violations or closure), not an official government pass/fail designation.
- Original Tableau `.twb` files can need a data-source reconnection to the local cleaned workbook.
- The predictive model's reported associations do not imply causation, and this is not a validated enforcement tool.

*Prepared as an educational business analytics project. Analysis and figures are attributed to the student team.*
