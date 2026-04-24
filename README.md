# Lab 6: Variance Reduction in Policy Gradient Methods
**MSDS Data Science Practicum | Barsha Kakshapati**

## Project Overview
[cite_start]This project compares **Vanilla REINFORCE** and **REINFORCE with a Learned Baseline** in the `CartPole-v1` environment[cite: 100]. [cite_start]The goal is to prove that a baseline reduces gradient variance for more stable convergence[cite: 101].

## Key Results

### 1. Performance Comparison
![Impact of Variance Reduction](./visuals/Impact of Variance Reduction.png)
[cite_start]*The Baseline agent (Blue) demonstrates a steeper and more consistent learning curve than the Vanilla agent (Red)[cite: 128, 129].*

### 2. Critic Convergence
![Critic Convergence](./visuals/Critic Convergence.png)
[cite_start]*The decline in MSE loss indicates the Value Network is successfully learning the state-value function[cite: 145].*

### 3. Stability Distribution
![Stability Distribution](./visuals/Stability Distribution.png)
[cite_start]*The Baseline method shows a high-frequency spike at the 500-reward mark, proving it is more robust against noise[cite: 167, 168].*

### 4. Trained Agent Stability
![Trained Agent Stability](./visuals/Trained Agent Stability.png)
[cite_start]*Trajectory plot showing the agent actively correcting the pole angle to maintain balance[cite: 182, 183].*

## Installation
1. Clone the repo.
2. Install dependencies: `pip install -r requirements.txt`.
