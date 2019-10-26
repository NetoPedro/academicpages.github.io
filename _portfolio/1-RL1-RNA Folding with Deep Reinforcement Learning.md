---
title: "RNA Folding with Deep Reinforcement Learning"
excerpt: "This project aims to tackle a simplified version of the RNA folding (secondary structure) problem using deep reinforcement learning.<br/>"
collection: portfolio.rl
topic: "Reinforcement Learning"
---

[Project Website](https://netopedro.github.io/RNAFoldingDeepRL/)

[Project Github](https://github.com/NetoPedro/RNAFoldingDeepRL)

Implementation of a RL agent to fold RNA sequences for the CS-E4880 - Machine Learning in Bioinformatics course at Aalto University, Finland.

  ![Sakurambo [CC BY-SA 3.0 (http://creativecommons.org/licenses/by-sa/3.0/)]](https://upload.wikimedia.org/wikipedia/commons/3/3f/Stem-loop.svg)

Sakurambo [CC BY-SA 3.0 (http://creativecommons.org/licenses/by-sa/3.0/)]

## Overview

This project aims to tackle a simplified version of the RNA folding (secondary structure) problem using reinforcement learning. To achieve the mentionated goal it will be necessary to build the entire environment from scratch, including rewards, states and other necessary utilities.  

* RNA
* Environment 
* Policy

All those components are further explained below. 

## Components

### RNA 

The RNA component has the main intention to model the behaviour of a RNA sequence and respective structure. This model is created in a simplified way.
 
#### Sequence

  The sequence is a string of the characters "A", "C", "U", "G" that represent the bases present on the RNA. 
  
  ![Sequence Example](https://raw.githubusercontent.com/NetoPedro/RNAFoldingDeepRL/master/RNASequence.png)

#### Structure Representation 
  
  The structure representation is not unique, in a way that the secondary structure of a RNA sequence can be represented by a myriad of ways. Some representations are better to detect pseudoknots, others are better to feed to a policy. 
  
  ![Structure Example](https://raw.githubusercontent.com/NetoPedro/RNAFoldingDeepRL/master/RNAStructure.png)
   
   Above it is possible to see a common representation of the secondary structure of a RNA sequence. Below it is possible to see a ar diagram representation of other sequence.
   
   ![Structure Example](https://raw.githubusercontent.com/NetoPedro/RNAFoldingDeepRL/master/arc_diagram.png)
  
