# Report

The learning algorithm is a DQN a Deep Q Network that uses experience replay with fixed Q targets.

The experience replay shuffles SARS tuples to remove correlation across consecutive states.

The model consists of 2 hidden layers with RELU activation functions 1 input layer and 1 output layer without RELU for regression.

The optimizer used is ADAM for the local QNetwork, every batch update the target QNetwork is updated with new Q parameters. (fixed Q targets)

Hyperparameters:

- BUFFER_SIZE = int(1e5)  , experience replay buffer size
- BATCH_SIZE = 64         , learning batch size
- GAMMA = 0.99            , reward discount 
- TAU = 1e-3              , linear interpolation parameter for updating target's weights.
- LR = 5e-4               # learning rate 
- UPDATE_EVERY = 4        # how often to update the network





