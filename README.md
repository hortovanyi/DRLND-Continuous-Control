# DRLND Continuous Control Project
---
This is the second project in the Udacity Deep Reinforcement Learning Nanodegree. 

This project works with the [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment.

[![Trained Agent](https://github.com/hortovanyi/DRLND-Continuous-Control/blob/master/output/reacherp_ddpg_agent_small.gif?raw=true)](https://www.youtube.com/watch?v=N1vWkCfbEGQ)

## Project Details
In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

## Getting Started
It is recommended to follow the Udacity DRL ND dependencies [instructions here](https://github.com/udacity/deep-reinforcement-learning#dependencies) 

This project utilises [Unity ML-Agents](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md), [NumPy](http://www.numpy.org/) and [PyTorch](https://pytorch.org/) 

A prebuilt simulator is required in be installed. You need only select the environment that matches your operating system:

### Version 1: One (1) Agent
Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)

### Version 2: Twenty (20) Agents
Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

The file needs to placed in the root directory of the repository and unzipped.

Next, before starting the environment utilising the corresponding prebuilt app from Udacity  **Before running the code cell in the notebook**, change the `file_name` parameter to match the location of the Unity environment that you downloaded.

## Instructions
Then run the [`DDPG_Continuous_Control.ipynb`](https://github.com/hortovanyi/DRLND-Continuous-Control/blob/master/DDPG_Continuous_Control.ipynb) notebook using the drlnd kernel to train the DDPG agent.

Once trained the model weights will be saved in the same directory in the files `checkpoint_actor.pth` and `checkpint_critic.pth`.

The model weights are used by the [`Trained Agent.ipynb` ](https://github.com/hortovanyi/DRLND-Continuous-Control/blob/master/Trained%20Agent.ipynb) notebook against the simulator. 

[Simulator Output Video](https://www.youtube.com/watch?v=N1vWkCfbEGQ)