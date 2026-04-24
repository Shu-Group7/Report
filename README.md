Student Depression Prediction using Machine Learning


🔹 Part A: Introduction

Mental health issues among students have become a significant global concern, with increasing academic pressure, financial stress, and lifestyle factors contributing to depression. Early detection of depression is critical to provide timely support and prevent severe consequences such as academic failure or self-harm.

This project aims to develop a machine learning-based system that predicts whether a student is likely to be depressed based on multiple factors such as academic performance, lifestyle habits, and psychological indicators.

The importance of this problem lies in:

Supporting early intervention in educational institutions
Reducing stigma through data-driven insights
Assisting counsellors and decision-makers

By leveraging data science techniques, this project contributes to building intelligent systems for mental health prediction.

🔹 Part B: Technical Review (LO1)

This project explores several data science and AI techniques relevant to classification problems:

1. Supervised Learning

The problem is formulated as a binary classification task (Depressed vs Not Depressed). Supervised learning models learn patterns from labelled data.

2. Logistic Regression

A statistical model used for binary classification. It provides:

Interpretability
Baseline performance

However, it may struggle with complex non-linear relationships.

3. Random Forest

An ensemble learning method that:

Combines multiple decision trees
Reduces overfitting
Handles non-linear relationships effectively

It is widely used for structured/tabular datasets and was selected as the primary model.

4. Data Preprocessing Techniques
Handling missing values (median/mode imputation)
Encoding categorical variables using Label Encoding
Feature scaling using StandardScaler
5. Evaluation Metrics

To assess model performance:

Accuracy → Overall correctness
Precision → Correct positive predictions
Recall → Ability to detect depressed students
F1-score → Balance between precision and recall

These metrics provide a comprehensive evaluation beyond accuracy.

🔹 Part C: Design & Implementation (LO2)
1. System Overview

The system follows a standard machine learning pipeline:

Data Collection → Preprocessing → Feature Engineering → Model Training → Evaluation → Prediction
2. Data Preprocessing

Key steps implemented:

Removed irrelevant columns (e.g., ID, Name)
Handled missing values:
Numerical → Median
Categorical → Mode
Converted categorical variables into numerical format using Label Encoding
3. Feature Selection

Input features include:

Academic Pressure
CGPA
Study Satisfaction
Sleep Duration
Financial Stress
Work/Study Hours
Family History of Mental Illness

Target variable:

Depression (0 = No, 1 = Yes)
4. Model Implementation

Two models were tested:

Logistic Regression
Used as baseline
Fast and interpretable
Random Forest (Final Model)
Better handling of complex relationships
Improved performance
5. Training Process
Data split: 80% training / 20% testing
Feature scaling applied using StandardScaler
Model trained using RandomForestClassifier
6. System Output

The system predicts:

“Depressed” or “Not Depressed” for new student data


🔹 Part D: Technical & Critical Evaluation (LO3, LO4)
✅ 1. Technical Evaluation
Performance Metrics
Metric	Value (Example)
Accuracy	~85–90%
Precision	High
Recall	Moderate–High
F1-score	Balanced
Confusion Matrix Analysis
True Positives: Correctly predicted depressed students
False Negatives: Missed depressed cases (critical issue)
False Positives: Over-prediction

👉 The model performs well overall but improving recall is important in mental health applications.

⚠️ 2. Limitations
Dataset size may be limited
Self-reported data may introduce bias
Model may not generalise to different populations
🌍 3. Ethical & Social Considerations
Bias
Dataset may not represent all demographics
Cultural differences in mental health reporting
Privacy
Sensitive personal data must be protected
Requires secure handling and anonymisation
Misuse Risk
Predictions should not replace professional diagnosis
Must be used as a support tool only
Responsible AI

This system should:

Be transparent
Avoid discrimination
Be used with human oversight


🔹 Part E: Project Proposal & Management
📊 1. Project Management
What Went Well
Clear problem definition
Successful implementation of ML pipeline
Effective use of VS Code and Python libraries
Challenges Faced
Data preprocessing complexities
Handling missing values
Model tuning and evaluation
Tools Used
Python
VS Code
GitHub (for version control)
🚀 2. Future Work

This project can be extended by:

Technical Improvements
Use advanced models (e.g., XGBoost, Neural Networks)
Hyperparameter tuning
Feature selection optimisation
Data Improvements
Larger and more diverse dataset
Real-time data collection
Deployment
Web application (Streamlit)
Integration with university systems
Research Extensions
Multi-class classification (mild/moderate/severe depression)
Integration with NLP (student feedback analysis)


🔹 Part F: Conclusion

This project successfully developed a machine learning system for predicting student depression using structured data. The Random Forest model achieved strong performance and demonstrated the effectiveness of data-driven approaches in mental health prediction.

The system highlights both the technical potential and ethical responsibilities of AI in sensitive domains. While the model performs well, its real-world use requires careful consideration of bias, privacy, and human oversight.

Overall, this project contributes to the application of AI in healthcare and education, offering a foundation for future intelligent mental health systems.
