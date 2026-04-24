# Lab 6: Variance Reduction in Policy Gradient Methods
**MSDS Data Science Practicum | Barsha Kakshapati**

## Project Overview
This project implements and compares **Vanilla REINFORCE** and **REINFORCE with a Learned Baseline** using `CartPole-v1`. The goal is to empirically demonstrate that a baseline (Critic) reduces gradient variance, leading to more stable convergence.

## Key Results

### 1. Performance Comparison (Variance Reduction)
![Impact of Variance Reduction](./visuals/Impact of Variance Reduction.png)
*The Baseline agent (Blue) demonstrates a steeper and more consistent learning curve compared to the Vanilla agent (Red).*

### 2. Critic Convergence (MSE Loss)
![Critic Convergence](./visuals/Critic Convergence.png)
*Mean Squared Error (MSE) decline proves the Value Network successfully learned the state-value function.*

### 3. Stability Distribution
![Stability Distribution](./visuals/Stability Distribution.png)
*The histogram confirms the Baseline method (Blue) consistently reaches the 500-reward threshold.*

### 4. Trained Agent Stability
![Trained Agent Stability](./visuals/Trained Agent Stability.png)
*Trajectory plot of the pole angle during a 500-step test, showing active balancing behavior.*

## Repository Structure
```text
├── visuals/                  <-- YOU MUST CREATE THIS FOLDER
│   ├── Impact of Variance Reduction.png
│   ├── Critic Convergence.png
│   ├── Trained Agent Stability.png
│   └── Stability Distribution.png
├── requirements.txt
└── README.md
