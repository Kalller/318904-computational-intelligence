# LAB 2

In the Task 1 I fixed the optimal agent in order to choose the correct move in the misere state of the game.   

In the Task 2 of the code was implemented an evolutionary strategy (ES) based agent to play the game of Nim using a rule-based approach. The Nim game involves removing objects from heaps, with the goal of being the player to remove the last object.

## Rule Representation

The fundamental concept is a `Rule` which comprises three components: condition, position, and action. These components are utilized to guide the agent's decision-making process.

### Components:

- **Conditions**: Functions that evaluate the game state and return boolean values. Examples include `odd_rows`, `even_rows`, and `misere_state`.
  
- **Positions**: Functions that determine the heap or row to act upon. For instance, `min_position`, `max_position`, and `random_position`.
  
- **Actions**: Functions dictating the move to be made. Examples are `get_one`, `leave_one`, `get_all`, and `get_random`.

## ES Agent

The `ESAgent` class represents an agent that employs an evolutionary strategy to learn and adapt its ruleset over generations to improve gameplay performance.

### Agent Functionality:

- **Initialization**: Generates all possible rules and initializes weights and sigmas randomly.
  
- **Rule Selection**: Picks a rule based on the condition being true for the current game state using stochastic universal sampling.
  
- **Gameplay**: Executes the chosen rule's action on the game state.
  
- **Evaluation**: Plays games against different opponents (optimal and random agents) to evaluate its performance and update fitness.
  
- **Mutation**: Introduces mutation by adjusting weights based on Gaussian noise.
  
- **Adaptation**: Adjusts sigmas for mutation based on the agent's win rate.

## Evolutionary Strategy

The code implements an evolutionary process to evolve a population of agents over multiple generations.

- **Population Initialization**: Creates a population of agents (ESAgents).
  
- **Fitness Evaluation**: Evaluates the fitness of each agent in the population by playing games.
  
- **Selection**: Selects parents based on top-performing individuals.
  
- **Reproduction**: Generates children through crossover and mutation from selected parents.
  
- **Adaptation and Evolution**: Applies adaptation to the population and progresses to the next generation.

## References and Collaborations

During the troubleshooting of Task 1, I collaborated closely with [`Loris Fabrizio Mario Vitale`](https://github.com/lfmvit/s317264-computational-intelligence-labs) to successfully address and rectify the misère bug present in the optimal method.

The foundational structure of Task 2 was influenced by the project led by [`Beatrice Occhiena`](https://github.com/beatrice-occhiena/Computational_intelligence/blob/main/Labs/Lab_02/Nim.ipynb). Her approach to the rule methodology was particularly insightful and served as an inspiring skeleton for my project.

Additionally, I leveraged [`chatGPT`](https://chat.openai.com/) to gain assistance and insights during the development process.


