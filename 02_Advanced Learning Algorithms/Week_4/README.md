
# 🌲 Decision Trees, Random Forests & Gradient Boosted Trees (XGBoost)

Welcome to Week 4 of **Advanced Learning Algorithms** (Course 2 of the Stanford University & DeepLearning.AI Machine Learning Specialization)! This module explores non-linear, non-parametric tree-based models: single decision trees, entropy and information gain mechanics, categorical one-hot encoding, continuous split points, random forest bagging ensembles, and XGBoost gradient boosting.

---

## 📝 Core Technical Objectives
* **Decision Tree Architecture:** Recursive binary partitioning of feature spaces based on node purity metrics to construct interpretable decision rules.
* **Entropy & Information Gain Mechanics:** Quantifying node impurity via Entropy $H(p_1) = -p_1 \log_2(p_1) - (1-p_1) \log_2(1-p_1)$ and maximizing Information Gain $I.G. = H(p_1^{\text{node}}) - \left( w^{\text{left}} H(p_1^{\text{left}}) + w^{\text{right}} H(p_1^{\text{right}}) \right)$.
* **Feature Processing Techniques:** Managing discrete categorical variables via One-Hot Encoding and handling continuous values by evaluating mid-point candidate thresholds.
* **Tree Ensemble Architectures:** Constructing Bagged Random Forests using bootstrap aggregation (sampling with replacement) and Gradient Boosted Decision Trees using XGBoost.

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

This module's core video lectures, interactive Jupyter notebooks, and practice assignments are mapped directly to their targeted analytical focus:

| Asset / Deliverable | Operational Focus |
| :--- | :--- |
| **[Decision Trees Lab](./01_Decision_Trees.ipynb)** | Calculating entropy, computing information gain across candidate feature splits, and building recursive binary decision tree nodes from scratch. |
| **[Tree Ensembles Lab](./02_Tree_Ensemble.ipynb)** | Implementing Random Forest ensembles and applying XGBoost (`xgboost.XGBClassifier`) for high-performance tabular classification. |
| **Decision Trees Assignment** | Graded programming project building a complete decision tree algorithm from scratch (entropy, split selection, tree construction) for mushroom classification. |

---

## 💡 Visual Pipeline Reference

The decision tree learning and ensemble modeling workflow implemented across this module:

* **Feature Impurity Evaluation** ➔ Calculate current node **Entropy** $H(p_1)$ based on positive label ratio $p_1$.
* **Information Gain Maximization** ➔ Evaluate candidate feature splits $\mathbf{x}_j$ ➔ Select split yielding maximum **Information Gain**.
* **Recursive Tree Splitting** ➔ Split dataset into left/right child nodes ➔ Recurse until maximum depth or purity thresholds are met.
* **Ensemble Aggregation** ➔ Combine predictions via **Random Forest** (majority vote across bootstrapped trees) or **XGBoost** (sequential error-residual fitting).

---

## 🎯 Technical Skills Architecture

### 📊 Machine Learning Theory
* **Non-Parametric Partitioning:** Understanding how decision trees partition feature space into axis-aligned rectangular hyperplanes without assuming linear separability.
* **Bagging vs. Boosting Mechanics:** Contrasting parallel variance-reduction ensembling (Random Forests) against sequential bias-reduction ensembling (Gradient Boosting).
* **Neural Networks vs. Decision Trees:** Evaluating architectural trade-offs: tabular structured data (Trees/XGBoost) vs. unstructured spatial/sequential data (Neural Networks).

### 🤖 Applied Machine Learning Engineering
* **Feature Transformation:** Preprocessing categorical features using One-Hot Encoding and dynamically determining split boundaries for continuous features.
* **XGBoost Optimization:** Configuring high-efficiency gradient boosted trees (`XGBClassifier`, `XGBRegressor`) with early stopping parameters.
* **Ensemble Hyperparameter Tuning:** Adjusting tree parameters (e.g., `max_depth`, `n_estimators`, `learning_rate`, `subsample`) to mitigate ensemble overfitting.

---

## 🛠️ Production Tech Stack & Ecosystem

| Gradient Boosting | Tree Ensembles | Scikit-Learn Framework | Development Environment |
| :---: | :---: | :---: | :---: |
| ![XGBoost](https://img.shields.io/badge/XGBoost-Gradient_Boosting-239120?style=flat&logo=xgboost&logoColor=white) | ![RandomForest](https://img.shields.io/badge/Random_Forest-Bagging_Ensemble-013243?style=flat&logo=python&logoColor=white) | ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-DecisionTreeClassifier-F7931E?style=flat&logo=scikit-learn&logoColor=white) | ![Jupyter](https://img.shields.io/badge/Jupyter-Interactive_Labs-FA0F00?style=flat&logo=jupyter&logoColor=white) |

