
# 🏆 Stanford University & DeepLearning.AI Machine Learning Specialization

Welcome to the root repository for the **Machine Learning Specialization**, a foundational 3-course online program created in collaboration between **Stanford Online** and **DeepLearning.AI**, taught by **Andrew Ng**.

This repository serves as a comprehensive, production-grade technical portfolio documenting all code implementations, interactive Jupyter laboratories, mathematical derivations, deep learning models, and applied machine learning projects across the entire Specialization.

---

## 📝 Core Technical Objectives
* **Supervised Learning Foundations:** Implementing Multiple Linear Regression, Logistic Regression, Feature Scaling, Polynomial Regression, and Regularization ($\text{L}_1/\text{L}_2$) from scratch in pure NumPy and Scikit-Learn.
* **Deep Learning & Neural Architectures:** Building, training, and optimizing Dense Multi-Layer Perceptrons (MLPs) using TensorFlow/Keras, implementing custom activations (ReLU, Sigmoid, Softmax), loss formulations (`from_logits=True`), Adam optimization, and backpropagation via computation graphs.
* **Production ML Engineering Diagnostics:** Partitioning train/validation/test sets, analyzing High Bias vs. High Variance (learning curves), executing systematic error analysis, applying data augmentation/transfer learning, and evaluating imbalanced classification metrics ($F_1$-score, Precision, Recall).
* **Non-Parametric Tree Ensembles:** Constructing recursive decision trees using Entropy and Information Gain, scaling tabular classification and regression via Random Forests (bagging) and XGBoost (gradient boosting).
* **Unsupervised Learning & Anomaly Detection:** Implementing iterative K-Means clustering, Gaussian probability density estimation $p(\mathbf{x}) < \epsilon$ for anomaly detection, and Principal Component Analysis (PCA) for dimensionality reduction.
* **Industrial Recommender Systems:** Developing Collaborative Filtering via matrix factorization and building Dual-Tower Content-Based Deep Learning Recommender Systems in TensorFlow.
* **Deep Reinforcement Learning:** Formulating Markov Decision Processes (MDPs), solving Bellman Equations, and training Deep Q-Networks (DQN) with Experience Replay buffers and soft target updates for continuous control tasks.

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

The specialization is organized into three core courses covering the complete spectrum of modern artificial intelligence and machine learning methodologies:

| Course / Directory | Core Analytical Focus | Key Projects & Technologies |
| :--- | :--- | :--- |
| **[01: Supervised Machine Learning](./01_Supervised_Machine_Learning_Regression_and_Classification)** | Fundamental regression and classification models, gradient descent optimization, cost functions, feature scaling, and regularization. | Housing Price Predictor, Breast Cancer Classifier, Gradient Descent from scratch, Scikit-Learn pipelines. |
| **[02: Advanced Learning Algorithms](./02_Advanced_Learning_Algorithms)** | Deep multi-layer neural networks, multiclass Softmax classification, backprop calculus, ML lifecycle diagnostics, and tree ensembles. | TensorFlow Handwritten Digit Classifier, Bias/Variance Diagnostics, Mushroom Classifier, XGBoost pipelines. |
| **[03: Unsupervised Learning & RL](./03_Unsupervised_Learning_Recommenders_Reinforcement_Learning)** | Unsupervised clustering, Gaussian anomaly detection, matrix factorization recommenders, dual-tower neural nets, and Deep Q-Learning. | Image Compression via K-Means, Server Anomaly Detector, Movie Recommender Systems, Lunar Lander DQN Agent. |

---

## 💡 Visual Pipeline Reference

The unified machine learning engineering lifecycle executed throughout this specialization portfolio:

* **Data Engineering & Unsupervised Exploration** ➔ Preprocess features with **NumPy/Pandas** ➔ Cluster unlabeled spaces via **K-Means** or detect outliers using **Gaussian Density Estimation**.
* **Supervised Model Execution** ➔ Choose architecture based on data topology:
  * **Tabular / Structured Data** ➔ Maximize Information Gain using **XGBoost / Random Forests**.
  * **Perceptual / Complex Data** ➔ Construct **TensorFlow/Keras** Neural Networks with **ReLU** and **Softmax** layers.
* **Diagnostic & Hyperparameter Loop** ➔ Evaluate $J_{\text{train}}$ vs. $J_{\text{cv}}$ ➔ Adjust Regularization $\lambda$ / Network Capacity ➔ Tune thresholds via **Precision-Recall / $F_1$-score**.
* **Sequential Decision Control** ➔ Model environment dynamics as an **MDP** ➔ Approximate $Q^*$-values using **Deep Q-Networks (DQN)** with target soft updates.

---

## 🎯 Technical Skills Architecture

### 📊 Machine Learning & Artificial Intelligence Theory
* **Mathematical Foundations:** Deriving gradient updates for linear/logistic objectives, partial derivative chain rule for backpropagation, vector projection for PCA, and Bellman optimality recurrences.
* **Statistical Modeling & Probability:** Estimating Gaussian joint probabilities, calculating continuous/discrete node entropy, and evaluating expected discounted return $R_t = \sum \gamma^k r_{t+k+1}$.
* **Generalization & Diagnostics:** Quantifying model capacity along the bias-variance tradeoff spectrum and managing class imbalance via harmonic mean $F_1$-score metrics.

### 🤖 Applied Machine Learning Engineering
* **Vectorized System Architecture:** Writing high-performance array manipulations and matrix operations in vectorized NumPy without explicit Python loops.
* **Deep Learning Pipeline Engineering:** Designing, compiling, training, and deploying Keras sequential and functional models with custom training loops (`tf.GradientTape`).
* **Production Tooling & Libraries:** Training state-of-the-art boosted ensembles (`xgboost`), configuring open-source RL environments (`gymnasium`), and executing Scikit-Learn workflows.

---

## 🛠️ Production Tech Stack & Ecosystem

| Core ML & Numerical Computing | Deep Learning Framework | Ensembles & Analytics | RL & Environment Ecosystem |
| :---: | :---: | :---: | :---: |
| ![NumPy](https://img.shields.io/badge/NumPy-1.2x-013243?style=flat&logo=numpy&logoColor=white) ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.x-F7931E?style=flat&logo=scikit-learn&logoColor=white) | ![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x_Keras-FF6F00?style=flat&logo=tensorflow&logoColor=white) | ![XGBoost](https://img.shields.io/badge/XGBoost-Gradient_Boosting-239120?style=flat&logo=xgboost&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c?style=flat&logo=python&logoColor=white) | ![Gymnasium](https://img.shields.io/badge/OpenAI_Gym-Lunar_Lander-0081C8?style=flat&logo=openai&logoColor=white) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-FA0F00?style=flat&logo=jupyter&logoColor=white) |

