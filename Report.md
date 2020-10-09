Introduction
I have worked on the DDPG agent algorithm by tweaking the hyper parameters to achieve the objective of achieving average score of 30+ for over 100 episodes.

Learning Algorithm (Deep Deterministic Policy Gradients (DDPG) )
I used Deep Deterministic Policy Gradients (DDPG) pendulum for this problem. a kind of actor-critic method.   

Network Architecture

The network architecture for actor and critic has two fully connected hidden layers of 400 and 300 units. Adam was used as an optimizer for both actor and critic networks in the DDPG pendulum code.


Hyperparameters
The important aspect of this project is to tweak the hyper parameters to achieve project objectives 

Initially , I tried varying the network architecture but it didnt yield expected results. Then i switched backed to existing architecture in ddpg pendulum code and changed the actor and critic learning rate to 2x10-4 each and then further tuned the frequency to update the replay buffer, the final parameters that helped to achieve 30+ moving average after first 100 episodes are below:

BUFFER_SIZE = int(1e5)  # replay buffer size
BATCH_SIZE = 128        # minibatch size
GAMMA = 0.99            # discount factor
TAU = 1e-3              # for soft update of target parameters
LR_ACTOR = 2e-4         # learning rate of the actor 
LR_CRITIC = 2e-4       # learning rate of the critic
WEIGHT_DECAY = 0.00        # L2 weight decay
LEARN_FREQ_in_STEP = 5        # learning timestep interval
LEARN_COUNT   = 1        # number of learning passes

Conclustion

The problem was solved in 100 episodes for score of over 30+. The plot for rewards is shared below:



Future Work:
The above version shared is a single-agent one.  Further i would like to expand my learnings into multi agent environment using DDPG. And try problem with recommended such as TRPO,TNPG and own version of PPO for multi agent problem, 
