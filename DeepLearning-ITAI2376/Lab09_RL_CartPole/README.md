# Reinforcement Learning: Autonomous CartPole Agent

## Problem Statement
Reinforcement Learning (RL) is a paradigm of machine learning where an agent learns to make decisions by performing actions within an environment to maximize cumulative reward. This project focuses on training an autonomous agent to solve the classic control problem of CartPole: balancing a pole on a moving cart by applying precise left or right forces. Understanding these foundational RL concepts is critical for advanced applications like Reinforcement Learning from Human Feedback (RLHF) used in modern LLMs.

## Approach and Methodology
The project transitioned the agent from a state of random exploration to an optimized policy using Q-Learning:
1. **Environment Setup:** Utilized the `Gymnasium` library to instantiate the CartPole physics simulation.
2. **State Discretization:** Transformed the continuous state space (cart position, cart velocity, pole angle, pole angular velocity) into discrete bins to make the environment compatible with tabular Q-Learning.
3. **Q-Learning Implementation:** Engineered a Q-Learning agent from scratch. Implemented the Bellman equation to iteratively update the Q-table based on the agent's experiences, balancing immediate rewards against long-term optimal strategies.
4. **Epsilon-Greedy Policy:** Designed an exploration-exploitation strategy using an exponentially decaying epsilon value, allowing the agent to discover new tactics early in training and rely on learned knowledge later.

## Results and Evaluation
- **Baseline:** The random agent failed rapidly, surviving an average of only 22 steps per episode.
- **Trained Agent:** Following 500 episodes of Q-Learning, the agent successfully learned the optimal policy, consistently achieving the maximum possible survival score (500 steps) over consecutive evaluation episodes.
- Plotted the agent's learning curve, clearly visualizing the transition from exploration to exploitation and the convergence of the optimal policy.

## Learning Outcomes
- Mastered the mathematical foundations of Reinforcement Learning, specifically Markov Decision Processes (MDPs) and the Bellman Equation.
- Developed practical experience with the OpenAI/Farama `Gymnasium` ecosystem for simulation and agent testing.
- Demonstrated the ability to write robust algorithm implementations (Q-Learning) from mathematical theory to executable code.

## Dependencies and Data
- **Languages & Frameworks:** Python, Gymnasium (OpenAI Gym), NumPy, Matplotlib.
- **Environment:** CartPole-v1.
