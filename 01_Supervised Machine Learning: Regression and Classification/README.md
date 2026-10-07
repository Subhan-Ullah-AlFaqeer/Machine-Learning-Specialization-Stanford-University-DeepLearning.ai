
# 🎓 Course 1: Supervised Machine Learning - Regression and Classification

Welcome to the root repository for **Course 1: Supervised Machine Learning (Regression and Classification)**, the foundational module of the **Stanford University & DeepLearning.AI Machine Learning Specialization**, taught by Andrew Ng.

This course introduces the core building blocks of modern artificial intelligence: supervised predictive modeling, vectorization, gradient descent optimization, feature engineering, binary classification, and regularization.

---

## 📝 Core Technical Objectives
* **Supervised Learning Frameworks:** Mastering univariate and multivariate linear regression alongside binary logistic regression.
* **Vectorized Mathematical Computation:** Accelerating linear algebra operations using NumPy matrix operations to bypass python `for` loops.
* **Optimization & Loss Mechanics:** Formulating Mean Squared Error (MSE) and Binary Cross-Entropy loss functions, optimized via batch gradient descent.
* **Regularization & Model Tuning:** Applying Z-score feature scaling, polynomial basis expansions, and $L_2$ regularization to eliminate underfitting and overfitting.

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

The course is structured across three core weekly modules, detailing theoretical foundations, interactive labs, and practical algorithm implementations:

| Module / Directory | Analytical Focus | Key Implementations & Labs |
| :--- | :--- | :--- |
| **[Week 1: Introduction & Linear Regression](./Week_1)** | Machine learning paradigms, model representation, cost functions, and univariate gradient descent. | Model representation, MSE loss surface visualization, manual gradient descent from scratch. |
| **[Week 2: Multiple Linear Regression](./Week_2)** | Multivariate regression, NumPy array vectorization, feature scaling, polynomial expansion, and Scikit-Learn tools. | High-performance matrix dot products, Z-score normalization, non-linear feature engineering, `SGDRegressor`. |
| **[Week 3: Classification & Regularization](./Week_3)** | Binary classification, Sigmoid decision boundaries, logistic loss (cross-entropy), and $L_2$ weight regularization. | Probabilistic outputs, non-linear decision boundaries, bias-variance trade-offs, regularized logistic models. |

---

## 💡 Visual Pipeline Reference

The overall end-to-end machine learning engineering workflow executed throughout Course 1:

* **Data Preprocessing & Scaling** ➔ Ingest feature matrix $\mathbf{X}$ ➔ Apply **Z-score Normalization** $x_j := \frac{x_j - \mu_j}{\sigma_j}$ to optimize contour geometry.
* **Feature Engineering** ➔ Expand non-linear relationship representation via **Polynomial Terms** ($x_1^2, x_1 x_2$).
* **Hypothesis & Activation** ➔ Compute linear combination $z = \mathbf{w} \cdot \mathbf{x} + b$ ➔ Apply **Sigmoid Function** $g(z) = \frac{1}{1 + e^{-z}}$ for classification tasks.
* **Regularized Optimization** ➔ Minimize cost $J(\mathbf{w},b)$ with $L_2$ penalty $\frac{\lambda}{2m}\sum w_j^2$ using **Vectorized Gradient Descent**.

---

## 🎯 Technical Skills Architecture

### 📊 Machine Learning Theory
* **Parametric Estimation:** Formulating linear hypotheses and mapping spatial boundaries via probabilistic logit activations.
* **Convex Loss Optimization:** Analyzing quadratic and logarithmic cost functions to guarantee global convergence.
* **Generalization & Regularization:** Controlling model variance and preventing overfitting using $L_2$ weight penalty constraints ($\lambda$).

### 🤖 Applied Machine Learning Engineering
* **Vectorized Scientific Computing:** Implementing scalable NumPy matrix workflows for fast array computation.
* **Scikit-Learn Framework Integration:** Building production pipelines with standard estimators (`LinearRegression`, `SGDRegressor`, `LogisticRegression`).
* **Model Profiling & Diagnostics:** Assessing learning rates, convergence plots, and loss surfaces with Matplotlib and Seaborn.

---

## 🛠️ Production Tech Stack & Ecosystem

| Numerical Computing | Production Frameworks | Data Visualization | Development Environment |
| :---: | :---: | :---: | :---: |
| ![NumPy](https://img.shields.io/badge/NumPy-Array_Vectorization-013243?style=flat&logo=numpy&logoColor=white) | ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine_Learning-F7931E?style=flat&logo=scikit-learn&logoColor=white) | ![Matplotlib](https://img.shields.io/badge/Matplotlib-Data_Visualization-11557c?style=flat&logo=python&logoColor=white) | ![Jupyter](https://img.shields.io/badge/Jupyter-Interactive_Notebooks-FA0F00?style=flat&logo=jupyter&logoColor=white) |

