# Tic-Tac-Toe Reinforcement Learning

This Jupyter Notebook contains Python code that implements a Tic-Tac-Toe game using Monte Carlo reinforcement learning techniques.

## Overview 

The code in this notebook implements a Tic-Tac-Toe player using reinforcement learning, specifically Monte Carlo methods. It consists of the following components:

- `State`: Defines the state of the game.
- `print_board`: Function to print the game board with emojis.
- `win`: Checks if a player has won the game.
- `state_value`: Calculates the value of a state for a player.
- `random_game`: Simulates a random game of Tic-Tac-Toe, used in the learning phase.
- `play_multiple_games`: Plays multiple games between two agents and displays win percentages.
- `play_game`: Allows two agents to play a single game and displays the result.
- `value_dictionaries`: Dictionaries to store state values for each player.
- `epsilon` and `eps`: Parameters for reinforcement learning.
- `rl_agent`: Represents an agent that uses Monte Carlo 
reinforcement learning to make moves.
- `random_agent`: Represents an agent that makes random moves.
## Usage

To use this notebook:

- Run the code cells sequentially.
- Adjust parameters like `epsilon` and `eps` for experimentation.
- Explore the outcomes of games between random and Monte Carlo reinforcement learning agents.

## Credits

- `Marcello Vitaggio`: I refined professor Squillero's code in order to make it able to learn as the second player.  
GitHub: [Link](https://github.com/Kalller/computational-intelligence), Email: s318904@studenti.polito.it
- `Giovanni Squillero`: Author of the original code.  
GitHub: [Link](https://github.com/squillero/computational-intelligence), Email: giovanni.squillero@polito.it

## Licensing

This code is free for personal or classroom use. Please refer to [`LICENSE.md`](https://github.com/Kalller/computational-intelligence/blob/main/LICENSE.md) for details.
