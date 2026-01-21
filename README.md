Assignment 2: Sampling Techniques Analysis
1. Objective
The goal of this assignment is to address class imbalance in a credit card dataset and evaluate the impact of various sampling strategies on the performance of different machine learning models.

2. Methodology

Balancing: The original imbalanced dataset was converted into a balanced dataset using SMOTE (Synthetic Minority Over-sampling Technique) to ensure equal representation of classes.


Sampling Techniques: Five different sampling strategies were implemented:

Simple Random Sampling: Randomly selecting a subset of the balanced data.

Systematic Sampling: Selecting records at a fixed interval.

Stratified Sampling: Maintaining the class distribution within the sample.

Cluster Sampling: Dividing data into clusters and selecting a random group.

Bootstrap Sampling: Sampling with replacement.


Machine Learning Models: Performance was evaluated across five models: Logistic Regression (M1), KNN (M2), SVM (M3), Decision Tree (M4), and Random Forest (M5)

3. Accuracy Result Table (%)
The following table summarizes the accuracy achieved by each model for every sampling technique


Sampling Technique,  M1_LogReg,  M2_KNN,    M3_SVM,  M4_DecTree,M   5_RanForest
Sampling1_Random,       92.58,    92.58,      95.20,     96.07,       98.25
Sampling2_Systematic,   88.28,    89.06,      89.84,     99.22,       100.00
Sampling3_Stratified,   91.70,    93.89,      92.14,     97.38,       98.69
Sampling4_Cluster,      97.83,    97.83,      97.83,     97.83,       97.83
Sampling5_Bootstrap,    92.15,    97.64,      93.46,     97.91,       99.21

<img width="1168" height="287" alt="Screenshot 2026-01-21 at 10 57 50 PM" src="https://github.com/user-attachments/assets/e79100be-30c2-4dad-8b0c-2476f30f65c1" />


4. Result Visualization
The visual representation of the model performance is saved in the repository as sampling_results_graph.png.


<img width="1090" height="550" alt="Screenshot 2026-01-21 at 10 55 31 PM" src="https://github.com/user-attachments/assets/9b0fce8f-4281-4e69-8971-2eb6bbf80240" />




6. Discussion & Conclusion

Best Model: Random Forest (M5) emerged as the most robust model, achieving a perfect accuracy of 100.00% with Systematic Sampling.


Best Sampling Strategy: While results varied, Cluster Sampling provided the most consistent performance (97.83%) across all models in this specific implementation.


Final Determination: Using SMOTE for balancing provided a more generalized training set, leading to highly reliable results compared to standard oversampling.
