# Cleaning Robot using Q-Learning

## Objective

Build a simple intelligent cleaning robot that learns how to clean dirty cells in a grid environment using Reinforcement Learning.

## Environment

The robot operates in a:

- 5 × 5 grid
- Environment containing predefined dirty cells
- State represented by the robot's current position
- Action space containing movement and cleaning actions

## Actions

The robot can perform five actions:

- Up
- Down
- Left
- Right
- Clean

## Reinforcement Learning Algorithm

The project uses Q-Learning.

Q-Learning allows the robot to learn which action is best in each state by repeatedly interacting with the environment and updating its Q-values.

The update rule is:

Q(s, a) = Q(s, a) + α [r + γ max Q(s', a') − Q(s, a)]

where:

- `α` = learning rate
- `γ` = discount factor
- `r` = reward
- `s` = current state
- `s'` = next state

## Parameters

- Learning rate: 0.1
- Discount factor: 0.9
- Epsilon: 0.2
- Training episodes: 1000

## Reward System

The reward design encourages useful cleaning behavior.

- Cleaning a dirty cell: positive reward
- Completing the cleaning task: additional positive reward
- Movement: small negative reward
- Cleaning an already clean cell: negative reward

This encourages the robot to clean efficiently while avoiding unnecessary actions.

## Learning Process

During training:

1. The robot begins in the environment.
2. It selects actions using an epsilon-greedy strategy.
3. It receives rewards based on its actions.
4. Q-values are updated after every action.
5. The process is repeated over many episodes.
6. The robot gradually learns better behavior.

## Visualization

The notebook contains a reward graph showing how the total reward changes over training episodes.

The graph helps demonstrate whether the robot improves its behavior through reinforcement learning.

## Tools Used

- Python
- Google Colab
- NumPy
- Matplotlib
- Q-Learning
- Reinforcement Learning

## Conclusion

The project demonstrates how reinforcement learning can be used to train an autonomous cleaning agent.

By learning from rewards and penalties, the robot gradually identifies better actions for navigating the grid and cleaning dirty cells.
