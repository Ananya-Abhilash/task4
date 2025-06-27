# Task 4: Classification with Logistic Regression

## 🎯 Objective
Build a binary classification model using Logistic Regression to distinguish between malignant and benign tumors using the Breast Cancer Wisconsin dataset.

---

## 🧰 Tools Used
- **Pandas**: For data loading and manipulation  
- **NumPy**: For numerical operations  
- **Scikit-learn**: For preprocessing, model training, and evaluation  
- **Matplotlib & Seaborn**: For data visualization  

---

## 📂 Steps Followed

### 1. Dataset Loading
- The dataset was loaded from a CSV file named `data.csv` which contained the dataset 'Breast Cancer Wisconsin (Diagnostic) Data Set'.
- Irrelevant columns such as `id` and an empty column `Unnamed: 32` were dropped for clarity.

### 2. Target Label Encoding
- The `diagnosis` column was mapped to binary values:
  - `M` (Malignant) → 1  
  - `B` (Benign) → 0

### 3. Feature and Target Separation
- Features (independent variables) and the target label (`diagnosis`) were separated for model training.

### 4. Data Cleaning
- The dataset was scanned for missing (`NaN`) and infinite values.
- These invalid entries were either removed or replaced.
- Ensured that the number of samples in features and labels matched after cleaning.

### 5. Train-Test Split
- The dataset was split into training and testing sets using a 90-10 split.
- A fixed random state was used for reproducibility.

### 6. Feature Scaling
- Standardization was applied using `StandardScaler` to ensure all features have zero mean and unit variance.
- This improves model performance and convergence.

### 7. Model Training
- Logistic Regression was used as the classifier.
- The model was trained on the scaled training dataset.

### 8. Model Evaluation
- The trained model was evaluated on the test dataset using:
  - **Confusion Matrix**: To visualize actual vs predicted classes.
  - **Accuracy**: Proportion of correct predictions.
  - **Precision**: Correctly predicted positives out of all predicted positives.
  - **Recall**: Correctly predicted positives out of all actual positives.
  - **ROC-AUC Score**: Ability of the model to distinguish between classes.

### 9. Visualization
- Plotted the Confusion Matrix as a heatmap.
- Plotted the ROC Curve to assess performance across thresholds.
- Plotted the Sigmoid function to illustrate how logistic regression models output probabilities.

---

## ✅ Final Outcome
- Successfully built a logistic regression model capable of classifying tumors as malignant or benign.
- Performed complete preprocessing, cleaning, training, and evaluation.
- Visualizations and metrics confirmed the model's effectiveness on real-world medical data.

