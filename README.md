## Battleship Project

### Abstract

The goal of this project is to train a model to optimize Battleship play by developing a strategy that maximizes the efficiency of targeting and sinking enemy ships. Collection of data will be conducted through randomizing the spawns of each ship and have the model learn after a certain rounds of games. With the data, we will train a machine learning model to predict optimal moves and evaluate different strategies. The model performance will be assessed through measuring the number of moves it took to win and overall win rate. Furthermore, we will explore how different rewards can affect the performance.

### Background

Battleship is a popular naval strategy game that is somewhat simple but has served as a testing ground for algorithms involving AI development and Reinforcement Learning. Battleship is a great well established environment for reinforcement learning because it encompasses a mix of strategic decisions, sequential actions, and hidden information between players [1].

The paper Reinforcement Learning for the Game of Battleship explores reinforcement learning algorithms in battleship. This paper analyzes certain challenges with the game's partially observable environment where the model has to to deduct the locations of the opponent's ships through several test-runs. This paper also explores heuristic search algorithms and analyzes the performances between the decision making processes [2].

Another article titled, An Artificial Intelligence Learns to Play Battleship on Medium, discusses the method of reinforcement learning for a game of battleship. This project has two main approaches, code from scratch using a linear model and using openAi gym library with neural networks. This author implemented q-learning to improve the agent's decision making over 100,000 training episodes[3].

Developing an AI approach to play battleship can involve several different types of algorithms to locate ships and stragetize. Common approaches are Monte Carlo Tree Search, Reinforcement Learning, and probability density function. By leveraging these algorithms, the search method can be refined over time and improve decision making [4].

The article, Coding an Intelligent Battleship Agent, discusses creating an agent to solve the Battleship game, from simple random guessing to advanced approaches such as a Hunt/Target strategy and probabilistic strategies. The agent has learned to compile shots based on probabilities improving overall efficiency [5].

### Problem Statement

The problem we are trying to solve is: “How can we develop an optimal strategy for winning the Battleship game using machine learning?” The winner of Battleship is the first person who sinks all of the enemy ships with the least number of actions taken. As such, we are exploring how to optimize the number of actions taken to win the game. The agent’s action space includes only attacking specific grid cells on the board. A reward function will assign positive rewards for successfully hitting and sinking enemy ships, and negative rewards for misses. The probability of hit can be estimated using various machine learning methods such as Monte Carlo and reinforcement learning. The performance can be measured by win and lose rates, as well as the total number of moves the model made. We will repeat simulating the game multiple times to create dataset, making this problem replicable.
