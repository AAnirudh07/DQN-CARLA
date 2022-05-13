# DQN-CARLA
This repository contains the implemetations for the following:
1. Internal state-based car control.
2. Self driving in CARLA's <a href="https://carla.readthedocs.io/en/latest/core_map/">Town02</a> map. 

The reinforcement learning method used for self driving was the Deep Q-Network. The <a href="https://arxiv.org/abs/1610.02357">Xception </a> model was used as the DQN neural network. 

The car has a camera attached to the hood. The frames captured by the camera are fed into the neural network for training in batches. A collision sensor is also attached to the vehicle. It is used in tandem with the episode duration to determine the reward.

The highest observed reward for the was around -130 at episode 100. The lowest observed reward was -340 at episode 1. 
