# TrAIs - Tic-Tac-Toe AI

Welcome to TrAIs, a Tic-Tac-Toe AI project! 
This repository contains code for a Tic-Tac-Toe (called Tris in Italy) game environment and an AI model trained using the Q-Table RL algorithm.

## Getting Started

All the code of the repo can be easily accessed and executed in a Colab notebook by following this link: [Play Tic-Tac-Toe](https://colab.research.google.com/github/IGieckI/TrAIs/blob/main/TrAIs.ipynb)

## Tris Environment

The `Tris` environment represents the Tic-Tac-Toe game. It includes the game board, actions, and methods to check for a winner.

### Usage

Here's an example of how to use the `Tris` environment:

```python
# Create a new Tris game
game = Tris()

# Print the initial game board
print(game)

# Make a move
board.step(action, sign)

# Check for a winner
winner = game.check_winner()
print('The winner is ', winner)

```

## TrAIs - Tic-Tac-Toe AI Model

The `TrAIs` class is an AI model that can play and learn Tic-Tac-Toe. It uses Q-learning to improve its gameplay over time.

### Usage

Here's a how to create and train the AI model:

```python
# Create TrAIs instances for two players
player1 = TrAIs(learning_rate, learning_rate_decay_rate, min_learning_rate, gamma, 'X')
player2 = TrAIs(learning_rate, learning_rate_decay_rate, min_learning_rate, gamma, 'O')

# Get the AI's action for a given game state
action = player1.get_action(board)

# Train the players by simulating games
player1.train(reward)
player2.train(reward)

# Repeat this process until the model is "smart enough"
```

## Training Parameters

You can adjust the training parameters to customize the AI's learning process. Here are the parameters you can modify:

- `NUM_EPISODES`: Number of training episodes
- `LEARNING_RATE`: Initial learning rate
- `LEARNING_RATE_DECAY_RATE`: Rate of learning rate decay
- `MIN_LEARNING_RATE`: Minimum learning rate
- `GAMMA`: Discount factor for future rewards
- `EPSILON`: Exploration rate (initial)
- `MIN_EPSILON`: Minimum exploration rate
- `EPSILON_DECAY_RATE`: Rate of exploration rate decay

## Play Against the AI

You can play against the trained AI model in the Colab notebook. The notebook provides a console interface on the last Colab block.

To play against the AI, execute all cells of the notebook, wait for the training to finish, and then follow the instructions showed on the console.