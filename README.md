# Reinforcement Learning for Continuous Action Spaces

## Overview
This project implements three different reinforcement learning algorithms: REINFORCE, Policy Gradient with Baseline (PGB), and Proximal Policy Optimization (PPO). These algorithms are designed to handle continuous action spaces and are demonstrated using the "Ant-v4" environment from OpenAI's Gym.

### Algorithms:
1. **REINFORCE**: A simple policy gradient method for reinforcement learning.
2. **Policy Gradient with Baseline (PGB)**: An extension of the basic policy gradient to reduce variance.
3. **Proximal Policy Optimization (PPO)**: An advanced policy gradient method that balances the trade-off between exploration and exploitation.

## Installation

Ensure you have Python 3.8+ installed on your system. You can install the required libraries using the following commands:

```bash
pip install gymnasium
pip install torch
pip install matplotlib
```

For rendering environments, you may need additional setup for mujoco. Please follow the installation guide specific to your system from [ Mujoco's official documentation](https://mujoco.org/)

## Usage

To run the simulations with the desired algorithm, you can use the following command structure:

```bash
python hw2.py --algo [algorithm]
```

Where [algorithm] can be:

1. ```pg``` for REINFORCE
2. ```pgb``` for Policy Gradient with Baseline
3. ```ppo``` for Proximal Policy Optimization

## Examples

1. ```python hw2.py --algo pg```
2. ```python hw2.py --algo pgb```
3. ```python hw2.py --algo ppo```

## Code Structure

1. ```PolicyNetwork```: Defines the neural network for policy approximation.
2. ```ValueNetwork```: Defines the neural network for value estimation.
3. ```sample_action```: Samples an action from the policy network output.
4. ```reinforce, pgb, ppo```: Implementation of the respective algorithms.

## Results

Results from the simulations are plotted in terms of total rewards per episode. Each run will display a graphical output showing the learning curve of the agent in the environment.

