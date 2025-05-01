# 🔬Comparative study of Q-Learning, Deep Q-Network (DQN), and Hybrid Quantum Q-Learning on FrozenLake using classical and quantum reinforcement learning techniques.

This repository contains a comprehensive experiment comparing **Q-Learning**, **Deep Q-Network (DQN)**, and a **Hybrid Quantum Q-Learning** algorithm using the OpenAI Gym FrozenLake-v1 environment (8x8 grid), both in slippery and non-slippery modes.

🚀 The goal: To understand how classical vs deep vs quantum-enhanced reinforcement learning performs under different environments, with a special focus on quantum circuit performance, training time, and reward convergence.

---

## 📚 Project Overview

### 🎯 Objectives
- Establish a strong Q-Learning baseline.
- Use DQNs to harness the power of deep neural networks.
- Introduce quantum noise and circuit dynamics with a hybrid Q-learning model using PennyLane.
- Evaluate success rate, cumulative rewards, training time, average steps, and more across all models.
- Test performance under both **deterministic (non-slippery)** and **stochastic (slippery)** conditions.

### 🔍 Environments
- `FrozenLake-v1 (8x8)` from OpenAI Gym
- Configured for both `is_slippery = False` and `is_slippery = True`

---


### 📈 Key Metrics
- **Cumulative Success Rate**
- **Average Reward per Episode**
- **Rolling Success Rate (100 episodes)**
- **Average Steps per Episode**
- **Training Time**
- **Quantum Circuit Depth & Shots**



## 🧠 Technologies Used

| Library      | Purpose                              |
|--------------|--------------------------------------|
| Python       | Core programming language            |
| NumPy        | Efficient numerical computation      |
| Matplotlib   | Visualization                        |
| OpenAI Gym   | FrozenLake RL environment            |
| PyTorch      | Deep Q-Network implementation        |
| PennyLane    | Quantum circuit integration          |
| Google Colab | Cloud-based experimentation          |



