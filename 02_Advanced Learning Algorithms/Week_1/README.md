
# 🧠 Neural Network Architectures & Forward Propagation

Welcome to Week 1 of **Advanced Learning Algorithms** (Course 2 of the Stanford University & DeepLearning.AI Machine Learning Specialization)! This module introduces deep learning, transitioning from linear and logistic models to artificial neural networks, multi-layer activation computations, TensorFlow sequential model construction, and low-level matrix forward propagation from scratch in NumPy.

---

## 📝 Core Technical Objectives
* **Neural Network Foundations:** Understanding biological neuron analogies, layer abstractions (input, hidden, output), and how intermediate layers learn abstract feature representations.
* **Forward Propagation Mechanics:** Calculating layer activations $\mathbf{a}^{[l]} = g(\mathbf{W}^{[l]} \mathbf{a}^{[l-1]} + \mathbf{b}^{[l]})$ across dense feedforward networks.
* **Production Framework Construction:** Building sequential neural networks using TensorFlow `Keras` APIs (`tf.keras.Sequential`, `tf.keras.layers.Dense`).
* **Low-Level Array Vectorization:** Implementing manual forward propagation loops and batch matrix multiplication ($\mathbf{A}^{[l]} = g(\mathbf{A}^{[l-1]} \mathbf{W}^{[l]} + \mathbf{B}^{[l]} presidency)$) from scratch in pure Python/NumPy.

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

This module's core video lectures, interactive Jupyter notebooks, and practice assignments are mapped directly to their targeted analytical focus:

| Asset / Deliverable | Operational Focus |
| :--- | :--- |
| **[Neurons and Layers](./01_Neurons_and_Layers.ipynb)** | Exploring single-neuron sigmoid activations and dense layer construction using basic NumPy and TensorFlow. |
| **[Coffee Roasting in TensorFlow](./02_CoffeeRoasting_TF.ipynb)** | Constructing a 2-layer sequential neural network in TensorFlow to solve a multi-feature binary classification task (temperature vs. duration). |
| **[Coffee Roasting in NumPy](./03_CoffeeRoasting_Numpy.ipynb)** | Implementing forward propagation, layer matrix transformations, and activation calculations completely from scratch in NumPy. |
| **Neural Networks for Binary Classification Assignment** | Graded programming project building an end-to-end multi-layer neural network in TensorFlow to perform handwritten digit recognition. |

---

## 💡 Visual Pipeline Reference

The deep learning forward propagation workflow implemented across this module:

* **Raw Feature Ingestion** ➔ Ingest input tensor $\mathbf{x} \in \mathbb{R}^n$ as activation vector $\mathbf{a}^{[0]}$.
* **Layer-by-Layer Transformation** ➔ Compute linear combination $\mathbf{z}^{[l]} = \mathbf{W}^{[l]} \mathbf{a}^{[l-1]} + \mathbf{b}^{[l]}$ for layer $l$.
* **Non-Linear Activation** ➔ Pass through activation function $\mathbf{a}^{[l]} = g(\mathbf{z}^{[l]})$ (e.g., Sigmoid, ReLU).
* **Final Output Inference** ➔ Evaluate final output layer $\mathbf{a}^{[L]}$ to output binary predictions or class probabilities $P(y=1\vert{}\mathbf{x})$.

---

## 🎯 Technical Skills Architecture

### 📊 Deep Learning Theory
* **Hierarchical Feature Learning:** Understanding how hidden layers transform raw features into higher-level representations automatically.
* **Activation Function Dynamics:** Analyzing non-linear activations ($g(z)$) and their role in breaking linear model bounds.
* **Matrix Operations & Vectorization:** Utilizing linear algebra matrix multiplication rules ($\mathbf{A} \cdot \mathbf{W}$) for high-throughput batch parallel inference.

### 🤖 Applied Machine Learning Engineering
* **TensorFlow Model Architecture:** Defining and compiling neural network graphs using `tf.keras.Sequential` and `tf.keras.layers.Dense`.
* **Custom Inference Engine:** Writing modular NumPy loop structures for neural network forward pass computations without framework abstractions.
* **Tensor Formatting & Manipulation:** Managing array dimensions, column vectors, and weight matrix alignments across model boundaries.

---

## 🛠️ Production Tech Stack & Ecosystem

| Deep Learning Framework | Vectorized Matrix Operations | Data Visualization | Development Environment |
| :---: | :---: | :---: | :---: |
| ![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-FF6F00?style=flat&logo=tensorflow&logoColor=white) | ![NumPy](https://img.shields.io/badge/NumPy-Matrix_Multiplication-013243?style=flat&logo=numpy&logoColor=white) | ![Matplotlib](https://img.shields.io/badge/Matplotlib-Activation_Plotting-11557c?style=flat&logo=python&logoColor=white) | ![Jupyter](https://img.shields.io/badge/Jupyter-Interactive_Labs-FA0F00?style=flat&logo=jupyter&logoColor=white) |

