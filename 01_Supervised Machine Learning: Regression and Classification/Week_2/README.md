
# 📈 Multiple Linear Regression, Feature Engineering & Vectorization

Welcome to Week 2 of **Supervised Machine Learning: Regression and Classification** by Stanford University & DeepLearning.AI! This module extends linear regression from single-variable models to multiple input features, introducing NumPy vectorization, feature scaling techniques, polynomial feature engineering, and Scikit-Learn implementations.

---

## 📝 Core Technical Objectives
* **Multiple Linear Regression Architecture:** Formulating multivariate prediction hypotheses $f_{\mathbf{w},b}(\mathbf{x}) = \mathbf{w} \cdot \mathbf{x} + b = w_1 x_1 + w_2 x_2 + \dots + w_n x_n + b$.
* **Vectorized Execution:** Utilizing NumPy matrix dot products ($\mathbf{w} \cdot \mathbf{x}$) to accelerate parameter updates and prediction calculations over large datasets.
* **Feature Scaling & Optimization:** Applying Z-score normalization and mean centering to equalize feature scales and accelerate gradient descent convergence.
* **Feature Engineering & Non-Linear Mapping:** Constructing non-linear transformations (polynomial regression $x_1^2, \sqrt{x_1}$) to capture complex feature relationships.

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

This module's core video lectures, interactive Jupyter notebooks, and practice assignments are mapped directly to their targeted analytical focus:

| Asset / Deliverable | Operational Focus |
| :--- | :--- |
| **[Python, NumPy & Vectorization](./01_Python_Numpy_Vectorization.ipynb)** | Implementing array operations, vector indexing, and matrix dot products to replace explicit Python `for` loops for scalable ML calculations. |
| **[Multiple Linear Regression](./02_Multiple_Variable.ipynb)** | Writing vectorized gradient descent routines for multiple input features and tracking multi-feature parameter convergence. |
| **[Feature Scaling & Learning Rates](./03_Feature_Scaling_and_Learning_Rate.ipynb)** | Applying Z-score normalization to rescale feature ranges and evaluating learning rate ($\alpha$) choices using learning curves. |
| **[Feature Engineering & Polynomial Regression](./04_FeatEng_PolyReg.ipynb)** | Creating non-linear polynomial features ($x^2, x^3$) to fit complex non-linear trends using linear regression frameworks. |
| **[Scikit-Learn Gradient Descent](./05_Sklearn_GD.ipynb)** | Implementing multivariate linear regression models using `SGDRegressor` with built-in feature scaling pipelines. |
| **[Scikit-Learn Normal Equation](./06_Sklearn_Normal.ipynb)** | Fitting linear regression models analytically using Scikit-Learn's `LinearRegression` without manual gradient step iterations. |
| **Linear Regression Programming Assignment** | Graded project building an end-to-end, vectorized multiple linear regression model with feature scaling from scratch. |

---

## 💡 Visual Pipeline Reference

The multivariate regression workflow implemented across this module:

* **Multivariate Data Processing** ➔ Ingest feature matrix $\mathbf{X} \in \mathbb{R}^{m \times n}$ and target vector $\mathbf{y} \in \mathbb{R}^m$.
* **Feature Standardization** ➔ Scale input features via Z-score $x_j^{(i)} := \frac{x_j^{(i)} - \mu_j}{\sigma_j}$ to form well-conditioned contour surfaces.
* **Polynomial Expansion** ➔ Engineer complex non-linear combinations (e.g., $x_1 x_2, x_1^2$) for improved model expressiveness.
* **Vectorized Gradient Optimization** ➔ Compute weight updates $\mathbf{w} := \mathbf{w} - \alpha \frac{1}{m} \mathbf{X}^T (f_{\mathbf{w},b}(\mathbf{X}) - \mathbf{y})$ until convergence.

---

## 🎯 Technical Skills Architecture

### 📊 Machine Learning Theory
* **Multivariate Hypothesis Mechanics:** Analyzing how individual weight parameters $w_j$ quantify feature importance in continuous target predictions.
* **Loss Surface Conditioning:** Understanding how disparate feature scales create elongated, inefficient cost contours and how normalization sphericalizes loss landscapes.
* **Polynomial Basis Expansion:** Using linear model architectures to learn non-linear decision boundaries through feature transformation.

### 🤖 Applied Machine Learning Engineering
* **High-Performance Vectorization:** Leveraging NumPy BLAS routines for fast array operations over large training sets.
* **Convergence Diagnostics:** Monitoring cost functions $J(\mathbf{w},b)$ across iterations to detect learning rate divergence or underfitting.
* **Production Framework Integration:** Comparing custom NumPy implementations against production-grade `scikit-learn` algorithms.

---

## 🛠️ Production Tech Stack & Ecosystem

| Vectorized Computing | Feature Preprocessing | Machine Learning Framework | Development Environment |
| :---: | :---: | :---: | :---: |
| ![NumPy](https://img.shields.io/badge/NumPy-Vectorization-013243?style=flat&logo=numpy&logoColor=white) | ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-StandardScaler-F7931E?style=flat&logo=scikit-learn&logoColor=white) | ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-SGDRegressor-F7931E?style=flat&logo=scikit-learn&logoColor=white) | ![Jupyter](https://img.shields.io/badge/Jupyter-Interactive_Labs-FA0F00?style=flat&logo=jupyter&logoColor=white) |

```
