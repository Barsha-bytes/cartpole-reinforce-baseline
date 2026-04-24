# Lab 6: Variance Reduction in Policy Gradient Methods
**MSDS Data Science Practicum | Barsha Kakshapati**

## Project Overview
This project compares **Vanilla REINFORCE** and **REINFORCE with a Learned Baseline** in the `CartPole-v1` environment. The goal is to prove that a baseline reduces gradient variance for more stable convergence.



## Key Results

### 1. Performance Comparison
![Impact of Variance Reduction](./visuals/Impact%20of%20Variance%20Reduction.png)
*The Baseline agent (Blue) demonstrates a steeper and more consistent learning curve than the Vanilla agent (Red).*

### 2. Critic Convergence
![Critic Convergence](./visuals/Critic%20Convergence.png)
*The decline in MSE loss indicates the Value Network is successfully learning the state-value function.*

### 3. Stability Distribution
![Stability Distribution](./visuals/Stability%20Distribution.png)
*The Baseline method shows a high-frequency spike at the 500-reward mark, proving it is more robust against noise.*

### 4. Trained Agent Stability
![Trained Agent Stability](./visuals/Trained%20Agent%20Stability.png)
*Trajectory plot showing the agent actively correcting the pole angle to maintain balance.*

## Installation & Reproducibility
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`.
3. Run the notebook located in the `notebooks/` directory.

## Repository Structure
```text
├── notebooks/
│   └── Lab6_Reinforce.ipynb
├── visuals/                  # Ensure your 4 images are inside this folder
├── requirements.txt
└── README.md
