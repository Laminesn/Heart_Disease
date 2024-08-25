Heart Disease Classification Using Logistic Regression, Decision Trees, and XGBoost

### **Heart Disease Classification**

1. **Data Preparation and Pairplot Analysis**
   - **Column Handling and Cleanup:**
     - Parsed column headers and loaded the dataset into a DataFrame.
     - Identified and removed rows containing non-numeric values.
     - Converted all data to numeric types, ensuring consistency for model training.
   - **Feature Selection and Visualization:**
     - Selected the 14 main features for analysis, focusing on potential correlations with heart disease.
     - Created pairplots to visualize relationships between features and output labels.
     - Observed strong relationships between features like age, thalach, and oldpeak, which guided feature importance in later analysis.
   - **Results:**
     - Discovered significant correlations, particularly age with oldpeak and thalach, highlighting their importance in predicting heart disease.
   
2. **Model Training and Evaluation**
   - **Classifier Comparison:**
     - Implemented and compared five classifiers: Naive Bayes, Logistic Regression, LDA, QDA, and K-Nearest Neighbors using the same train/test split.
     - Calculated accuracy and confusion matrices for each model, evaluating performance on the test set.
     - Plotted confusion matrices to visualize classification effectiveness.
   - **Decision Tree Implementation and Pruning:**
     - Trained a Decision Tree classifier and evaluated its accuracy on the test set.
     - Performed cost-complexity pruning to simplify the tree while maintaining high validation accuracy.
     - Visualized the pruned decision tree, analyzing intuitive and non-intuitive aspects of the decision-making process.
   - **Results:**
     - Logistic Regression achieved the highest accuracy at 66.67%, with the Decision Tree accuracy improving post-pruning to 60.00%.
     - Key features such as `ca`, `thal`, and `thalach` were consistently important across different models, underscoring their practical significance.
