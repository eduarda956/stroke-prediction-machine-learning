# Stroke Prediction Using Machine Learning

## Overview

This academic research project investigates the application of **Machine Learning techniques to stroke prediction**, using demographic, clinical, and lifestyle-related data.

The study follows the **CRISP-DM methodology** to explore stroke risk factors, prepare and analyze the dataset, and compare the performance of different classification algorithms.

The main objective is to investigate how predictive analytics can support the identification of individuals at increased risk of stroke, while addressing the challenges associated with imbalanced healthcare datasets.

## Research Objectives

- Explore demographic and clinical factors associated with stroke occurrence.
- Perform exploratory data analysis to identify patterns and correlations.
- Assess data quality and handle missing values.
- Apply the CRISP-DM methodology to structure the analytical process.
- Compare three Machine Learning classification algorithms.
- Evaluate predictive performance, particularly the ability to detect positive stroke cases.
- Identify limitations and opportunities for improving predictive models.

## Dataset

The study uses the **Stroke Prediction Dataset**, publicly available on Kaggle.

- **Observations:** 5,110
- **Attributes:** 12
- **Target Variable:** `stroke` (0 = No Stroke, 1 = Stroke)

The dataset contains information related to age, gender, hypertension, heart disease, average glucose level, BMI, smoking status, and other demographic characteristics.

**Dataset Source:** [Kaggle – Stroke Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)

## Methodology

The project follows the CRISP-DM framework, covering:

1. **Business Understanding:** Defining the stroke prediction problem.
2. **Data Understanding:** Exploring clinical and demographic attributes.
3. **Data Preparation:** Checking data consistency and handling missing values.
4. **Exploratory Data Analysis:** Investigating distributions, correlations, and stroke prevalence.
5. **Modeling:** Applying three classification algorithms.
6. **Evaluation:** Comparing classification metrics and analyzing the effects of class imbalance.

## Exploratory Data Analysis

The analysis examines relationships between stroke occurrence and several risk factors, including:

- Age
- Hypertension
- Heart disease
- Average glucose level
- Body Mass Index (BMI)
- Smoking habits
- Gender and occupation

The dataset presents a significant class imbalance, with approximately **4.87% of observations corresponding to stroke cases**.

This imbalance represents a major challenge for predictive modeling, as high overall accuracy does not necessarily indicate effective identification of positive cases.

## Machine Learning Models

Three classification algorithms were evaluated:

### 1. Random Forest
An ensemble learning method combining multiple decision trees to perform classification.

### 2. Logistic Regression
A statistical classification model used to estimate the probability of a binary outcome.

### 3. Naive Bayes
A probabilistic classifier based on Bayes' theorem, assuming conditional independence between features.

## Model Performance

The reported results are:

| Model | Accuracy | Stroke Recall |
|---|---:|---:|
| Random Forest | 94.27% | 4.0% |
| Logistic Regression | 95.15% | 0.4% |
| Naive Bayes | 89.80% | 30.5% |

Although Logistic Regression achieved the highest overall accuracy, its ability to identify positive stroke cases was extremely limited.

**Naive Bayes achieved the highest recall for the positive stroke class**, detecting 76 out of 249 stroke cases in the reported evaluation.

These findings highlight why class-specific recall and other appropriate metrics should be considered alongside accuracy when evaluating models trained on imbalanced healthcare datasets.

*Note: The reported evaluations are not fully identical across models; the paper explicitly reports stratified cross-validation for Naive Bayes. Results should therefore be interpreted with this limitation in mind.*

## Key Findings

- Age showed the strongest positive correlation with stroke occurrence among the variables examined.
- Hypertension, heart disease, and average glucose levels were also positively associated with stroke.
- The dataset's strong class imbalance substantially affected positive-case detection.
- High overall accuracy did not guarantee effective stroke identification.
- Naive Bayes demonstrated comparatively better sensitivity to stroke cases than the other two evaluated models.

## Limitations and Future Work

The research identifies several limitations, particularly the low representation of positive stroke cases and the need for more comprehensive and representative healthcare data.

Future improvements may include:

- Applying appropriate class-balancing techniques.
- Exploring more advanced models, including boosting and neural networks.
- Improving data representativeness.
- Developing a prototype to evaluate potential applications in clinical decision support.

## Conclusion

This project demonstrates both the potential and the limitations of Machine Learning in healthcare prediction.

The comparative analysis emphasizes that reliable predictive modeling depends not only on algorithm selection but also on data quality, class distribution, and appropriate evaluation metrics.

The study highlights the importance of developing models that can effectively identify clinically relevant cases rather than relying exclusively on overall classification accuracy.

## Academic Context

- **Institution:** Coimbra Business School — ISCAC
- **Degree:** Data Science for Management
- **Course:** Artificial Intelligence
- **Academic Year:** 2025/2026
- **Project Type:** Academic Research Project

## Authors

- Eduarda Correia
- Lara Veríssimo

**Academic supervision:** Prof.ª Doutora Dora Melo (as identified in the paper).

## Full Research Paper

[Read the full research paper (PDF)](stroke-prediction-research-paper.pdf)

## Keywords

Machine Learning · Stroke Prediction · Healthcare Analytics · CRISP-DM · Random Forest · Logistic Regression · Naive Bayes · Predictive Modeling
