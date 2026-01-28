# Predicting Earthquake Significance

This project explores how **earthquake magnitude, location, and tsunami occurrence** relate to the overall **significance** of an earthquake. The goal is to model these relationships using a **Bayesian Network** and analyze what factors contribute most to severe earthquake impacts.

## Dataset

The dataset comes from Kaggle: **The Ultimate Earthquake Dataset (1990–2023)**.

Key features used:
- **Magnitude** – strength of the earthquake  
- **Significance** – impact score (0–2910)  
- **State / Region** – geographic location  
- **Tsunami** – whether a tsunami occurred  

Data preprocessing included filtering non-earthquake events, cleaning noisy location names, removing missing values, and discretizing continuous variables.

## Methodology

- Cleaned and standardized earthquake records  
- Discretized magnitude and significance into bins  
- Built Bayesian Networks with fixed DAG structures  
- Learned conditional probability tables using **Maximum Likelihood Estimation (MLE)**  
- Analyzed learned probability distributions qualitatively

## Results

- Earthquake significance increases monotonically with magnitude  
- Tsunami occurrence significantly amplifies earthquake severity  
- The **Full DAG** better captures catastrophic events, especially in coastal regions  
- Geographic location plays an important role in determining impact

## Files

- `significance of earthquakes.ipynb` – main notebook containing preprocessing, modeling
