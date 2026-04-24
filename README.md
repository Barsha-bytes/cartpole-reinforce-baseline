# Lab 6: Variance Reduction in Policy Gradient Methods
**MSDS Data Science Practicum | Barsha Kakshapati**

## Project Overview
This project implements and compares **Vanilla REINFORCE** and **REINFORCE with a Learned Baseline** using the `CartPole-v1` environment. The primary objective is to demonstrate how a baseline (Critic) reduces gradient variance, leading to faster and more stable convergence.

## Key Results

### 1. Performance Comparison
![Impact of Variance Reduction](./visuals/Impact%20of%20Variance%20Reduction.png)
*The Baseline agent (Blue) demonstrates a steeper learning curve and higher reliability compared to the Vanilla agent (Red).*

### 2. Critic Convergence
![Critic Convergence](./visuals/Critic%20Convergence.png)
*The downward trend in the Value Network's Mean Squared Error (MSE) indicates successful learning of the state-value function.*

### 3. Stability Distribution
![Stability Distribution](./visuals/Stability%20Distribution.png)
*The histogram shows the Baseline method consistently achieving maximum rewards of 500, whereas the Vanilla method is prone to early failure.*

### 4. Trained Agent Stability
![Trained Agent Stability](./visuals/Trained%20Agent%20Stability.png)
*A trajectory plot of the pole angle during a 500-step test episode, showing the agent's ability to maintain balance through active corrections.*

## Repository Structure
```text
├── visuals/                  # Contains the 4 PNG images
├── requirements.txt          # Library dependencies
└── README.md                 # Project documentation
