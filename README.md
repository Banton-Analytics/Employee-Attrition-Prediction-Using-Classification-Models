# Employee-Attrition-Prediction-Using-Classification-Models

#### Objective:
The goal of this project is to develop a classification model that predicts whether an employee will leave (attrition) or stay with the organization. By analyzing various employee characteristics, the project aims to identify key factors influencing attrition and provide insights to help the organization reduce turnover and retain talent.

#### Dataset:
The dataset used is a synthetic HR dataset from IBM, containing information on employees across various features, such as:
- [x] Attrition: Target variable indicating whether an employee left (Yes) or stayed (No).
- [x] Age, Monthly_Income, Job_Role, and many others: Various features describing employee demographics, job characteristics, and personal details.

The dataset consists of 35 features, but for this project, a subset of 14 features was used.

#### Methodology

#### Data Exploration
   - [x] Descriptive Statistics: Initial exploration to understand the dataset's structure and feature distributions.
   - [x] Visualization: A histogram was plotted to visualize the distribution of the target variable (Attrition), revealing that the majority of employees did not leave the organization.

#### Data Preprocessing
   - [x] Feature Selection: 14 relevant features were selected for the analysis, and the target variable was dropped from the feature set.
   - [x] Train-Test Split: The dataset was split into 50% training and 50% testing data to evaluate the model's performance on unseen data.

#### Model Building
   - [x] Classifiers Used: Five different classifiers were implemented:
     - Gaussian Naive Bayes (NB)
     - Support Vector Machine (SVM)
     - K-Nearest Neighbors (KNN)
     - Decision Tree (DT)
     - Random Forest (RF)
   - [x] Training: Each classifier was trained on the training data and tested on the test data.

#### Model Evaluation
   - [x] Metrics Used:
     - Accuracy: Proportion of correct predictions.
     - Precision: Ratio of true positive predictions to total positive predictions.
     - Recall: Ratio of true positives to actual positives.
     - F₁ Score: Harmonic mean of precision and recall.
     - F₂ Score: Similar to F₁ but gives more weight to recall.

#### Summary of Classifier Performance
- [x] Accuracy
Classifier_NB (Naive Bayes) and classifier_RF (Random Forest) have the highest accuracy 85.85% and 85.17% respectively, indicating they are most effective at correct classification.
- [x] Precision
Classifier_RF has the highest precision 87.38%, indicating it is more conservative and precise in predicting the positive class.
- [x] Recall
Classifier_NB and classifier_SVM performed well in this area, 85.85% and 84.76% respectively showing they are effective at identifying most of the positive instances.
- [x] F₁ Score
Classifier_SVM achieves the highest F₁ score 91.75%, suggesting it best balances precision and recall.
- [x] F₂ Score
Classifier_NB performs best here 85.68%, indicating it is particularly good at minimizing false negatives.

#### Conclusion
- Naive Bayes (classifier_NB): Consistently performs well across all metrics, making it a strong overall performer, especially for cases where recall is critical.
- Support Vector Machine (classifier_SVM): Although it has the lowest precision, it has the highest F₁ score, indicating a good balance between precision and recall. This makes it a strong choice for scenarios where this balance is important.

#### Future Work
- Feature Engineering: Explore additional features or transformations that could improve model accuracy.

- Ensemble Methods: Explore combining multiple classifiers to enhance prediction accuracy.
