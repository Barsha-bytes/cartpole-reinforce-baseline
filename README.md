# Lab 6: Variance Reduction in Policy Gradient Methods
**MSDS Data Science Practicum | Barsha Kakshapati**

## Project Overview
This project implements and compares **Vanilla REINFORCE** and **REINFORCE with a Learned Baseline** using `CartPole-v1`. The goal is to prove that a baseline (Critic) reduces gradient variance for more stable convergence.

## Key Results

### 1. Performance Comparison
![Impact of Variance Reduction](./visuals/Impact%20of%20Variance%20Reduction.png)
*The Baseline agent (Blue) demonstrates a steeper and more consistent learning curve compared to the Vanilla agent (Red).*

### 2. Critic Convergence
![Critic Convergence](./visuals/Critic%20Convergence.png)
*The decline in MSE loss indicates the Value Network is successfully learning the state-value function.*

### 3. Stability Distribution
![Stability Distribution](./visuals/Stability%20Distribution.png)
*The histogram shows the Baseline method consistently achieving maximum rewards.*

### 4. Trained Agent Stability
![Trained Agent Stability](./visuals/Trained%20Agent%20Stability.png)
*Trajectory plot of the pole angle during a 500-step test episode.*

## Installation
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`.

## Repository Structure
```text
├── visuals/                  <-- Images MUST be in this folder
│   ├── Impact of Variance Reduction.png
│   ├── Critic Convergence.png
│   ├── Trained Agent Stability.png
│   └── Stability Distribution.png
├── requirements.txt
└── README.md
