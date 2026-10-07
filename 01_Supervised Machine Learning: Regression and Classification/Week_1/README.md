
# 🤖 Supervised Machine Learning: Introduction, Linear Regression & Gradient Descent

Welcome to Week 1 of **Supervised Machine Learning: Regression and Classification** by Stanford University & DeepLearning.AI! This module establishes the core foundations of modern AI: defining supervised vs. unsupervised paradigms, constructing linear regression models, visualizing cost surfaces, and executing gradient descent optimization.

---

## 📝 Core Technical Objectives
* **Paradigms of Machine Learning:** Differentiating supervised learning (regression and classification) from unsupervised learning (clustering, dimensionality reduction, anomaly detection).
* **Model Representation:** Formulating univariate linear regression equations $f_{w,b}(x) = wx + b$ to map input features to continuous target predictions.
* **Cost Function Formulation:** Implementing the Mean Squared Error (MSE) cost function $J(w,b)$ to quantify parameter error against ground-truth labels.
* **Gradient Descent Optimization:** Deriving and implementing iterative parameter updates ($\theta_j := \theta_j - \alpha \frac{\partial}{\partial \theta_j} J$) to minimize loss surfaces.

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

This module's core video lectures, interactive Jupyter notebooks, and practice quizzes are mapped directly to their targeted analytical focus:

| Asset / Deliverable | Operational Focus |
| :--- | :--- |
| **[Python & Jupyter Notebooks](./01_Python_Jupyter_Notebook.ipynb)** | Environment setup, Python execution basics, vector operations, and Markdown documentation in Jupyter. |
| **[Model Representation Lab](./02_Model_Representation.ipynb)** | Hands-on construction of single-feature linear regression models using Matplotlib to plot data points and prediction lines. |
| **[Cost Function Lab](./04_Cost_function.ipynb)** | Visualizing Mean Squared Error (MSE) loss surfaces using 2D plots and 3D contour maps to build intuition for parameter selection ($w, b$). |
| **[Gradient Descent Lab](./05_Gradient_Descent.ipynb)** | Implementing batch gradient descent from scratch, analyzing learning rate ($\alpha$) tuning, convergence behavior, and parameter optimization trajectories. |

---

## 💡 Visual Pipeline Reference

The foundational machine learning workflow implemented across this module:

* **Training Data Ingestion** ➔ Features $x$ and ground-truth targets $y$ fed into **Linear Hypothesis** $f_{w,b}(x) = wx + b$.
* **Prediction & Loss Calculation** ➔ Measure prediction error via **Mean Squared Error (MSE)** $J(w,b) = \frac{1}{2m} \sum_{i=1}^m (f_{w,b}(x^{(i)}) - y^{(i)})^2$.
* **Gradient Step Computation** ➔ Calculate partial derivatives $\frac{\partial J}{\partial w}$ and $\frac{\partial J}{\partial b}$ against current weights.
* **Iterative Parameter Updates** ➔ Update weight $w := w - \alpha \frac{\partial J}{\partial w}$ and bias $b := b - \alpha \frac{\partial J}{\partial b}$ until cost convergence.

---

## 🎯 Technical Skills Architecture

### 📊 Machine Learning Theory
* **Supervised vs. Unsupervised Taxonomy:** Categorizing data problems based on labeled training data availability versus unlabelled structural discovery.
* **Loss Surface Geometry:** Analyzing convex quadratic cost functions, global minima, and learning rate sensitivity (overshooting vs. slow convergence).
* **Linear Parameter Estimation:** Understanding the roles of slope weight $w$ and intercept bias $b$ in spatial mapping.

### 🤖 Applied Machine Learning Engineering
* **Custom Algorithm Implementation:** Writing vectorized NumPy loops to execute gradient descent without high-level framework dependencies.
* **Hyperparameter Tuning:** Selecting appropriate learning rates ($\alpha$) to ensure numerical stability and efficient gradient convergence.
* **Data Visualization:** Utilizing Matplotlib and Seaborn to construct interactive 3D contour plots and parameter trajectory tracks.

---

## 🛠️ Production Tech Stack & Ecosystem

| Core Mathematics | Matrix Vectorization | Data Visualization | Development Environment |
| :---: | :---: | :---: | :---: |
| ![Calculus](https://img.shields.io/badge/Mathematics-Gradient_Calculus-blue?style=flat&logo=sympy&logoColor=white) | ![NumPy](https://img.shields.io/badge/NumPy-Vectorized_Math-013243?style=flat&logo=numpy&logoColor=white) | ![Matplotlib](https://img.shields.io/badge/Matplotlib-Loss_Visualization-11557c?style=flat&logo=python&logoColor=white) | ![Jupyter](https://img.shields.io/badge/Jupyter-Interactive_Labs-FA0F00?style=flat&logo=jupyter&logoColor=white) |

