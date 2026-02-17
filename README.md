# Hyperparameter Tuning using GridSearchCV

## Project Overview
This project demonstrates systematic model optimization using GridSearchCV
on the Breast Cancer dataset with a Support Vector Machine (SVM) classifier.

The aim is to evaluate whether tuning hyperparameters improves model
generalization compared to default settings.

---

## Dataset
Breast Cancer dataset from scikit-learn

- Binary classification problem
- 30 numerical medical features
- Target:
  - 0 → Malignant
  - 1 → Benign

---

## Methodology

### Baseline Model
A default SVM classifier is trained to establish baseline performance.

### Hyperparameter Tuning
GridSearchCV is applied using 5-fold cross-validation to search for optimal parameters.

Tuned parameters:
- **C** → Regularization strength
- **Kernel** → Decision boundary type
- **Gamma** → Influence of training samples

### Model Selection
The parameter combination with the highest cross-validation accuracy is selected.

---

## Results
The tuned model demonstrates improved performance compared to the default model.

The notebook includes:
- Best parameter output
- Cross-validation score
- Performance comparison table

---

## Key Takeaways
- Default hyperparameters are not always optimal
- Cross-validation improves model reliability
- Systematic tuning enhances generalization ability

---

## Practical Insight

This experiment shows that model performance depends strongly on hyperparameter selection.

The default SVM learns a decision boundary based on generic assumptions,
while GridSearchCV systematically identifies parameters that better fit the dataset structure.

Cross-validation ensures the improvement is consistent across multiple splits,
making the tuned model more reliable for unseen data rather than just fitting one test split.

In real-world ML workflows, hyperparameter tuning is essential to move from a working model to a dependable model.

---

## Repository Contents

| File | Description |
|------|------------|
| Hyperparameter_Tuning_GridSearchCV.ipynb | Full implementation and outputs |
| README.md | Project documentation |

---

## Tools Used
- Python
- Scikit-learn
- Pandas 
- NumPy
