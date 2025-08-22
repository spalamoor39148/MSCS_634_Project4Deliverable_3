# MSCS_634_Project4Deliverable_3
## Overview

This project explores classification, clustering, and association rule mining techniques to analyze data, uncover hidden patterns, and evaluate model performance. The workflow involved building machine learning models, tuning hyperparameters, and interpreting results with visualizations.

## Classification Models

Decision Tree Classifier

Trained with default parameters and pruned for interpretability.

Key features influencing predictions were identified using feature importance.

Support Vector Machine (SVM)

Applied with kernel optimization and hyperparameter tuning (GridSearchCV).

Improved generalization compared to the Decision Tree, especially for non-linear data boundaries.

Hyperparameter Tuning

Grid search was applied on SVM with parameters such as C, gamma, and kernel.

The best model achieved higher accuracy and F1 score after tuning.

## Evaluation

Confusion Matrix highlighted correct vs. misclassified samples.

ROC Curve & AUC showed strong separability for tuned SVM.

Accuracy and F1-score confirmed that SVM outperformed Decision Tree.

## Clustering

Implemented K-Means Clustering.

The Elbow Method and Silhouette Score were used to determine the optimal number of clusters.

Visualizations revealed well-separated groups, providing insights into natural segmentations in the data.

Insights:

Clusters corresponded to groups with similar characteristics (e.g., demographic similarity, product usage patterns).

These groupings could support customer segmentation, targeted marketing, or anomaly detection.

## Pattern Mining

Applied Apriori algorithm to extract frequent itemsets.

Association rules generated with metrics: support, confidence, and lift.

Key Findings:

Strong associations were discovered (e.g., items frequently purchased together).

Lift > 1 indicated non-random co-occurrence patterns.

Applications:

Market Basket Analysis – identifying products often bought together.

Recommendation Systems – suggesting complementary items to users.

## Practical Relevance

Business: Customer segmentation and product bundling opportunities.

Healthcare: Classification models can aid in diagnosis prediction.

E-commerce: Rule mining enables cross-selling and personalized recommendations.

## Challenges & Solutions

Data Preprocessing

Issue: Non-binary values in association rule mining caused errors.

Solution: Converted categorical variables into one-hot encoded (0/1) format.

Class Imbalance

Issue: Some classes were underrepresented, skewing results.

Solution: Used F1-score and ROC-AUC instead of just accuracy.

Hyperparameter Complexity

Issue: SVM training was computationally expensive.

Solution: Used grid search with a reduced parameter space and cross-validation.

Deprecation Warnings in Jupyter

Issue: Warnings from datetime.utcnow() cluttered output.

Solution: Suppressed irrelevant warnings with warnings.filterwarnings.

## Visualizations Included

Confusion Matrix heatmaps.

ROC Curves for classification models.

Cluster scatterplots with K-Means.

Bar plots of frequent itemsets and rules (Apriori).

## Conclusion

This deliverable demonstrated the power of supervised learning, unsupervised learning, and pattern mining in extracting valuable insights from data. The models and rules identified can be adapted for real-world decision-making in retail, healthcare, and business strategy.
