![LSE](lse-logo.jpg) 
# ST449 Artificial Intelligence and Deep Learning 

### Lent Term 2020

### Instructors

* [Milan Vojnovic](http://personal.lse.ac.uk/vojnovic/), [email](mailto:m.vojnovic@lse.ac.uk), Department of Statistics.  *Office hours*: By appointment, COL 5.05

### Teaching Assistant
* Tianlin Xu, [email](mailto:t.xu12@lse.ac.uk), Department of Statistics.  *Office hours*: Thursday 11:00 - 12:00, COL 5.03 (from week 2)

### Course Information

* Lectures on Wednesdays 11:00–13:00 in NAB.1.04
* Classes on Fridays 14:30–16:00 in 32L.LG.18

No lectures or classes will take place during School Reading Week 6.

| **Week** | **Topic**                            |
|----------|--------------------------------------|
| 1        | [Course overview](#week-1-course-overview) |
| 2        | [Introduction to neural networks](#week-2-introduction-to-neural-networks)                  |
| 3        | [Training neural networks](#week-3-training-neural-networks)    |
| 4        | [Convolutional neural networks](#week-4-convolutional-neural-networks)       |
| 5        | [Sequence modeling](#week-5-sequence-modeling)                  |
| 6        | _Reading Week_                       |
| 7        | [Introduction to reinforcement learning](#week-7-introduction-to-reinforcement-learning) |
| 8        | [Dynamic programming and Monte Carlo methods](#week-8-dynamic-programming-and-monte-carlo-methods) | 
| 9        | [Temporal difference methods and eligibility traces](#week-9-temporal-difference-methods-and-eligibility-traces)|
| 10       | [Generalization and function approximation](#week-10-generalization-and-function-approximation) |
| 11       | [Policy gradient methods](#week-11-policy-gradient-methods)           |



### Course Description

This course covers main principles of neural networks, supervised learning, and reinforcement learning. 
The topic of neural networks covers basic principles of neural network architectures, optimization methods for training neural networks, and special neural network architectures that are in common use for image classification, speech recognition, machine translation and other tasks. The topic of reinforcement learning covers basic concepts of a reinforcement learning problem formulation, such as agent, environment, tasks, and rewards, as well as mathematical formulation as a Markov Decision Process and Bellman optimality equations. The course then proceeds with discussing elementary solution methods including dynamic programming, Monte Carlo methods, temporal difference learning, and eligibility traces. The course ends with closing the loop by covering reinforcement learning methods based on function approximation including both value-based and policy-based methods. 

The lectures cover fundamental theoretical principles while seminar sessions provide students with an 
opportunity to gain hands-on experience with using state-of-the-art software frameworks for learning and evaluating neural networks and reinforcement learning algorithms. The exercises are based on using TensorFlow, an open source machine learning framework for dataflow graph computations, and OpenAI Gym, a software framework for developing and evaluating reinforcement algorithms. 

The course has a signficiant project component. Students work on individual course projects with the goal to 
study specific methodological topics within the scope of the course. For example, this may involve studying particular neural network architectures, optimization methods for learning neural networks, or reinforcement learning problem formulations. 

### Organization

This course provides introduction to fundamental concepts of neural networks, training of neural networks, and reinforecement learning algorithms. The course does not assume a prior knowledge of these concepts.  

The course involves 20 hours of lectures and 15 hours of computer workshops in the LT. 	


### Prerequisites

Basic prior knowledge of statistics, probability and machine learning, as well as some programming experience in Python are expected. 

### Software

We will use a wide range of tools, including Juypter notebooks, Google Colab, TensorFlow, OpenAI Gym, as well as cloud computing platforms such as Google Cloud Platform.

Where appropriate, we use Jupyter notebooks for lab assignments, demonstrations, and course notes themselves.

### Assessment

Project assignment (80%) and continuous assessment in weeks 4 and 7 (10% each). Students are expected to produce 10 problem sets in the LT. 


### Schedule

---
#### Week 1. Course overview

In the first week lecture, we describe organization and overview the content of the course. We will go through a wide range of machine learning tasks for which deep learning has proven to provide high accuracy rates. This will include image recognition, speech recognition, machine translation, and reinfocement learning tasks. The reinforcement learning tasks include various game playing and resource allocation problems. We will quickly review main software frameworks for learning and evaluating neural networks and reinforcement learning algorithms.  

*Readings*:
* LeCun, Bengio and Hinton, [Deep Learning](https://www.nature.com/articles/nature14539), Nature Review, Vol 521, 2015
* Mitchell et al, [Never-Ending Learning](https://cacm.acm.org/magazines/2018/5/227193-never-ending-learning/fulltext), CACM 2018

*Lab*: **Getting started** 
* Getting started with TensorFlow

---
#### Week 2. Introduction to neural networks

We start with discussing single-layer networks, linear discriminant functions, perceptron, and their limitations. 
We explain their learning limitations for the well-known XOR problem. We then describe multi-layer perceptron, perceptron learning criteria, and perceptron learning algorithm. We show that a multi-layer perceptron can learn a XOR function. We introduce the framework of multi-layer feedforward neural networks, and pertinent concepts such as neural units, activation functions, and different types of activation functions. We show how two-layer feedforward neural networks can approximate Boolean functions, and discuss how the size of networks (number of parameters) depend on the depth of these networks. 

*Readings*:
* GoodFellow, Bengio and Courville, Deep Learning, Chapter 6: Deep Forward Networks
* Bishop, Neural Networks for Pattern Recognition, Chapters 3 and 4
* Shalev-Shwartz and Ben-David, Understanding Machine Learning, Chapter 20

*Lab*: **Learning neural networks in TensorFlow**
* XOR problem in TensorFlow
* Single-layer perceptron learning algorithm implementation and analysis of its convergence properties

---
#### Week 3. Training neural networks

We describe basic concepts of empirical risk minimization and commonly used optimization algorithms such as batch gradient descent, mini-batch stochastic gradient descent, convergence rates of these algorithms under smoothness and convexity conditions, backpropagation algorithm for efficient computation of gradient vectors, iterative optimization algorithms with momentum, including Nesterov's accelerated gradient, AdaGrad, RMSProp, and Adam. We then discuss commonly used regularization 
methods such as Dropout and data augmentation, as well as methods for mitigating exploding and vanishing gradients such as batch normalization. This lecture concludes with discussion of commonly used evaluation metrics such as top-1 and top-5 accuracy.
 
*Readings*:
* GoodFellow, Bengio and Courville, Deep Learning, Chapter 8: Optimization for Training Deep Models
* Bubeck, [Convex Optimization: Algorithms and Complexity](http://sbubeck.com/book.html)

*Further Resources*:
* L. Bottou and O. Bousquet, [The trade-off of large-scale learning](https://leon.bottou.org/publications/pdf/nips-2007.pdf), NIPS 2017 

*Lab*: **Optimization methods for learning neural networks**
* Optimization in TensorFlow
* Computing gradient vectors
* Momentum algorithms
* Stochastic optimization
* Adam optimizer


