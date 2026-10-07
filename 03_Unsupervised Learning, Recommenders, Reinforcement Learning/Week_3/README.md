
# 🚀 Reinforcement Learning: Bellman Equations, State-Action Value Functions & Deep Q-Networks (DQN)

Welcome to Week 3 of **Unsupervised Learning, Recommenders, Reinforcement Learning** (Course 3 of the Stanford University & DeepLearning.AI Machine Learning Specialization)! This final module transitions into Markov Decision Processes (MDPs) and Reinforcement Learning (RL): discount factors, policies, Bellman equations, state-action value functions $Q(s, a)$, continuous state spaces, $\epsilon$-greedy exploration, experience replay mini-batches, soft target updates, and Deep Q-Networks (DQN) applied to land a virtual lunar module safely.

---

## 📝 Core Technical Objectives
* **Markov Decision Process (MDP) Framework:** Modeling agent-environment interactions via states $s$, actions $a$, rewards $r$, next states $s'$, discount factor $\gamma \in [0, 1)$, and policy $\pi(s)$.
* **Discounted Return & Policy Optimization:** Maximizing expected cumulative discounted return $R_t = \sum_{k=0}^{\infty} \gamma^k r_{t+k+1}$ to prioritize immediate vs. long-term strategic rewards.
* **Bellman Equation Formulation:** Expressing state-action value recursively via $Q^*(s, a) = R(s, a) + \gamma \max_{a'} Q^*(s', a')$.
* **Deep Q-Network (DQN) Architecture:** Utilizing a neural network $Q(s, a; \mathbf{w})$ to approximate $Q^*$-values for continuous state spaces and selecting actions via an $\epsilon$-greedy exploration policy.
* **DQN Convergence Stabilization:** Implementing Experience Replay buffers (mini-batch sampling to break temporal correlation) and Target Network Soft Updates $\mathbf{w}^- \leftarrow \tau \mathbf{w} + (1 - \tau) \mathbf{w}^-$ to prevent moving-target divergence.

---

## 🧪 Interactive Laboratory & Visual Selection Matrix

This module's core video lectures, interactive Jupyter notebooks, and practice assignments are mapped directly to their targeted analytical focus:

| Asset / Deliverable | Operational Focus |
| :--- | :--- |
| **[State-Action Value Function Lab](./State-action%20value%20function%20example.ipynb)** | Calculating tabular $Q(s, a)$ matrices manually across discrete grid environments to visualize optimal policy trajectories $\pi^*(s) = \arg\max_a Q^*(s,a)$. |
| **[Deep Q-Network Lunar Lander Assignment](./Assignment.ipynb)** | Graded programming project building a complete Deep Q-Network in TensorFlow and OpenAI Gym/Gymnasium to control thrusters and land a space module smoothly on a target pad. |

---

## 💡 Visual Pipeline Reference

The Deep Q-Learning (DQN) agent-environment loop and neural network training process implemented across this module:

* **Environment State Perception** ➔ Observe continuous state vector $\mathbf{s}_t \in \mathbb{R}^n$ (position, velocity, angle, angular velocity, ground contacts).
* **$\epsilon$-Greedy Action Selection** ➔ With probability $\epsilon$, choose random action $a_t$ (exploration); otherwise select $a_t = \arg\max_a Q(\mathbf{s}_t, a; \mathbf{w})$ (exploitation).
* **Experience Replay Memory** ➔ Store transition tuple $(\mathbf{s}_t, a_t, r_t, \mathbf{s}_{t+1}, \text{done})$ into Replay Buffer $\mathcal{D}$.
* **Neural Network Optimization Step**:
  * Sample mini-batch of experiences from $\mathcal{D}$.
  * Compute target $y_j = r_j + \gamma (1 - \text{done}_j) \max_{a'} Q(\mathbf{s}'_j, a'; \mathbf{w}^-)$ using target network weights $\mathbf{w}^-$.
  * Minimize Mean Squared Error (MSE) loss $\mathcal{L}(\mathbf{w}) = \frac{1}{B} \sum_{j=1}^B \left( y_j - Q(\mathbf{s}_j, a_j; \mathbf{w}) \right)^2$.
* **Soft Weight Update** ➔ Update target network weights gradually: $\mathbf{w}^- \leftarrow \tau \mathbf{w} + (1 - \tau) \mathbf{w}^-$ where $\tau \ll 1$.

---

## 🎯 Technical Skills Architecture

### 📊 Reinforcement Learning Theory
* **Markovian Property Mechanics:** Assuming future state probabilities depend exclusively on current state $s_t$ and action $a_t$, independent of past history.
* **Exploration vs. Exploitation Trade-off:** Managing decay schedules for $\epsilon$-greedy strategies ($\epsilon \to \epsilon_{\min}$) to balance domain discovery against cumulative reward maximization.
* **Target Instability Control:** Resolving overestimation bias and moving target oscillations by separating evaluation network parameters $\mathbf{w}$ from target parameters $\mathbf{w}^-$.

### 🤖 Applied Machine Learning Engineering
* **Custom Keras Q-Network Construction:** Building fully connected neural networks mapping continuous state vectors to multi-action $Q$-value outputs.
* **Memory-Efficient Replay Buffers:** Implementing deque/array data structures to store, shuffle, and sample batch transitions efficiently during online learning.
* **OpenAI Gym / Gymnasium Integration:** Environment lifecycle management (`env.reset()`, `env.step(action)`), state vector normalization, and frame rendering.

---

## 🛠️ Production Tech Stack & Ecosystem

| Deep Learning Framework | RL Environment Ecosystem | Numerical Optimization | Development Environment |
| :---: | :---: | :---: | :---: |
| ![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x_Keras-FF6F00?style=flat&logo=tensorflow&logoColor=white) | ![Gymnasium](https://img.shields.io/badge/OpenAI_Gym-Lunar_Lander_v2-0081C8?style=flat&logo=openai&logoColor=white) | ![NumPy](https://img.shields.io/badge/NumPy-Replay_Buffers-013243?style=flat&logo=numpy&logoColor=white) | ![Jupyter](https://img.shields.io/badge/Jupyter-Interactive_Labs-FA0F00?style=flat&logo=jupyter&logoColor=white) |

