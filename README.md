# Lab 6: Variance Reduction in Policy Gradient Methods
**MSDS Data Science Practicum | Regis University**

## Project Overview
This project implements and compares two Reinforcement Learning (RL) architectures—**Vanilla REINFORCE** and **REINFORCE with a Learned Baseline**—applied to the `CartPole-v1` environment. The goal is to demonstrate how a baseline (Critic) reduces gradient variance, leading to more stable and faster convergence in policy-based agents.

## Key Features
* **Actor-Critic Architecture:** Implemented using PyTorch for dynamic gradient management.
* **Variance Reduction:** Utilizes a Value Network to compute the Advantage Function $(G_t - V(s))$.
* **Performance Metrics:** Includes comparative learning curves, loss convergence, and agent trajectory stability plots.

## Results

### 1. Performance Comparison
![Impact of Variance Reduction](./visuals/Impact_of_Variance_Reduction.png)
*The Baseline agent (Blue) shows a significantly steeper learning curve and higher stability compared to the Vanilla agent (Red).*

### 2. Critic Convergence
![Critic Convergence](./visuals/Critic_Convergence.png)
*Mean Squared Error (MSE) loss for the Value Network demonstrates consistent convergence, providing a reliable baseline for the policy.*

### 3. Stability Distribution
![Stability Distribution](./visuals/Stability_Distribution.png)
*A frequency distribution of rewards proving that the Baseline method consistently hits the 500-reward threshold.*

## Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/yourusername/Lab6_Reinforce_Baseline.git](https://github.com/yourusername/Lab6_Reinforce_Baseline.git)
   cd Lab6_Reinforce_Baseline
