## Objective
Implement SVMs for binary classification using both linear and RBF kernels, visualize decision boundaries, tune hyperparameters (`C` and `gamma`), and evaluate model performance using cross-validation.

---

## Tools & Libraries
- Python
- scikit-learn
- matplotlib
- numpy
- seaborn (optional, for visualization)

---

## Dataset Used
**Breast Cancer Dataset**  
Source: [Kaggle](https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset)

---

## Steps Followed

### 1. Load and Explore the Dataset
- Loaded Breast Cancer dataset into Pandas DataFrame.
- Checked for null values and data imbalance.

### 2. Preprocessing
- Performed Label Encoding on the `diagnosis` column.
- Split data into features (X) and target (y).
- Train-test split (80-20).

### 3. Feature Scaling
- Applied `StandardScaler` to normalize the feature set.

### 4. Model Training
- Trained **SVM with Linear Kernel**
- Trained **SVM with RBF Kernel**

### 5. Model Evaluation
- Used `confusion_matrix`, `classification_report`, and `accuracy_score` to evaluate both models.

### 6. Hyperparameter Tuning
- Used `GridSearchCV` to tune parameters:
  - `C` (regularization)
  - `gamma` (RBF kernel coefficient)

### 7. Cross-Validation
- Applied 5-fold cross-validation to avoid overfitting and validate performance.

---

## Results

| Model        | Accuracy |
|--------------|----------|
| SVM (Linear) | 95%      |
| SVM (RBF)    | 98%      |
| Best from GridSearch | 98% |
