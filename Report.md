# Report on Udacity Deep RL Nanodegree: project1-Navigation

### Training Code
The code is written in PyTorch and Python3, executed in Jupyter Notebook
- Navigation.ipynb	: Main Instruction file
- dqn_agent.py	: Agent and ReplayBuffer Class
- model.py	: Build QNetwork and train function
- model_dqn.pth : Saved Model Weights

**Neural Network Architecture**<br/>
The state space has 37 dimensions and the size of action space per state is 4.<br/>
so the number of input features of NN is 37 and the output size is 4.<br/>
And the number of hidden layers and each size is configurable in this project.<br/>
You can input the list of hidden layers as one of the input parameters when creating an agent.<br/>
The hidden layers used in this project is [97,32] <br/>

Number of features
* Input layers : 37
* Hidden layer 1: 96
* Hidden layer 2: 32
* Output layer : 4

**Start with <br/>
1. Cloning the repository
2. Download the environment from one of the links given in Udacity Project details page. You need only select the environment that matches your operating system:

(For Windows users) Check out this link if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

(For AWS) If you'd like to train the agent on AWS (and have not enabled a virtual screen), then please use this link to obtain the environment.

Place the file in your DRLND GitHub repository and start with Navigation.ipynb

**Hyper-parameters**<br/>

- BUFFER_SIZE = int(1e5)
- BATCH_SIZE = 64
- GAMMA = 0.99
- TAU = 1e-3
- LR = 5e-5
- UPDATE_EVERY = 4

Note: learning rate is also configurable, you can specify when creating an agent.


###Average Score

Episode 100	Average Score: 0.99
Episode 200	Average Score: 6.05
Episode 300	Average Score: 10.32
Episode 400	Average Score: 12.34
Episode 416	Average Score: 13.00
Environment solved in 316 episodes!	Average Score: 13.00
Total training time 0:05:13 s

### Ideas for Future Work
This implemetation is mainly focused on VDQN.. To have better results and understanding, we can also use double DQN, dueling DQN for improved navigation performance. 

