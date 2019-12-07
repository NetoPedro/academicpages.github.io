---
title: "Playing Pong from Pixels with Deep Q Learning"
topic: "Reinforcement Learning"
excerpt: "Using Q-Learning to teach an agent how to play Pong from the pixels <br/>"
collection: portfolio.rl
---

[Project Website](https://netopedro.github.io/Pong-Pixels-Reinforcement-Learning)

[Project GitHub](https://github.com/NetoPedro/Pong-Pixels-Reinforcement-Learning)


Using Q-Learning to teach an agent how to play Pong from the pixels. Final project to the course [ELEC-E8125 - Reinforcement learning](https://mycourses.aalto.fi/course/view.php?id=24753) at Aalto University, Finland.

## Overview 

Reinforcement learning has been growing for a few years and giving some amazing new techniques that were thought to be impossible or really hard. It has evolved from simple tasks requiring domain knowledge, to other more abstract ones, and finally it ended up beating humans on human games. For this project, the idea is to develop an agent that can learn how to play the game of Pong, not only that, but it shall start without any knowledge, about what is the ball, the paddles and how a point is scored. It shall learn from the frame pixels, similarly to the vision captured by the human eye from the game and decide between 3 possible actions: UP, DOWN and STAY.

![Agent Playing](https://raw.githubusercontent.com/NetoPedro/Pong-Pixels-Reinforcement-Learning/master/images/image_2.png)

## Results 

| Colour  | Experience Replay Size | Target Update Frequency  | Exploration episodes | WinRate Simple AI  | 
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Pink  | 40000 | 1000  | 100000  | \[65;70\[  | 
| Green  | 40000  | 250  | 100000  | \[65;70\[   | 
| Gray  | 10000  | 1000  | 100000  | \[75;85\[  | 
| Orange  | 10000  | 250  | 100000  | \[65;70\[  | 
| **Blue**  | **100000**  | **250**  | **100000**  | **\[85;95\[**  | 
| Red  | 70000  | 250  | 250000  | \[75;80\[  | 
