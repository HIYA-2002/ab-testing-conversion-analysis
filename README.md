A/B Testing Analysis for Conversion Rate Optimization

📌 Project Overview

This project presents an end-to-end statistical analysis of an A/B test conducted to evaluate whether a new landing page (Treatment) improves user conversion rate compared to the existing version (Control).

The objective was to use statistical methods to determine whether the Treatment version should be deployed.

🎯 Business Problem

A new landing page design was introduced with the goal of increasing user conversion rate.

The key question:

Does the Treatment version significantly improve conversion rate compared to the Control version?

The primary metric evaluated was conversion rate (binary outcome: converted / not converted).

🧪 Hypothesis Formulation

Since the objective was to test for improvement, a one-sided hypothesis test was conducted.

Null Hypothesis (H₀): Treatment conversion rate ≤ Control conversion rate

Alternative Hypothesis (H₁): Treatment conversion rate > Control conversion rate

The direction of the test was defined prior to analysis, aligning with the business objective of detecting improvement before deployment.

🛠 Methodology

The analysis included:

Data preprocessing and validation

Calculation of conversion rates for Control and Treatment groups

Absolute and relative lift calculation

Two-proportion Z-test to evaluate statistical significance

95% confidence intervals for conversion rates

Chi-square test of independence

Segmentation analysis across clusters

Statistical significance was evaluated at a 95% confidence level (α = 0.05).

📊 Results

Conversion rates were calculated for both groups.

Absolute and relative lift were computed.

The two-proportion Z-test returned a p-value greater than 0.05.

Confidence intervals for Control and Treatment overlapped.

Chi-square test also indicated no statistically significant difference.

At the 95% confidence level, there was insufficient statistical evidence to conclude that the Treatment version outperformed the Control version.

💼 Business Decision

Since no statistically significant improvement was detected, the recommendation was to retain the Control version.

Although minor differences were observed, they were not statistically significant and therefore do not justify deployment based on current evidence.

The analysis highlights the importance of evaluating both:

Statistical significance

Practical (business) significance

before making rollout decisions.

🔍 Segmentation Insight

Segment-level analysis (cluster-based) was conducted using a Chi-square test to evaluate variation in conversion behavior across groups.

No strong evidence suggested a significant improvement within specific clusters, reinforcing the decision not to deploy the Treatment variant.

📚 Key Learnings

Proper statistical testing is essential before product deployment.

Large sample sizes can detect small differences that may not be practically meaningful.

One-sided tests must align with predefined business objectives.

Confidence intervals provide additional context beyond p-values.

Segmentation analysis helps prevent overgeneralization.

🧰 Tools & Technologies

Python

Pandas

NumPy

SciPy

Statsmodels

Matplotlib

Seaborn

Jupyter Notebook
