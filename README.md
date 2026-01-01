# ML Journey 2025

This repository contains my Machine Learning learning journey.
Day-wise notebooks, code, and practical examples are included.

Week 1: Python & Math Intuition
Project: Statistical Analysis Toolkit

Goal: Learn Python for ML pipelines and gain math intuition for ML. Apply knowledge on a CSV dataset to explore, analyze, and visualize key statistics.

1️⃣ Overview

This project demonstrates:

Python skills for ML pipelines

Math intuition (gradient descent, bias-variance, probability)

Exploratory Data Analysis (EDA) and statistical insights

Practical, reproducible workflows for data analysis

All work is performed using Jupyter Notebook in a conda environment with libraries: pandas, numpy, matplotlib, seaborn, scikit-learn.

2️⃣ Tools & Environment

Conda environment: ml-env

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

Editor: VS Code (Python, Jupyter, GitHub Copilot extensions)

Version control: Git + GitHub

Repository: ml-journey-2025

.gitignore: excludes notebooks outputs, datasets, models

3️⃣ Python for ML Pipelines
Key Concepts Applied:

Lambda functions: Quick, inline data transformations for custom metrics.

List/Dict comprehensions: Efficient feature transformations.

Generators: Batch-wise data processing for memory efficiency.

Decorators: Logging and timing function execution for debugging.

Type hints: Production-ready Python code.

Example:

# Custom lambda metric
df.groupby("Survived")["Age"].agg(lambda x: x.max() - x.min())

4️⃣ Math Intuition for ML

Gradient Descent: Iteratively updates weights to minimize loss.

Loss Surfaces: Convex (single minimum) vs non-convex (multiple minima).

Probability Distributions:

Normal → Continuous features

Binomial → Classification outcomes

Bias-Variance Tradeoff: Visual simulation shows underfitting (high bias), optimal fit, and overfitting (high variance).

📌 Tip: Diagrams are included in notebook to visualize gradient steps and bias-variance tradeoff.

5️⃣ Exploratory Data Analysis (Practical)

Performed on Titanic dataset (or any CSV dataset):

a) Distribution Plots

Histograms & KDE: Continuous features (Age, Fare)

Count plots: Categorical features (Survived, Parch)

b) Outlier Detection

IQR method: Values outside 1.5×IQR flagged

Z-score method: Values beyond ±3 standard deviations flagged

c) Correlation Heatmap

Shows relationships between numerical features

Helps identify potential predictors and redundant features

d) Insights Extracted

Children had higher survival probability

Elderly passengers had lowest survival probability

Higher passenger class had higher survival rate

Certain features (e.g., Fare, Pclass) strongly correlated

e) Technical Twist

Custom metrics calculated using lambda functions

Type hints applied for all functions in notebook

6️⃣ How to Run

Clone repo:

git clone https://github.com/yourusername/ml-journey-2025.git


Create conda environment:

conda create -n ml-env python=3.10
conda activate ml-env
pip install -r requirements.txt


Open Jupyter Notebook and run Week1_StatisticalAnalysis.ipynb.

7️⃣ Key Learning Outcomes

Mastered Python functional tools for ML pipelines

Built gradient descent & bias-variance intuition

Applied EDA techniques to real-world dataset

Learned outlier detection, feature distribution, and correlation analysis

Practiced lambda functions, comprehensions, decorators, generators

Developed production-ready Python skills

8️⃣ Interview Preparation Mapping
Concept	Practical Example	How to Explain in Interview
Bias-Variance	Simulation plot	Explain underfitting vs overfitting visually
Gradient Descent	Numpy linear regression	Explain iterative loss minimization
Lambda Functions	Custom groupby metrics	Quick transformation without defining full function
Count/Hist/KDE plots	Titanic dataset	Explain feature distributions and insights
Outlier Detection	IQR/Z-score plots	Explain method and visualization for detecting anomalies