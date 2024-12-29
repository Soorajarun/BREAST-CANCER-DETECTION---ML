# BREAST-CANCER-DETECTION-ML
Project Report:  Breast Cancer Detection
1. The objective: Developing an effective machine learning classification model to precisely identify breast cancer based on a variety of diagnostic criteria was the aim of this study. Preprocessing the data, identifying and managing outliers, choosing pertinent characteristics, and comparing several classification models in order to determine which one performed best were the objectives.
2. Dataset Description: The dataset includes diagnostic metrics like mean radius, mean area, and texture for breast cancer tumors. It has a target variable that indicates if the tumor is malignant (1) or benign (0).
Dataset Summary: Shape: Rows: ; Columns: Features: Numerical diagnostic features. Target Variable: Binary classification (0 = Benign, 1 = Malignant).
Data Quality:No missing values. No duplicate entries.
3. EDA
 Shape, description(), and info() were used to retrieve the most basic information. Statistical qualities such as mean, standard deviation, min, and max values were examined in the features. Identification and Handling of Outliers: To show outliers, boxplots were created for each feature separately and as a group. The Interquartile Range, or IQR, approach was used to find outliers. With the exception of the target variable, all features had outliers fixed via capping. Boxplots were redrew after capping to confirm the modifications.
Skewness: After checking, the skewness values were determined to be within acceptable bounds. To see feature distributions, histograms were plotted.
Analysis of Correlation:
To comprehend the connections between characteristics, a correlation heatmap was made. For some feature pairs, scatterplots were included (e.g., mean radius vs. mean area).
4. Data Preprocessing Feature Selection:
A correlation matrix was used to identify and select the most relevant features.
Feature Scaling: Applied MinMax Scaler to normalize features and bring them to a common scale.
Train-Test Split:The data was split into training and testing sets to evaluate model performance.
Model Building and Evaluation Five machine learning models were trained and evaluated:
Logistic Regression Decision Tree Classifier Random Forest Classifier Support Vector Machine (SVM) k-Nearest Neighbors (k-NN)
Performance Comparison:Logistic Regression: Accuracy = 0.9825 Decision Tree Classifier: Accuracy = 0.9211 Random Forest Classifier: Accuracy = 0.9561 SVM: Accuracy = 0.9825 k-NN: Accuracy = 0.9474
6. Model Optimization Hyperparameter Tuning: The Logistic Regression model was optimized using hyperparameter tuning techniques. Post-tuning, the model retained its high accuracy and robust performance metrics.
7. Model Deployment The tuned Logistic Regression model was saved for future use, ensuring it is ready for deployment in real-world scenarios.

8. Conclusion Key Findings:
Logistic Regression emerged as the best model with an accuracy of 98.25%. Outlier treatment and feature scaling significantly improved model performance. EDA and correlation analysis provided valuable insights into feature relationships. 
Impact:
The project demonstrates how machine learning can effectively detect breast cancer, aiding in early diagnosis and better treatment planning.

9. Future Work Experiment with advanced ensemble models like XGBoost or LightGBM. Perform further feature engineering, including interaction terms or polynomial features. Incorporate cross-validation for more robust performance evaluation.
