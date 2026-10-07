
# 🎬 Recommender Systems: Collaborative Filtering, Content-Based Neural Nets & PCA

Welcome to Week 2 of **Unsupervised Learning, Recommenders, Reinforcement Learning** (Course 3 of the Stanford University & DeepLearning.AI Machine Learning Specialization)! This module explores industrial recommender system architectures: Collaborative Filtering matrix factorization, Mean Normalization, deep learning Content-Based Filtering with dual-tower neural networks, large catalog retrieval/ranking pipelines, and Principal Component Analysis (PCA) dimensionality reduction.

---

## 📝 Core Technical Objectives
* **Collaborative Filtering Formulation:** Simultaneously learning user preference vectors $\mathbf{w}^{(u)}, b^{(u)}$ and item feature representations $\mathbf{x}^{(i)}$ by minimizing $J = \frac{1}{2} \sum_{(i,u):r(i,u)=1} \left( \mathbf{w}^{(u)} \cdot \mathbf{x}^{(i)} + b^{(u)} - y^{(i,u)} \right)^2 + \text{regularization}$.
* **Mean Normalization Preprocessing:** Adjusting rating matrices by subtracting user average ratings $\mu_i$ to ensure cold-start users with zero ratings receive reasonable baseline predictions.
* **Content-Based Dual-Tower Neural Networks:** Training separate user and item neural networks to map user features $\mathbf{v}_u$ and item features $\mathbf{v}_m$ into a shared embedding space, predicting affinity via dot product $y^{(i,u)} = \mathbf{v}_u \cdot \mathbf{v}_m$.
* **Large Catalog Retrieval & Ranking Strategy:** Scaling recommendations to millions of items via candidate generation (retrieval) followed by fine-grained neural scoring (ranking).
* **Principal Component Analysis (PCA):** Reducing feature dimensionality by projecting data onto orthogonal principal axes that maximize variance retention.

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

This module's core video lectures, interactive Jupyter notebooks, and practice assignments are mapped directly to their targeted analytical focus:

| Asset / Deliverable | Operational Focus |
| :--- | :--- |
| **[Collaborative Filtering Assignment](./Collaborative_RecSys_Assignment.ipynb)** | Graded programming lab building a collaborative filtering movie recommender system using TensorFlow custom training loops (`tf.GradientTape`) and mean normalization. |
| **[Content-Based RecSys Assignment](./RecSysNN_Assignment.ipynb)** | Graded programming lab constructing a dual-tower neural network architecture in TensorFlow/Keras to match user and movie feature embeddings. |

---

## 💡 Visual Pipeline Reference

The end-to-end recommender system and dual-tower neural architecture workflow implemented across this module:

* **Rating Matrix Ingestion & Mean Normalization** ➔ Subtract item/user rating averages $\boldsymbol{\mu}$ ➔ Construct binary mask matrix $\mathbf{R}$ where $r(i,u)=1$.
* **Matrix Factorization Gradient Step** ➔ Minimize collaborative loss $J(\mathbf{W}, \mathbf{X}, \mathbf{B})$ using auto-differentiation via `tf.GradientTape()`.
* **Dual-Tower Neural Embedding Architecture**:
  * User Features $\mathbf{x}_u$ ➔ **User Network** ➔ Low-dimensional Embedding Vector $\mathbf{v}_u$.
  * Item Features $\mathbf{x}_m$ ➔ **Item Network** ➔ Low-dimensional Embedding Vector $\mathbf{v}_m$.
* **Affinity Prediction & Retrieval** ➔ Predict rating $y = \mathbf{v}_u \cdot \mathbf{v}_m$ ➔ Generate top-N recommendations via approximate nearest neighbors (ANN).

---

## 🎯 Technical Skills Architecture

### 📊 Recommender System Theory
* **Implicit vs. Explicit Feedback Mechanics:** Transitioning from numeric star ratings to binary interaction logs (clicks, views, likes, watch time).
* **Cold-Start Handling:** Addressing unrated items and new users through mean normalization and content feature networks.
* **Retrieval vs. Ranking Architecture:** Designing multi-stage production recommendation funnels (million items ➔ hundreds generated ➔ top-10 ranked).

### 🤖 Applied Machine Learning Engineering
* **TensorFlow Custom Training Loops:** Implementing automatic differentiation and manual parameter updates using `tf.GradientTape` for non-standard loss functions.
* **Dual-Tower Network Construction:** Building decoupled `tf.keras` sub-models that output matching linear embedding vectors for cosine similarity dot products.
* **Dimensionality Reduction via PCA:** Utilizing Scikit-Learn `PCA` for feature compression and high-dimensional dataset visualization.

---

## 🛠️ Production Tech Stack & Ecosystem

| Deep Learning Framework | Vectorized Tensor Computations | Framework Analytics | Development Environment |
| :---: | :---: | :---: | :---: |
| ![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x_Keras-FF6F00?style=flat&logo=tensorflow&logoColor=white) | ![NumPy](https://img.shields.io/badge/NumPy-Matrix_Factorization-013243?style=flat&logo=numpy&logoColor=white) | ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-PCA_Embeddings-F7931E?style=flat&logo=scikit-learn&logoColor=white) | ![Jupyter](https://img.shields.io/badge/Jupyter-Interactive_Labs-FA0F00?style=flat&logo=jupyter&logoColor=white) |

