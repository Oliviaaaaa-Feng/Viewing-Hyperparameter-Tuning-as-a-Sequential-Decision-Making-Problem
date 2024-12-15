# Hyperparameter Tuning as a Sequential Decision-Making Problem

## Overview
This project explores **Hyperparameter Optimization (HPO)** through the lens of sequential decision-making, addressing the inefficiencies of traditional methods like Grid Search and Random Search. By applying **Bayesian Optimization** and **Q-learning**, the project demonstrates how sequential methods can achieve superior performance with fewer evaluations, providing insights into balancing exploration and exploitation.

## Key Features
- **Sequential Decision-Making Framework**:
  - Framed HPO as a Markov Decision Process (MDP) with states, actions, transitions, and rewards.
  - Compared sequential methods (Bayesian Optimization, Q-learning) to traditional non-sequential methods (Grid Search, Random Search).
- **Bayesian Optimization**:
  - Utilized Gaussian Processes to model hyperparameter performance and guide sampling.
  - Implemented exploration methods like **Expected Improvement (EI)**, **Upper Confidence Bound (UCB)**, and greedy approaches.
- **Q-Learning**:
  - Applied model-free reinforcement learning with an ε-greedy strategy and reward-based feedback.
  - Balanced exploration and exploitation to optimize hyperparameters iteratively.
- **Experimental Setups**:
  - Conducted experiments across three setups:
    1. Decision Tree on a Digits Dataset.
    2. Self-defined black-box objective function for continuous spaces.
    3. SVM on Kaggle's Application Dataset.
  - Benchmarked algorithms on performance and computational efficiency.

## Results
- **Bayesian Optimization** outperformed Grid Search and Random Search in terms of accuracy and efficiency in most setups.
- **Q-Learning** showed promise but exhibited variability and instability due to sparse state-action exploration.
- Analysis of exploration methods highlighted UCB's faster convergence compared to EI and the limitations of greedy strategies in local maxima scenarios.

## Technologies Used
- **Programming**: Python
- **Algorithms**: Bayesian Optimization, Q-Learning
- **Libraries**: Scikit-learn, NumPy, Pandas
- **Visualization**: Matplotlib, Seaborn

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hpo-sequential.git
