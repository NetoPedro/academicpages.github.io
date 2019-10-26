---
title: "Playing Flappy Bird with Deep Reinforcement Learing (Incomplete)"
topic: "Reinforcement Learning"
excerpt: "An implementation with Pytorch of an agent to learn how to play the Flappy Bird game. <br/>"
collection: portfolio.rl
---

[Project Website](https://netopedro.github.io/DeepReinforcementLearningFlappyBird)

[Project GitHub](https://github.com/NetoPedro/DeepReinforcementLearningFlappyBird)

## Overview
This project is heavly inspired by the one developed by [1].
Although, there are some significative changes: 

1. Pytorch was used instead of Tensorflow 
2. The preprocessing was modified in order to decrease even further the convergence time and test how small can the input be and still be enough to the network. 
3. The network architecture is slightly different, only 3 inputs channels are used, and smaller kernel filters are used for each convolution. 
4. It is intended to have further experiences relating convergence times and graphical elements. 



## Environment

The environment used was developed originally in [1].
It uses a regular flappy bird game without background and with the following rewards: 

1. Crash = -1
2. Did not crash = 0.1
3. +1 for each pipe 
