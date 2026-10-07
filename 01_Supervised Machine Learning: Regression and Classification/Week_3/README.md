
# 🎯 Logistic Regression, Decision Boundaries & Regularization

Welcome to Week 3 of **Supervised Machine Learning: Regression and Classification** by Stanford University & DeepLearning.AI! This module transitions from linear regression to binary classification, establishing the theoretical mechanics of Logistic Regression, non-linear decision boundaries, binary cross-entropy loss, and regularization to combat model overfitting.

---

## 📝 Core Technical Objectives
* **Logistic Regression Hypothesis:** Mapping continuous linear predictions to probabilities via the Sigmoid/Logistic activation function $g(z) = \frac{1}{1 + e^{-z}}$, yielding hypothesis $f_{\mathbf{w},b}(\mathbf{x}) = g(\mathbf{w} \cdot \mathbf{x} + b)$.
* **Decision Boundary Formulation:** Establishing spatial classification thresholds where $f_{\mathbf{w},b}(\mathbf{x}) \ge 0.5$ when $\mathbf{w} \cdot \mathbf{x} + b \ge 0$, creating linear and non-linear polynomial decision surfaces.
* **Binary Cross-Entropy Cost Function:** Deriving the convex non-linear loss $L(f_{\mathbf{w},b}(\mathbf{x}), y) = -y \log(f) - (1-y) \log(1-f)$ to ensure reliable convergence during gradient optimization.
* **Overfitting & $L_2$ Regularization:** Quantifying high variance and applying regularization penalties $\frac{\lambda}{2m} \sum_{j=1}^n w_j^2$ to shrink model weights and improve out-of-sample generalization.

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

This module's core video lectures, interactive Jupyter notebooks, and practice assignments are mapped directly to their targeted analytical focus:

| Asset / Deliverable | Operational Focus |
| :--- | :--- |
| **[Classification Motivation](./01_Classification.ipynb)** | Contrasting linear regression failure modes on categorical labels with probabilistic classification approaches. |
| **[Sigmoid Activation Function](./02_Sigmoid_function.ipynb)** | Plotting and evaluating properties of the Sigmoid function $g(z)$ across continuous logit inputs. |
| **[Decision Boundaries](./03_Decision_Boundary.ipynb)** | Visualizing spatial decision surfaces for linear and non-linear polynomial classification features. |
| **[Logistic Loss Analysis](./04_LogisticLoss.ipynb)** | Comparing squared error loss instability against smooth, convex binary cross-entropy loss functions. |
| **[Logistic Cost Function](./05_Cost_Function.ipynb)** | Computing total cross-entropy loss over binary training sets across varied weight and bias parameters. |
| **[Gradient Descent Optimization](./06_Gradient_Descent.ipynb)** | Implementing vectorized gradient descent parameter updates specifically tailored for logistic models. |
| **[Scikit-Learn Classification](./07_Scikit_Learn.ipynb)** | Training production logistic regression classifiers using Scikit-Learn's `LogisticRegression` API. |
| **[Overfitting Diagnostics](./08_Overfitting.ipynb)** | Analyzing high bias (underfitting) vs. high variance (overfitting) across varying model complexities. |
| **[Regularization Mechanics](./09_Regularization.ipynb)** | Implementing $L_2$ regularized cost functions and gradient steps for linear and logistic models. |
| **Logistic Regression Assignment** | Graded programming project implementing a complete, regularized logistic regression classifier with non-linear decision boundaries from scratch. |

---

## 💡 Visual Pipeline Reference

The binary classification and regularization workflow implemented across this module:

* **Linear Combination Ingestion** ➔ Calculate logit input $z = \mathbf{w} \cdot \mathbf{x} + b$ for feature vector $\mathbf{x}$.
* **Probability Activation** ➔ Pass logit through **Sigmoid Function** $a = g(z) = \frac{1}{1 + e^{-z}} \in (0, 1)$.
* **Binary Cross-Entropy Loss** ➔ Calculate loss $J(\mathbf{w},b) = -\frac{1}{m} \sum_{i=1}^m \left[ y^{(i)} \log(a^{(i)}) + (1 - y^{(i)}) \log(1 - a^{(i)}) \right]$.
* **Regularized Gradient Step** ➔ Update weights $\mathbf{w} := \mathbf{w} \left(1 - \alpha \frac{\lambda}{m}\right) - \alpha \frac{1}{m} \mathbf{X}^T (\mathbf{a} - \mathbf{y})$ to penalize large parameter magnitudes.

---

## 🎯 Technical Skills Architecture

### 📊 Machine Learning Theory
* **Probabilistic Classification:** Interpreting logistic outputs $f_{\mathbf{w},b}(\mathbf{x})$ as conditional probability estimates $P(y=1 \vert{} \mathbf{x}; \mathbf{w}, b)$.
* **Convex Loss Optimization:** Understanding why Mean Squared Error yields non-convex local minima in classification and how logarithmic loss guarantees global convergence.
* **Variance Control via Regularization:** Managing the bias-variance tradeoff using the regularization hyperparameter $\lambda$.

### 🤖 Applied Machine Learning Engineering
* **Vectorized Logistic Optimization:** Building scalable NumPy routines for Sigmoid activations, log-loss computations, and regularized gradients.
* **Non-Linear Classification Boundaries:** Engineering higher-order polynomial features to fit complex, non-spherical decision regions.
* **Framework vs. Scratch Implementation:** Benchmarking hand-crafted vectorized Python pipelines against optimized `sklearn.linear_model.LogisticRegression` estimators.

---

## 🛠️ Production Tech Stack & Ecosystem

| Core Mathematics | Vectorized Optimization | Classification Architecture | Development Environment |
| :---: | :---: | :---: | :---: |
| ![Probability](https://img.shields.io/badge/Mathematics-Logistic_Loss-blue?style=flat&logo=sympy&logoColor=white) | ![NumPy](https://img.shields.io/badge/NumPy-Vectorized_Sigmoid-013243?style=flat&logo=numpy&logoColor=white) | ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-LogisticRegression-F7931E?style=flat&logo=scikit-learn&logoColor=white) | ![Jupyter](https://img.shields.io/badge/Jupyter-Interactive_Labs-FA0F00?style=flat&logo=jupyter&logoColor=white) |

```
