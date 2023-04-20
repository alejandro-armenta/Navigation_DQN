# Report

The learning algorithm is a DQN a Deep Q Network that uses experience replay with fixed Q targets.

The experience replay shuffles SARS tuples to remove correlation across consecutive states.

The model consists of 2 hidden layers with RELU activation functions 1 input layer and 1 output layer without RELU for regression.

The optimizer used is ADAM for the local QNetwork, every batch update the target QNetwork is updated with new Q parameters. (fixed Q targets)

Hyperparameters:

- 





