---
title: "Universal Adversarial Perturbations"
excerpt: "Implementation of Universal Adversarial perturbations with Pytorch. <br/>"
topic: "Paper Reproduction"
collection: portfolio
---

[Project Website](https://netopedro.github.io/Universal-Adversarial-Perturbations-Pytorch)

[Project Github](https://github.com/NetoPedro/Universal-Adversarial-Perturbations-Pytorch)

Implementation of [Universal Adversarial Perturbations paper](https://arxiv.org/abs/1610.08401) for the CS-E4070 - Special Course in Machine Learning and Data Science: Advanced Topics in Deep Learning course at Aalto University, Finland.


## Overview

Adversarial examples are a big issue of machine learning models, especially neural networks. In this paper, the authors try to exploit some characteristics of this problem and the properties of the adversarial examples. 

The paper studied for this project has shown some impressive results: 

- It has shown that the state of the art neural networks can be fooled with a high probability on most of the images with the same computed adversarial example.

- The paper also proposed the pseudo code of the algorithm implemented in this repository to find the perturbations that can fool with high probability most of the images shown to a neural network. 

- It is also shown and possible to see in this implementation that a rather small number of training samples is enough to generate a perturbation capable of fooling the network with high probability on the remaining data.  

- Although this part is not compared with the code in this repository, it is shown that these perturbations are somewhat capable to generalize also to other architectures. This is what the authors call "Doubly universal", with respect to the data and to the architecture of the network. 

- Finally, it is shown that there is a geometric correlation behind these examples that make neural networks highly vulnerable if anyone with malicious intent tries to affect the system. 

## Universal Perturbations

The main goal is to find a perturbation where: 

- ![equation1](https://latex.codecogs.com/gif.latex?%5Cwidehat%7Bk%7D%28x&plus;v%29%20%5Cneq%20%5Cwidehat%7Bk%7D%28x%29) for most ![equation2](https://latex.codecogs.com/gif.latex?x%20%5Csim%20D)

The above formula can be translated to a perturbation v that when added to x, changes the output of K' for most of the data points x drawn from the distribution. 

The generated perturbation 'v' is subject to some constraints: 

- ![equation3](https://latex.codecogs.com/gif.latex?%5C%7C%20v%20%5C%7C_%7Bp%7D%20%5Cleq%20%5Cvarepsilon)

- ![equation4](https://latex.codecogs.com/gif.latex?foolingRate%20%5Cgeq%201-%20%5Cdelta)

The first constraint is responsible to manage and regulate how small is the vector v. The second one ensures that the fooling rate for all images is above the defined threshold. On this implementation, the fooling rate is calculated using all the images on the test set.  

## Results

### Fooling rate 

Evolution of the fooling rate per iteration of the universal adversarial perturbation algorithm , using only 100 images from the train data to generate universal perturbations.  

   ![Fooling rate per iteration](https://raw.githubusercontent.com/NetoPedro/Universal-Adversarial-Perturbations-Pytorch/master/fool_rate.png)
   
### Accuracy 

Evolution of the accuracy of the network on the test set when added the final perturbation of some iteration.
 
 ![Accuracy per iteration](https://raw.githubusercontent.com/NetoPedro/Universal-Adversarial-Perturbations-Pytorch/master/accuracy.png)

