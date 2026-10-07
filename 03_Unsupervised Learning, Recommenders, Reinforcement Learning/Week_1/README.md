
# 🔍 Unsupervised Learning: K-Means Clustering & Anomaly Detection

Welcome to Week 1 of **Unsupervised Learning, Recommenders, Reinforcement Learning** (Course 3 of the Stanford University & DeepLearning.AI Machine Learning Specialization)! This module introduces unsupervised learning techniques for unlabelled datasets: the K-Means clustering iterative optimization algorithm, Gaussian density estimation for anomaly detection, feature engineering for normal distributions, and evaluation strategy trade-offs.

---

## 📝 Core Technical Objectives
* **K-Means Clustering Algorithm:** Partitioning unlabeled feature vectors $\mathbf{x}^{(i)}$ into $K$ spatial clusters by alternating between cluster assignment $\min_k \|\mathbf{x}^{(i)} - \boldsymbol{\mu}_k\|^2$ and centroid re-computation $\boldsymbol{\mu}_k = \frac{1}{|c^{(k)}|} \sum_{i \in c^{(k)}} \mathbf{x}^{(i)}$.
* **K-Means Distortion Cost Function:** Minimizing distortion objective $J(c^{(1)}, \dots, c^{(m)}, \boldsymbol{\mu}_1, \dots, \boldsymbol{\mu}_K) = \frac{1}{m} \sum_{i=1}^m \|\mathbf{x}^{(i)} - \boldsymbol{\mu}_{c^{(i)}}\|^2$ using random centroid initializations and the Elbow Method.
* **Gaussian Anomaly Detection Mechanics:** Estimating multi-feature probability density $p(\mathbf{x}) = \prod_{j=1}^n p(x_j; \mu_j, \sigma_j^2) = \prod_{j=1}^n \frac{1}{\sqrt{2\pi}\sigma_j} \exp\left(-\frac{(x_j - \mu_j)^2}{2\sigma_j^2}\right)$ to flag rare instances where $p(\mathbf{x}) < \epsilon$.
* **Supervised vs. Anomaly Detection Paradigms:** Evaluating structural trade-offs between binary classification (large labeled positive dataset) and anomaly detection (extremely small/rare positive anomaly set, unknown future anomaly types).

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

This module's core video lectures, interactive Jupyter notebooks, and practice assignments are mapped directly to their targeted analytical focus:

| Asset / Deliverable | Operational Focus |
| :--- | :--- |
| **[K-Means Clustering Assignment](./KMeans_Assignment.ipynb)** | Graded programming lab implementing closest centroid assignment, centroid update loops, random initialization, and image color quantization compression. |
| **[Anomaly Detection Lab](./Anomaly_Detection.ipynb)** | Graded programming lab estimating Gaussian distribution parameters $(\mu_j, \sigma_j^2)$, calculating multi-variable probability densities, and tuning threshold $\epsilon$ using $F_1$-score on validation data. |

---

## 💡 Visual Pipeline Reference

The unsupervised clustering and Gaussian anomaly detection workflows implemented across this module:

* **K-Means Iterative Loop** ➔ Randomly initialize $K$ centroids $\boldsymbol{\mu}_1, \dots, \boldsymbol{\mu}_K$ ➔ Assign points to nearest centroid ➔ Update centroids to mean point positions ➔ Convergence.
* **Feature Transformation** ➔ Check feature histograms for normal distributions ➔ Apply non-linear transformations (e.g., $\log(x)$, $\sqrt{x}$) to transform skewed features.
* **Gaussian Density Estimation** ➔ Calculate sample means $\mu_j = \frac{1}{m}\sum x_j^{(i)}$ and variances $\sigma_j^2 = \frac{1}{m}\sum (x_j^{(i)} - \mu_j)^2$.
* **Threshold Flagging** ➔ Evaluate joint density $p(\mathbf{x}) < \epsilon$ ➔ Flag anomalous server/hardware faults or suspicious system behavior.

---

## 🎯 Technical Skills Architecture

### 📊 Unsupervised Machine Learning Theory
* **Iterative Convergence Guarantees:** Proving why the K-Means two-step loop monotonically decreases or maintains the distortion cost function $J$.
* **Gaussian Joint Probability Density:** Modeling multi-dimensional feature distributions assuming independent conditional probability products.
* **Anomaly Evaluation Metrics:** Tuning detection thresholds $\epsilon$ using labeled cross-validation sets with Precision, Recall, and $F_1$-score rather than raw accuracy.

### 🤖 Applied Machine Learning Engineering
* **Vectorized Array Operations:** Implementing NumPy broadcast routines to compute pairwise distances between $m$ data points and $K$ centroids without explicit double loops.
* **Image Compression via Quantization:** Reducing color storage depth by mapping RGB pixel colors to $K$ learned centroid colors.
* **Feature Engineering for Density Models:** Constructing domain-specific ratio features (e.g., $\frac{\text{CPU load}}{\text{network throughput}}$) to expose hidden anomalous behavior.

---

## 🛠️ Production Tech Stack & Ecosystem

| Numerical Computing | Scikit-Learn Framework | Data Visualization | Development Environment |
| :---: | :---: | :---: | :---: |
| ![NumPy](https://img.shields.io/badge/NumPy-Array_Broadcasting-013243?style=flat&logo=numpy&logoColor=white) | ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-KMeans_%26_Gaussian-F7931E?style=flat&logo=scikit-learn&logoColor=white) | ![Matplotlib](https://img.shields.io/badge/Matplotlib-Density_Contours-11557c?style=flat&logo=python&logoColor=white) | ![Jupyter](https://img.shields.io/badge/Jupyter-Interactive_Labs-FA0F00?style=flat&logo=jupyter&logoColor=white) |

