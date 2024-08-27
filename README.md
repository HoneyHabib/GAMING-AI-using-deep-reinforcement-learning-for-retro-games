# Gaming AI with Deep Reinforcement Learning for Retro Games

Welcome to the **Gaming AI with Deep Reinforcement Learning** repository! This project demonstrates the use of deep reinforcement learning (DRL) to develop an AI agent capable of playing retro games, specifically Street Fighter. The goal is to create an intelligent agent that can learn to play and excel at the game through self-play and reinforcement learning techniques.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Usage](#usage)
  - [Environment Setup](#environment-setup)
  - [Training the Agent](#training-the-agent)
  - [Evaluation and Results](#evaluation-and-results)
- [Contributing](#contributing)
- [Contact](#contact)

## Project Overview

This repository contains an implementation of a deep reinforcement learning agent designed to play the classic retro game Street Fighter. Using techniques such as Deep Q-Learning (DQN), Proximal Policy Optimization (PPO), or other DRL algorithms, the project aims to develop an AI that learns optimal strategies and actions through interaction with the game environment.

## Features

- **Deep Reinforcement Learning**: Utilizes state-of-the-art DRL algorithms to train the AI agent.
- **Game Integration**: Specifically tailored for playing and mastering Street Fighter.
- **Self-Play and Training**: The AI improves its performance by playing against itself and learning from experience.
- **Performance Metrics**: Includes tools for tracking and evaluating the AI's progress and gameplay effectiveness.

## Technologies Used

- **Python**: Core programming language for implementing the AI.
- **TensorFlow**: Libraries for building and training deep learning models.
- **OpenAI Gym**: Framework for creating and interacting with the game environment.
- **Retro**: A library for interfacing with classic retro games like Street Fighter.

## Getting Started

To get started with this project, follow these steps:

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/gaming-ai-deep-reinforcement-learning.git
   ```

2. **Navigate to the Project Directory**

   ```bash
   cd gaming-ai-deep-reinforcement-learning
   ```

3. **Install Dependencies**

   You will need to install the following Python packages:

   - Pygame
   - Gym
   - Pytorch
   - Optuna

   Install these packages using `pip`:

   ```bash
   pip install gym==0.21.0
   ```

4. **Download the Street Fighter ROM**

   You will need the Street Fighter ROM file for the Retro library. Ensure you have the appropriate ROM file and place it in the `Roms` directory. Follow [Retro's instructions](https://github.com/openai/retro) for obtaining and configuring ROMs.

## Usage

### Environment Setup

Configure the game environment and ensure it is correctly integrated:

```python
import retro

##startup the game environment
env = retro.make(game = 'StreetFighterIISpecialChampionEdition-Genesis')

# Reset the environment
obs = env.reset()
```

### HyperParameter Tuning

### setup callbacks

### Training the agent


### Evaluation and Results

Evaluate the trained agent’s performance:

```python
model = PPO.load('./train/best_model_5100000.zip')
mean_reward, _ = evaluate_policy(model, env, render=True, n_eval_episodes=2)
obs = env.reset()
obs.shape
env.step(model.predict(obs)[0])
```
## Contributing

Contributions are welcome! If you have suggestions, improvements, or fixes, please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a pull request


## Contact

For any questions or feedback, please reach out to honeyhabib.habib@gmail.com or open an issue in the repository.

Happy gaming and coding! 🚀

---

Feel free to adjust or add more details based on your specific implementation and setup!
