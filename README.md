# Distance-Based-Replay-Sampling-in-Hindsight-Experience-Replay
ECE276C Final Project

## Introduction
This was my final project for the Robot Reinforcement Learning Graduate Course at UCSD with Professor Yip in Winter 2021  

This project utilizes Deep Deterministic Policy Gradient (DDPG) along with Hindsight Experience Replay (HER) to train a robotic arm agent to perform certain long term tasks. A novel Euclidean-based replay sampling is implemented in the HER algorithm in order to reduce training time.  

## Running the Code
Compiling all the Jupyter Notebook cells will create all the python files you need to run the code. You can then either use command line or a Jupyter Notebook cell to run the code.  
Example:
```bash
mpirun -n 8 python -u main.py --env-name 'FetchPush-v1' --filename='vanilla_her_push'
```
This command will use 8 CPU cores to train the robot agent on the 'FetchPush-v1' environment. It will then store the trained parameters into a pickle file named 'vanilla_her_push.pickle'.   
Throughout this project, the agent was trained on three Mujoco simulation environments: 'FetchPush-v1', 'FetchPickAndPlace-v1', and 'FetchSlide-v1'. You can try other environments, but there is no guarantee that they will work.

Rest of README is WIP
