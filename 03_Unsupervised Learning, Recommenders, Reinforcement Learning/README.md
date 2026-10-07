
# 🤖 Course 3: Unsupervised Learning, Recommenders, Reinforcement Learning

Welcome to the root repository for **Course 3: Unsupervised Learning, Recommenders, Reinforcement Learning**, the third and final core module of the **Stanford University & DeepLearning.AI Machine Learning Specialization**, taught by Andrew Ng.

This course transitions beyond traditional supervised paradigms into advanced unsupervised learning methodologies (K-Means clustering and Gaussian anomaly detection), industrial-scale recommender system architectures (Collaborative Filtering and Dual-Tower Deep Content-Based Filtering), and Deep Reinforcement Learning (Q-Learning and Deep Q-Networks).

---

## 📝 Core Technical Objectives
* **Unsupervised Clustering & Density Estimation:** Implementing the iterative K-Means algorithm (centroid updates and distortion cost minimization) and Gaussian probability density estimation $p(\mathbf{x}) < \epsilon$ for anomaly detection.
* **Matrix Factorization Recommenders:** Formulating collaborative filtering to simultaneously learn user preferences $\mathbf{w}^{(u)}, b^{(u)}$ and item feature embeddings $\mathbf{x}^{(i)}$, optimized using TensorFlow custom training loops (`tf.GradientTape`) with mean normalization.
* **Dual-Tower Content-Based Deep Learning:** Training user and item neural networks in TensorFlow/Keras to output matching vector embeddings $\mathbf{v}_u$ and $\mathbf{v}_m$ for large-scale catalog retrieval and ranking.
* **Dimensionality Reduction via PCA:** Computing Principal Component Analysis transformations to reduce high-dimensional feature spaces while preserving maximum variance.
* **Deep Reinforcement Learning (DQN):** Modeling Markov Decision Processes (MDPs), solving Bellman optimality recurrences, and training Deep Q-Networks (DQN) with Experience Replay buffers and soft target updates for continuous state-space control tasks.

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

The course is structured across three comprehensive weekly modules detailing theoretical foundations, interactive labs, and practical algorithm implementations:

| Module / Directory | Analytical Focus | Key Implementations & Labs |
| :--- | :--- | :--- |
| **[Week 1: Unsupervised Learning](./Week_1)** | K-Means clustering iterative optimization, image quantization compression, Gaussian anomaly detection, and feature transformation. | `KMeans_Assignment`, `Anomaly_Detection`, Server Outlier Detection, Image Color Compression. |
| **[Week 2: Recommender Systems](./Week_2)** | Matrix factorization collaborative filtering, mean normalization, dual-tower neural network embeddings, and PCA visualization. | `Collaborative_RecSys_Assignment`, `RecSysNN_Assignment`, Movie Recommendation Engine, PCA Lab. |
| **[Week 3: Reinforcement Learning](./Week_3)** | Markov Decision Processes (MDPs), Bellman equations, $Q(s, a)$ value functions, continuous state spaces, and Deep Q-Networks. | `State-action value function example`, `Assignment` (Lunar Lander DQN Agent in OpenAI Gym). |

---

## 💡 Visual Pipeline Reference

The comprehensive unsupervised, recommender, and reinforcement learning pipeline executed throughout Course 3:

* **Unsupervised Structure Discovery** ➔ Cluster unlabeled data via **K-Means** or isolate rare anomalous patterns using **Gaussian Joint Densities** $p(\mathbf{x})$.
* **Multi-Stage Recommender Pipeline**:
  * **Collaborative Layer** ➔ Factorize rating matrices using `tf.GradientTape()` with **Mean Normalization**.
  * **Deep Content Layer** ➔ Map User $\mathbf{x}_u$ and Item $\mathbf{x}_m$ features through **Dual-Tower Neural Networks** to compute similarity dot products $\mathbf{v}_u \cdot \mathbf{v}_m$.
* **Dimensionality Reduction** ➔ Compress high-dimensional representations via **PCA** projection axes.
* **Sequential Control Loop (DQN)** ➔ Agent perceives continuous state $\mathbf{s}$ ➔ Selects action $a$ via $\epsilon$-greedy strategy ➔ Stores transitions in **Replay Memory** ➔ Optimizes $Q(\mathbf{s}, a; \mathbf{w})$ with **Soft Target Network Updates** $\mathbf{w}^-$.

---

## 🎯 Technical Skills Architecture

### 📊 Advanced Machine Learning Theory
* **Unsupervised Latent Representations:** Mathematical formulation of K-Means distortion cost $J$, matrix factorization lower-rank embeddings, and principal components.
* **Recommender Engineering Mechanics:** Managing cold-start scenarios via content networks, separating retrieval from ranking stages, and applying mean normalization.
* **Markov Decision Dynamics:** Solving recursive Bellman optimality equations $Q^*(s, a) = R(s, a) + \gamma \max_{a'} Q^*(s', a')$ for stochastic/continuous environments.

### 🤖 Applied Machine Learning Engineering
* **Custom TensorFlow Pipelines:** Implementing non-standard auto-differentiation using `tf.GradientTape` for collaborative filtering and constructing multi-input dual-tower architectures.
* **Stabilized Deep Q-Learning:** Engineering memory-efficient experience replay buffers and soft parameter updating to eliminate moving-target divergence in DQNs.
* **Production Environment Interfaces:** Integrating RL agents with standard control simulation frameworks (`gymnasium` / `openai-gym`).

---

## 🛠️ Production Tech Stack & Ecosystem

| Deep Learning Framework | RL Simulation Ecosystem | Numerical Computing & Analytics | Development Environment |
| :---: | :---: | :---: | :---: |
| ![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x_Keras-FF6F00?style=flat&logo=tensorflow&logoColor=white) | ![Gymnasium](https://img.shields.io/badge/OpenAI_Gym-Lunar_Lander-0081C8?style=flat&logo=openai&logoColor=white) | ![NumPy](https://img.shields.io/badge/NumPy-Matrix_Ops-013243?style=flat&logo=numpy&logoColor=white) ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-PCA_%26_Cluster-F7931E?style=flat&logo=scikit-learn&logoColor=white) | ![Jupyter](https://img.shields.io/badge/Jupyter-Interactive_Labs-FA0F00?style=flat&logo=jupyter&logoColor=white) |

