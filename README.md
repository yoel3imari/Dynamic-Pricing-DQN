# Price Optimization with Deep Q-Networks

This project implements a reinforcement learning (RL) agent that learns dynamic pricing strategies in a simulated environment. The agent uses a Deep Q-Network (DQN) approach to optimize pricing decisions over a set time horizon.

The environment represents a simplified market scenario where each action corresponds to setting a price for a product. The state consists of current and historical pricing data as well as indicators reflecting previous actions. The RL agent interacts with the environment, learns from observed rewards, and updates its policy to maximize cumulative profit.

Key aspects of this project:
- **DQN Framework**: Utilizes PyTorch to build a feedforward policy network and a target network. The agent learns to approximate the Q-values of state-action pairs.
- **Exploration-Exploitation Trade-off**: An annealed epsilon-greedy policy balances exploration (random actions) and exploitation (greedy actions based on learned Q-values).
- **Replay Memory**: Experiences (state, action, next state, reward) are stored and sampled to stabilize learning.
- **Training Dynamics**: Includes periodic updates of the target network and use of smooth L1 (Huber) loss for robust learning.
- **Visualization**: The project plots the cumulative rewards (return trace), price schedules, and Q-values of actions. It also generates an animated GIF to illustrate how price decisions evolve over episodes.

The project highlights how reinforcement learning can be applied to sequential decision-making tasks in economics and business, such as dynamic pricing, showcasing how intelligent agents can adaptively learn to improve outcomes in changing environments.
