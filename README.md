# Analytics_Capstone_Project

### Targeted Problem:
##### How can we construct an effective predictive framework for distinguishing students likely to succeed academically from those at risk of dropping out in educational institutions. 

### Research Question:
##### What strategies and techniques can be effectively employed to achieve precise predictions regarding students at risk of dropout and those on track for academic success?

### Dataset:
##### A dataset created from a higher education institution (acquired from several disjoint databases) related to students enrolled in different undergraduate degrees, such as agronomy, design, education, nursing, journalism, management, social service, and technologies. The dataset includes information known at the time of student enrollment (academic path, demographics, and social-economic factors) and the students' academic performance at the end of the first and second semesters. The data is used to build classification models to predict students' dropout and academic sucess. The problem is formulated as a three category classification task, in which there is a strong imbalance towards one of the classes.

### Methodology:
##### Data Balancing:
##### Address class imbalances using techniques like SMOTE, SMOTEENN, or ADASYN to create a more balanced dataset.
##### Experiment with different balancing methods to evaluate their impact on model performance.
##### Model Selection and Training:
##### Implement a variety of machine learning algorithms, including Random Forest, Gradient Boosting, Logistic Regression, and Neural Networks.
##### Split the dataset into training, validation, and test sets for model training and evaluation.
##### Apply hyperparameter tuning techniques like grid search or Bayesian optimization to optimize model performance.
##### Evaluation Metrics and Interpretability:
##### Utilize a range of evaluation metrics such as accuracy, precision, recall, F1-score, and area under the ROC curve (AUC-ROC) to assess model performance.
##### Conduct SHAP (SHapley Additive exPlanations) analysis to interpret the model predictions and understand the impact of individual features on outcomes.
##### Use confusion matrices to understand prediction errors and identify areas of improvement. 
##### Model Fine-Tuning:
##### Fine-tune the selected models based on SHAP analysis and other evaluation results.
##### Experiment with ensemble techniques to combine the strengths of multiple models for more robust predictions.

### Results:
##### The performance of six machine learning algorithms—Logistic Regression, SVM, Decision Tree, Naive Bayes, Random Forest, and XGBoost-was assessed for a classification task. Initial evaluation without hyperparameter tuning revealed varied performance metrics. Notably, Random Forest outperformed others with an accuracy of 90.42%, precision of 89.10%, recall of 95.55%, and F1 score of 92.21%. Subsequently, hyperparameter tuning using GridSearchCV for the Random Forest model. This refinement resulted in a marginal improvement, maintaining the accuracy at 90.42% while enhancing precision, recall, and F1 scores to 89.10%, 95.55%, and 92.21%, respectively. These findings highlight the initial strength of Random Forest and the limited impact of hyperparameter tuning on its performance in this specific classification task. Using  SHAPley, the Circular units of 1st and 2nd semester have the most impact on the ML model.

### Conclusion:
##### The study investigated the use of machine learning (ML) tools to predict the academic performance of first-year computer science (CS) students and identify key factors affecting their success. It found that Random Forest classifiers were effective in this prediction task. While previous work centered on GPA-based performance prediction, focusing on academic probation status allows for aiding struggling students beyond just those with low grades.


