# 🌳 Task 5: Decision Trees & Random Forests

This repository contains my implementation of **Decision Tree** and **Random Forest** algorithms as part of my **AI & ML Internship – Task 5**.

---

## 🎯 Objective

To understand and implement **tree-based models** for classification using:

- Decision Trees
- Random Forests

with focus on:
- Overfitting and pruning
- Feature importance
- Cross-validation
- Model comparison

---

## 🧰 Tools & Libraries

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Graphviz (for visualization)

---

## 📦 Dataset

- **Heart Disease Dataset**
- Binary classification: Predict presence of heart disease
- Features include age, sex, cholesterol, resting BP, etc.
- Target: `1` = Disease, `0` = No Disease


---

## 📊 Steps Performed

### 1. Data Preprocessing
- Checked for missing values
- Split data into features (`X`) and target (`y`)
- Train-test split (80-20)

### 2. Decision Tree Classifier
- Trained a `DecisionTreeClassifier` with max depth of 4
- Visualized the tree using `plot_tree()`
- Analyzed performance using accuracy & confusion matrix

### 3. Random Forest Classifier
- Trained a `RandomForestClassifier` with 100 estimators
- Compared its performance with decision tree
- Visualized feature importances

### 4. Evaluation
- Confusion matrices for both models
- Classification reports
- Cross-validation using `cross_val_score()`

---

## 📈 Results
| Model         | Train Accuracy | Test Accuracy | CV Accuracy (Mean ± Std) |
| ------------- | -------------- | ------------- | ------------------------ |
| Decision Tree | *e.g., 95.6%*  | *e.g., 83.0%* | **83.41% ± 0.02**        |
| Random Forest | *e.g., 100.0%* | *e.g., 98.9%* | **99.71% ± 0.01**        |


---

## 📉 Visualizations

- 📌 Decision Tree Plot  
- 📊 Feature Importance Plot  
- ✅ Confusion Matrices (DT & RF)

---

## 💡 Interview Questions & Answers

**1. How does a Decision Tree work?**  
A decision tree splits the data at feature thresholds to reduce impurity and reach a classification decision.

**2. What is Entropy and Information Gain?**  
- *Entropy* measures impurity in a dataset.
- *Information Gain* is the reduction in entropy after a split.

**3. How is Random Forest better than a single tree?**  
It reduces variance by averaging predictions over multiple trees (ensemble learning).

**4. What is Overfitting and how to prevent it?**  
Overfitting is when a model performs well on training data but poorly on new data. Prevent it using:
- `max_depth`, `min_samples_split`
- Ensemble models (e.g., Random Forest)

**5. What is Bagging?**  
Bagging (Bootstrap Aggregating) trains models on random subsets and combines their output to improve robustness.

**6. How do you visualize a decision tree?**  
Using `plot_tree()` or exporting via `graphviz`.

**7. How to interpret feature importance?**  
Top features are those that contribute most to impurity reduction across splits.

**8. Pros/Cons of Random Forest?**  
✅ Pros: High accuracy, handles missing data, reduces overfitting  
❌ Cons: Less interpretable, slower to train

---

