# Project2_Continuous_Control

Project Objective

The goal of this project is to create and train a double-jointed arm agent that is able to maintain its hand in contact with a moving target for as many time steps as possible.


Environment:
This environment provided using  the Unity ML-Agents. A double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the target location.

State/Action Spaces:
The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm.
the actiona space consists of 4 actions

Instructions to download:
Please download the github repository and use place all the files in a folder and open .ipynb file
https://github.com/sriten15/Project2_Continuous_Control

ipynb will install the python environment



Train and Test the agent:

Firstly, we shd import the following modules, 


Create the agent and call the training function:



Checkpoints to test:
Once the agent is trained, the checkpoint.pth will hold the training parameters which can be loaded to test the agent 

Goal:

To solve the environment, one agent version , the agent is expected to achieve average score of 30+ for 100 consecutive episodes.



Github Repository Files:
Readme.md
Continuous_Control.ipynb
ddpg_agent.py
model.py
checkpoint.pth
Report.md

Since the project is executed in jupyter notebook. Please run the jupyter notebook as is to look at the agent trained in the environment.

