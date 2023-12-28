# Deep-Reinforcement-Learning-in-OpenAI-Gym-
Implementation of Q-learning to solve the Taxi-v3 game from OpenAI Gym

## Overview
This project showcases the implementation of Q-learning to solve the Taxi-v3 game from OpenAI Gym. This game serves as an excellent reinforcement learning problem, featuring a simple environment with small state and action spaces. It provides an ideal example of the exploration-exploitation trade-off, aiming to train the agent to navigate a taxi in a grid-world environment for passenger pickup and drop-off.

### Environment
The environment consists of a 5x5 grid with 500 possible states representing the passenger's location and destination. The agent receives rewards between -10 and 20 for each action taken, where correct drop-offs yield positive rewards, and incorrect actions or drop-offs result in negative rewards.

## Animation
The `animationVisual()` function generates an animated visualization of the game. It renders frames depicting the game's state, episode number, action taken, reward earned, and epoch number. Using Q-learning, the function captures images at each time step, producing an RGB representation of the game state. These images compile into an animated GIF, showcasing the agent's navigation.

## Training
Training involves the `trainTaxi()` function, implementing the Q-learning algorithm. With epsilon-greedy action selection, the algorithm aims to maximize rewards over time. The Q-learning equation guides the learning process, updating the Q-table based on rewards, discount factor, and learning rate. Plots of total rewards and failed deliveries across episodes depict the agent's learning progress.

![Training](https://github.com/sacadelmi/Deep-Reinforcement-Learning-in-OpenAI-Gym-/blob/main/Training.png)

## Results
The `runSimulation()` function tests the trained agent across multiple episodes. Rendered frames from simulations create an animated visualization, revealing the agent's decision-making process. Key metrics, including average epochs per episode and failed drop-offs, indicate the agent's performance. The agent demonstrates successful navigation with minimal failed deliveries and a low average number of epochs per episode.

### Example Simulation
#### Initial Environment:**

![Initial Environment](https://github.com/sacadelmi/Deep-Reinforcement-Learning-in-OpenAI-Gym-/blob/main/start.png)

#### Final Environment:**

![Final Environment](https://github.com/sacadelmi/Deep-Reinforcement-Learning-in-OpenAI-Gym-/blob/main/end.png)

#### Simulation Data:
- Average epochs per episode: 15.0
- Average failed drop-offs per episode: 0.0

## Conclusion
Through Q-learning and the exploration-exploitation trade-off, the trained agent achieves an optimal policy, maximizing cumulative rewards while successfully navigating the environment. With minimal failed deliveries and efficient navigation, the agent demonstrates its ability to learn and adapt within the given environment.
