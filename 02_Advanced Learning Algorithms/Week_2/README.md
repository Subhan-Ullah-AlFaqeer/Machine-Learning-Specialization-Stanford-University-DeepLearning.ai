
# ⚡ Neural Network Training, Multiclass Classification & Backpropagation

Welcome to Week 2 of **Advanced Learning Algorithms** (Course 2 of the Stanford University & DeepLearning.AI Machine Learning Specialization)! This module expands neural network capabilities beyond binary classification, covering hidden layer activation functions (ReLU vs. Sigmoid vs. Linear), numerical stability in Softmax loss calculation, advanced optimizers like Adam, and the calculus of backpropagation via computation graphs.

---

## 📝 Core Technical Objectives
* **Activation Function Dynamics:** Choosing layer activations based on non-linear mapping needs (ReLU for hidden layers, Sigmoid for binary output, Linear for continuous regression, Softmax for multiclass).
* **Multiclass Classification Framework:** Formulating Softmax outputs $a_k = \frac{e^{z_k}}{\sum_{j=1}^N e^{z_j}}$ and Sparse Categorical Cross-Entropy loss to output probability distributions over $N$ mutually exclusive classes.
* **Numerical Stability (`from_logits=True`):** Computing loss directly on linear logits ($z$) to prevent floating-point underflow/overflow during intermediate exponential steps.
* **Advanced Optimization & Backprop Calculus:** Utilizing the Adam (Adaptive Moment Estimation) optimizer and understanding automatic differentiation through computation graphs.

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

This module's core video lectures, interactive Jupyter notebooks, and practice assignments are mapped directly to their targeted analytical focus:

| Asset / Deliverable | Operational Focus |
| :--- | :--- |
| **[ReLU Activation Lab](./Relu.ipynb)** | Visualizing Rectified Linear Unit (ReLU) $g(z) = \max(0, z)$ behavior, addressing dead neuron issues, and comparing performance against Sigmoid activations. |
| **[Softmax Function Lab](./SoftMax.ipynb)** | Calculating Softmax activations for multi-class distributions and observing probability shifts across changing input logit scales. |
| **[Multiclass TensorFlow Lab](./Multiclass_TF.ipynb)** | Building and compiling multi-class neural networks in TensorFlow using `SparseCategoricalCrossentropy(from_logits=True)`. |
| **[Derivatives Lab](./Derivatives.ipynb)** | Computing partial derivatives numerically and symbolically to build mathematical intuition for parameter slope updates. |
| **[Backpropagation Lab](./Backprop.ipynb)** | Tracing forward and backward passes across computation graphs to evaluate intermediate local gradients and global parameter updates. |
| **Multiclass Classification Assignment** | Graded programming project training a multi-layer neural network in TensorFlow with Softmax activations for handwritten digit classification. |

---

## 💡 Visual Pipeline Reference

The multiclass neural network training and optimization workflow implemented across this module:

* **Layer Activations (ReLU)** ➔ Hidden layers execute non-linear transformations $\mathbf{a}^{[l]} = \max(0, \mathbf{W}^{[l]} \mathbf{a}^{[l-1]} + \mathbf{b}^{[l]})$.
* **Logit Generation** ➔ Output layer outputs unscaled continuous values $\mathbf{z}^{[L]} = \mathbf{W}^{[L]} \mathbf{a}^{[L-1]} + \mathbf{b}^{[L]}$.
* **Numerically Stable Loss** ➔ Pass raw logits $\mathbf{z}^{[L]}$ into `SparseCategoricalCrossentropy(from_logits=True)` for loss optimization.
* **Adaptive Gradient Optimization** ➔ Update weights using **Adam Optimizer**, adjusting individual learning rates per parameter based on running momentum estimates.

---

## 🎯 Technical Skills Architecture

### 📊 Deep Learning Theory
* **Non-Linear Representation Need:** Demonstrating why neural networks without non-linear activations collapse into simple linear regression models regardless of depth.
* **Categorical Cross-Entropy Mechanics:** Evaluating loss $L(\mathbf{a}, y) = -\log(a_y)$ for ground-truth class $y$ and measuring prediction confidence.
* **Computational Graph Calculus:** Applying the calculus chain rule to compute gradients $\frac{\partial J}{\partial \mathbf{W}^{[l]}}$ backwards from loss output to input features.

### 🤖 Applied Machine Learning Engineering
* **TensorFlow Loss Optimization:** Implementing numerically robust Softmax pipelines in `tf.keras` by decoupling logits from standalone activations.
* **Adam Optimization Setup:** Configuring adaptive momentum optimizers (`tf.keras.optimizers.Adam(learning_rate=0.001)`) for accelerated training convergence.
* **Multi-Class vs. Multi-Label Design:** Distinguishing between mutually exclusive categorical classification (Softmax) and independent multi-label classification (Sigmoid output array).

---

## 🛠️ Production Tech Stack & Ecosystem

| Deep Learning Framework | Numerical Optimization | Visualization & Analytics | Development Environment |
| :---: | :---: | :---: | :---: |
| ![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras_APIs-FF6F00?style=flat&logo=tensorflow&logoColor=white) | ![Adam](https://img.shields.io/badge/Optimizer-Adam_Adaptive-013243?style=flat&logo=python&logoColor=white) | ![Matplotlib](https://img.shields.io/badge/Matplotlib-Derivative_Plots-11557c?style=flat&logo=python&logoColor=white) | ![Jupyter](https://img.shields.io/badge/Jupyter-Interactive_Labs-FA0F00?style=flat&logo=jupyter&logoColor=white) |

