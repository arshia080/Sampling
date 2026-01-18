# Sampling Assignment – Credit Card Fraud Analysis

## Objective
The objective of this assignment is to analyze how different sampling techniques affect the performance of machine learning models on an imbalanced dataset.

## Dataset
The dataset Creditcard_data.csv contains records of credit card transactions(Class = 0 → Normal transaction,Class = 1 → Fraud transaction).
The number of fraud cases is very small compared to normal cases, making the dataset highly imbalanced.

## Data Preprocessing
To handle class imbalance, the dataset was balanced using random undersampling.
The majority class was reduced so that both classes had an equal number of samples.

## Sampling Methods
The following sampling approaches were applied on the balanced dataset:
-Simple Random Sampling
-Systematic Sampling
-Stratified Sampling
-Cluster Sampling
-Bootstrap Sampling
Each method produced a separate dataset for model training.

## Models Applied
The following machine learning models were used:
-M1: Logistic Regression
-M2: Decision Tree
-M3: Random Forest
-M4: K-Nearest Neighbors
-M5: Support Vector Machine

## Methodology
1. The dataset was first balanced using random undersampling.
2. Five different sampling techniques were applied to the balanced dataset.
3. Each sampled dataset was divided into training and testing sets.
4. Five machine learning models were trained on each sampled dataset.
5. Model performance was evaluated using accuracy.
6. The results were stored in a comparison table for analysis.

## Result Table
| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
| ----- | --------- | --------- | --------- | --------- | --------- |
| M1    | 100.00    | 33.33     | 75.00     | 20.00     | 83.33     |
| M2    | 50.00     | 0.00      | 75.00     | 20.00     | 83.33     |
| M3    | 100.00    | 0.00      | 75.00     | 20.00     | 66.67     |
| M4    | 100.00    | 33.33     | 25.00     | 40.00     | 50.00     |
| M5    | 100.00    | 33.33     | 100.00    | 40.00     | 66.67     |

## Result Visualization
A bar chart is generated using the average accuracy of all models for each sampling technique.
The plot is saved as results.png for reference.

## Observations
1. Model accuracy varies significantly across different sampling techniques.
2. Very small samples (Sampling1) show high accuracy for most models, which may not be reliable.
3. Sampling2 results in poor performance for most models.
4. Sampling3 performs well for Logistic Regression, Decision Tree, Random Forest, and Support Vector Machine.
5. Sampling4 shows consistently low accuracy across all models.
6. Sampling5 provides more stable and balanced performance compared to smaller samples.

## Conclusion
This assignment shows that sampling techniques have a strong impact on model performance when working with imbalanced data.
Balancing the dataset before sampling helps in fair comparison of machine learning models.


