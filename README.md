# elevate_labs-task-7
# 🧠 Breast Cancer Classification using SVM

This project uses the Breast Cancer Wisconsin (Diagnostic) dataset to classify tumors as benign or malignant using Support Vector Machines (SVM). It includes model training with both linear and RBF kernels, visualization of decision boundaries, hyperparameter tuning, and cross-validation.

---

## 📌 Dataset Information

- **Source**: UCI Machine Learning Repository / scikit-learn datasets
- **Samples**: 569
- **Features**: 30 numeric features describing cell nuclei characteristics
- **Target**: 
  - `M` - Malignant
  - `B` - Benign

---

## ⚙️ Project Workflow

### 1. Load and Prepare Dataset
- Drop unnecessary columns (`id`)
- Encode `diagnosis` to binary (M → 1, B → 0)
- Scale features using `StandardScaler`
- Train-test split (80-20)

### 2. Train SVM Classifiers
- Train an SVM with a **linear** kernel
- Train an SVM with a **RBF** kernel
- Evaluate both models using accuracy score and classification report

### 3. Visualize Decision Boundary
- Use 2D data (`radius_mean`, `texture_mean`) for visualization
- Plot the decision surface of RBF SVM using `matplotlib`

### 4. Hyperparameter Tuning
- Perform grid search on `C` and `gamma` using `GridSearchCV`
- Identify best parameters and evaluate final model

### 5. Cross-Validation
- Perform 5-fold cross-validation to ensure model generalization

---

## 🧪 Dependencies

Install the required Python libraries:
```bash
pip install numpy pandas scikit-learn matplotlib
