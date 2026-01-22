# Weighted-Likelihood Naive Bayes for Cancer Diagnosis
**Authors:** Rishi Pathuri & Arjun Nadakuduru  
**Course:** Machine Learning 1 (TJHSST)  
**Date:** January 2026

## Project Overview
This project addresses the feature independence assumption of Naive Bayes, which is often violated in medical datasets. We propose a **Weighted-Likelihood Gaussian Naive Bayes** that assigns a "Relevance vs. Redundancy" weight ($\alpha$) to each feature.

Using the **UCI Breast Cancer Wisconsin (Diagnostic)** dataset, our model improves Recall and F1-Score by explicitly penalizing redundant features (e.g., Radius, Perimeter, and Area) while amplifying unique signals.

## Key Results
| Metric | Standard NB | Weighted NB (Ours) |
| :--- | :--- | :--- |
| **Accuracy** | 92.97% | **94.20%** |
| **Recall** | 89.16% | **89.62%** |
| **F1-Score** | 90.45% | **91.97%** |

## Repository Contents
* **`/code`**: Python implementation of the `DependencyWeightedNB` class and cross-validation scripts.
* **`/paper`**: The final IEEE-format project report (PDF & LaTeX source).
* **`/presentation`**: The slide deck used for the class presentation.

## Usage
To run the analysis:
1. Install dependencies: `pip install pandas numpy seaborn scikit-learn matplotlib`
2. Run the script: `python code/weighted_nb.py`

## References
* UCI Machine Learning Repository: Breast Cancer Wisconsin (Diagnostic)
* Scikit-Learn Documentation
