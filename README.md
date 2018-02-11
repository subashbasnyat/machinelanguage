# **BREAKOUT Game using A3C Pytorch**

This repository includes implementation of Asynchronous Advantage Actor-Critic (A3C) in Pytorch.

# **Requirements**
 -  Python 3+
-   OpenAI Gym
-   Pytorch
-   other python packages as scipy,numpy, opencv etc

  
We implemented an A3C model, using LSTM's, and trained it on atari 2600 environment, Breakout-v0 provided in the Openai Gym.
Adam optimizer was used for sharing weights.

# **Training**
Limit number of worker threads to number of cpu cores available as too many threads (e.g. more than one thread per cpu core available) will actually
result in decrease of training speed and effectiveness.
To train agent in Breakout-v0 environment:
  _**python main.py --env-name Breakout-v0 --num-processes 4**_
  
# **Test**
To run a N episode gym evaluation with trained model : 
  _**python test.py --env-name Breakout-v0 --num-episodes N**_
  
# **Results**
![image](https://user-images.githubusercontent.com/19267332/36074665-8455f7ec-0f6b-11e8-89bc-c7b9fc02b336.png)

![image](https://user-images.githubusercontent.com/19267332/36074674-996b4448-0f6b-11e8-8def-6c3a3216a025.png)

# **Team Members**  
1. Subash Basnet (https://github.com/subashbasnyat)
2. Uttam Sapkota (https://github.com/uttsap)

# **Report**
[final report.pdf](https://github.com/docker/machine/files/1714499/ML.report.pdf)

# **References**

1. https://arxiv.org/pdf/1602.01783.pdf
2. https://medium.com/emergent-future/simple-reinforcement-learning-with-tensorflow-part-8-asynchronous-actor-critic-agents-a3c-c88f72a5e9f2
3. https://github.com/liampetti/A3C-LSTM
