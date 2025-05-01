# 🔬 Hybrid Quantum-Classical Reinforcement Learning on FrozenLake (8x8)

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

## 📊 Summary of Results

| Algorithm         | Non-Slippery Success | Slippery Success | Avg. Reward | Avg. Steps | Training Time |
|------------------|----------------------|------------------|-------------|------------|----------------|
| **Q-Learning**    | ~80.5–80.7%          | ~11.4–11.6%      | ~0.80 / ~0.07 | ~43 / ~15   | ~10–15 mins     |
| **DQN**           | 100%                 | ~71–80%          | ~0.2 / ~0.5–1.0 | 6 / 41–66  | ~30–40 mins     |
| **Quantum Hybrid**| 100% (possible overfit) | ~35–65%       | ~0.2–0.3 / ~-0.5 | 6 / 10–56  | ~1–2 hours      |

### 📈 Key Metrics
- **Cumulative Success Rate**
- **Average Reward per Episode**
- **Rolling Success Rate (100 episodes)**
- **Average Steps per Episode**
- **Training Time**
- **Quantum Circuit Depth & Shots**

### 🧪 Equations Used
- Cumulative success rate  
  \[
  \text{Success Rate} = \frac{\text{Successful Episodes}}{\text{Total Episodes}}
  \]
- Average reward  
  \[
  \text{Avg. Reward} = \frac{1}{N} \sum_{i=1}^N \sum_{t=1}^{T_i} R(s_t, a_t, s_{t+1})
  \]
- Average steps  
  \[
  \text{Avg. Steps} = \frac{1}{N} \sum_{i=1}^N T_i
  \]
- Q-table change  
  \[
  \Delta Q = \sqrt{\sum_{s, a} \left[ Q_{\text{new}}(s, a) - Q_{\text{old}}(s, a) \right]^2}
  \]

---

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

---

## 📁 File Structure

