
# 🧠 Course 2: Advanced Learning Algorithms

Welcome to the root repository for **Course 2: Advanced Learning Algorithms**, the second core module of the **Stanford University & DeepLearning.AI Machine Learning Specialization**, taught by Andrew Ng.

This course builds directly upon foundational regression and classification models, expanding into multi-layer artificial neural networks with TensorFlow, advanced multiclass loss formulations, backpropagation calculus, machine learning engineering diagnostics, bias/variance tuning, and tree-based ensemble algorithms (Random Forests and XGBoost).

---

## 📝 Core Technical Objectives
* **Deep Neural Networks:** Constructing and training multi-layer neural networks using TensorFlow and Keras, alongside low-level matrix forward propagation in pure NumPy.
* **Multiclass Classification Mechanics:** Implementing Softmax activation layers and numerically stable Sparse Categorical Cross-Entropy loss ($z$-logit formulations).
* **Machine Learning Diagnostics:** Applying cross-validation splits ($60/20/20$), evaluating learning curves, diagnosing High Bias (underfitting) vs. High Variance (overfitting), and analyzing skewed datasets ($F_1$-score, Precision, Recall).
* **Decision Trees & Ensembles:** Building recursive binary decision trees using Entropy and Information Gain, scaling performance with Random Forests (bagging) and XGBoost (gradient boosting).

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

The course is structured across four comprehensive weekly modules detailing theoretical foundations, interactive labs, and practical algorithm implementations:

| Module / Directory | Analytical Focus | Key Implementations & Labs |
| :--- | :--- | :--- |
| **[Week 1: Neural Networks](./Week_1)** | Feedforward neural network architectures, layer activations, TensorFlow `Sequential` models, and manual matrix forward propagation. | `Neurons_and_Layers`, `CoffeeRoasting_TF`, `CoffeeRoasting_Numpy`, Binary Digit Classifier. |
| **[Week 2: Neural Network Training](./Week_2)** | Hidden activations (ReLU), Softmax multiclass classification, Adam optimization, derivative computation graphs, and backprop mechanics. | `Relu`, `SoftMax`, `Multiclass_TF`, `Derivatives`, `Backprop`, Multiclass Digit Classifier. |
| **[Week 3: ML Engineering Advice](./Week_3)** | Model evaluation, cross-validation, bias/variance diagnostics, regularization tuning, learning curves, error analysis, and transfer learning. | Model Selection, Bias/Variance Diagnostics, Precision/Recall Tradeoffs, Practice ML Assignment. |
| **[Week 4: Decision Trees & Ensembles](./Week_4)** | Non-parametric decision trees, node entropy, information gain, one-hot categorical encoding, Random Forests, and XGBoost models. | `Decision_Trees`, `Tree_Ensemble`, Mushroom Classifier, `XGBClassifier` Pipelines. |

---

## 💡 Visual Pipeline Reference

The comprehensive deep learning and ensemble engineering lifecycle executed throughout Course 2:

* **Neural Network Forward Pass** ➔ Transform features via stacked dense layers $\mathbf{a}^{[l]} = g(\mathbf{W}^{[l]} \mathbf{a}^{[l-1]} + \mathbf{b}^{[l]})$ using **ReLU** and **Softmax** activations.
* **Numerically Stable Optimization** ➔ Minimize Loss using raw logits $z$ with `SparseCategoricalCrossentropy(from_logits=True)` via the **Adam Optimizer**.
* **Diagnostic Loop & Error Analysis** ➔ Compare $J_{\text{train}}$ vs. $J_{\text{cv}}$ ➔ Adjust Regularization $\lambda$ or Layer Capacity ➔ Evaluate **Precision-Recall / $F_1$-score**.
* **Non-Parametric Ensemble Alternative** ➔ Compute **Information Gain** $I.G. = H(p_1^{\text{node}}) - \sum w^{v} H(p_1^{v})$ ➔ Deploy **XGBoost** for structured tabular data tasks.

---

## 🎯 Technical Skills Architecture

### 📊 Deep Learning & Ensemble Theory
* **Hierarchical Representation:** Understanding how hidden layers automatically extract complex abstract features from raw inputs.
* **Optimization Dynamics:** Managing backpropagation via computation graphs and accelerating convergence using adaptive momentum (Adam).
* **Model Choice Paradigms:** Choosing between dense neural architectures (unstructured data) and tree ensembles like Random Forests / XGBoost (structured/tabular data).

### 🤖 Applied Machine Learning Engineering
* **Production TensorFlow/Keras Execution:** Designing, compiling, and training end-to-end multi-class neural networks.
* **Systematic Model Tuning:** Utilizing cross-validation sets, diagnostic learning curves, and manual error analysis to guide iterative model improvements.
* **High-Performance Tree Pipelines:** Preprocessing continuous/categorical features and building high-accuracy XGBoost classifiers.

---

## 🛠️ Production Tech Stack & Ecosystem

| Deep Learning Framework | Gradient Boosting & Ensembles | Numerical Optimization | Development Environment |
| :---: | :---: | :---: | :---: |
| ![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x_Keras-FF6F00?style=flat&logo=tensorflow&logoColor=white) | ![XGBoost](https://img.shields.io/badge/XGBoost-Gradient_Boosting-239120?style=flat&logo=xgboost&logoColor=white) | ![NumPy](https://img.shields.io/badge/NumPy-Vectorized_Calculus-013243?style=flat&logo=numpy&logoColor=white) | ![Jupyter](https://img.shields.io/badge/Jupyter-Interactive_Labs-FA0F00?style=flat&logo=jupyter&logoColor=white) |

