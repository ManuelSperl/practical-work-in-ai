
# Implicit Q-Learning (IQL) - Practical Work in AI 2023

## Overview
This repository contains the implementation and results of the Implicit Q-Learning (IQL) model as part of the "Practical Work in AI" project. This project aims to explore advanced reinforcement learning techniques by implementing IQL to train agents capable of making decisions from offline datasets.

## Contents
- `pw_implicit_q_learning_datasets.ipynb`: Notebook for creating various datasets used for training the IQL model.
- `pw_implicit_q_learning.ipynb`: Notebook for training and evaluating the IQL model using the preprocessed datasets.

## Datasets
This project utilizes five different datasets to train the IQL model, each tailored to explore different aspects of learning:
1. **Random Dataset**: Generated by a policy that selects actions uniformly at random.
2. **Expert Dataset**: Generated from a pre-trained expert policy.
3. **Mixed Dataset**: Combines data from both random and expert policies.
4. **Noisy Dataset**: Expert data with injected noise to simulate real-world unpredictability.
5. **Replay Dataset**: A mix of the above datasets with added temporal correlations.

## How to Use
To use this repository:
1. Clone the repository to your local machine or open it in a Jupyter environment that supports IPython notebooks.
3. Run the `pw_implicit_q_learning_datasets.ipynb` notebook to generate and preprocess the datasets.
4. Execute the `pw_implicit_q_learning.ipynb` to train the IQL model and evaluate its performance on different datasets.

## Model
The implementation includes:
- `ActorNet`: Defines the policy model using a squashed Gaussian distribution.
- `CriticNet`: Evaluates the quality of actions taken by the actor.
- `ValueNet`: Estimates the value of states.
- `IQLAgent`: Coordinates the training of the Actor, Critic, and Value networks.

## Dependencies
Ate the Beginning of each Notebook is a Installation Section to install everything needed within this Notebook.
- Python 3.8+
- PyTorch
- NumPy
- Matplotlib
- Gym
- TensorBoard

## Authors
- **Manuel Sperl**
