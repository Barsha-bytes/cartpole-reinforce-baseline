# Lab 6: Variance Reduction in Policy Gradient Methods
**MSDS Data Science Practicum | Regis University**

## Project Overview
This project implements and compares two Reinforcement Learning (RL) architectures—**Vanilla REINFORCE** and **REINFORCE with a Learned Baseline**—applied to the `CartPole-v1` environment. The goal is to demonstrate how a baseline (Critic) reduces gradient variance, leading to more stable and faster convergence.

## Results

### 1. Performance Comparison (Variance Reduction)
![Impact of Variance Reduction](./visuals/Impact of Variance Reduction.png)
*The Baseline agent (Blue) reaches the 500-reward threshold more consistently than the Vanilla agent (Red), demonstrating reduced gradient variance.*

### 2. Critic Convergence (MSE Loss)
![Critic Convergence](./visuals/Critic Convergence.png)
*The downward trend in the Value Network's Mean Squared Error (MSE) confirms the baseline is successfully learning to predict state values.*

### 3. Trained Agent Stability
![Trained Agent Stability](./visuals/Trained Agent Stability.png)
*A trajectory plot of the pole angle during a test episode, showing the agent's ability to maintain balance through active corrections.*

### 4. Reward Distribution
![Stability Distribution](./visuals/Stability Distribution.png)
*The histogram shows the Baseline method (Blue) consistently achieving maximum rewards compared to the high-failure rate of the Vanilla method.*

## Installation & Usage
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`.
3. Run the notebook in the `notebooks/` directory.

## Repository Structure
```text
├── notebooks/
│   └── Lab6_Reinforce.ipynb
├── visuals/                  <-- Put your 4 PNG images here!
│   ├── Impact of Variance Reduction.png
│   ├── Critic Convergence.png
│   ├── Trained Agent Stability.png
│   └── Stability Distribution.png
├── requirements.txt
└── README.md
