---
title: "Predicting Pneumonia with Deep Learning"
excerpt: "Using Deep Learning to Segment pneumonia opacities on X-Ray images. <br/>"
topic: "Deep Learning"
collection: portfolio.dl
---

[Project Website](https://netopedro.github.io/DeepLearningProject/)

[Project Github](https://github.com/NetoPedro/DeepLearningProject)

Final project for the CS-E4890 - Deep Learning course at Aalto University, Finland. 

## Overview

My goal for this project was to not only classify X-ray images as pneumonia or not pneumonia but also to detect opacities that are the cause of a positive classification. To achieve this goal with good enough results a few techniques were considered, and the pros and cons compared.  

The first idea was to try an object detection algorithm like [RetinaNet](https://arxiv.org/abs/1708.02002), [R-CNN](https://arxiv.org/abs/1311.2524) or even the improved version [Faster R-CNN](https://arxiv.org/abs/1506.01497). Nevertheless, I wanted to train the model just by using a CPU, ao I started to consider some simpler model for image segmentation. Hence, I came across the [U-Net](https://arxiv.org/abs/1505.04597), a this became the chosen approach.  It was not as fast as I would like on the CPU, but much faster than the other options, especially with some tweaks. 
