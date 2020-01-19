# ST451 Bayesian Machine Learning 

### Lent Term 2020

### Instructors

* [Kostas Kalogeropoulos](https://kostaskalog.github.io/webpage/), [email](mailto:k.kalogeropoulos@lse.ac.uk), Department of Statistics.  *Office hours*: Mondays 10:30-12:30, COL 6.10

### Teaching Assistants
* Gianluca Giudice [email](mailto:g.giudice@lse.ac.uk), Department of Statistics
* Phil Chan, [email](mailto:p.chan@lse.ac.uk), Department of Statistics.  


### Course Information

- **Lectures** on Mondays 13:00–15:00 in NAB.2.04 (except week 6 which is NAB.LG.01).
- **Computer Classes** there are 3 groups: 
  1. Mondays 15:00–16:30 in STC.S018 taught by Kostas Kalogeropoulos
  2. Tuesdays 16:00-17:30 in FAW.4.03 taught by Gianluca Giudice
  3. Thursdays 15:00-16:30 in STC.S08 taught by Phil Chan
 
 There will be **no reading week**, hence teaching will be concluded on week 10. 

| **Week** | **Topic**                            |
|----------|--------------------------------------|
| 1        | [Bayesian Inference Concepts](#week-1-bayesian-inference-concepts) |
| 2        | [Bayesian Linear Regression](#week-2-introduction-to-neural-networks)                  |
| 3        | [Bayesian Model Selection](#week-3-training-neural-networks)    |
| 4        | [Classification](#week-4-convolutional-neural-networks)       |
| 5        | [Variational Bayes](#week-5-sequence-modeling)                  |                       |
| 6        | [Graphical Models](#week-7-introduction-to-reinforcement-learning) |
| 7        | [Mixture models and Clustering](#week-8-dynamic-programming-and-monte-carlo-methods) | 
| 8        | [Sampling Methods](#week-9-temporal-difference-methods-and-eligibility-traces)|
| 9        | [Sequential Data](#week-10-generalization-and-function-approximation) |
| 10       | [Gaussian Processes](#week-11-policy-gradient-methods)           |

### Course Description

The course sets up the foundations and covers the basic algorithms covered in probabilistic machine learning. Several techniques that are probabilistic in nature are introduced and standard topics are revisited from a Bayesian viewpoint. The module provides training in state-of-the-art methods that have been applied successfully for several tasks such as natural language processing, image recognition and fraud detection.

The first part of the module covers the basic concepts of Bayesian Inference such as prior and posterior distribution, Bayesian estimation,  model choice and forecasting. These concepts are also illustrated in real world applications modelled via linear models of regression and classification and compared with alternative approaches.

The second part of the module introduces and provides training in further topics of probabilistic machine learning such as Graphical models, mixtures and cluster analysis, Variational approximation, advanced Monte Carlo sampling methods, sequential data and Gaussian processes. All topics are illustrated via real-world examples and are contrasted against non-Bayesian approaches.

### Prerequisites

Basic knowledge in probability and first course in statistics such as ST202 or equivalent Probability Distribution Theory and Inference; basic knowledge of the principles of computer programming is sufficient (e.g. in any of Python, R, Matlab, C, Java). This is desired rather than essential. 

### Reading

Lecture slides will be **sufficient** for exam purposes but for optional further reading you can check the books below. 

 - [C. M. Bishop, Pattern Recognition and Machine Learning, Springer 2006](https://www.microsoft.com/en-us/research/uploads/prod/2006/01/Bishop-Pattern-Recognition-and-Machine-Learning-2006.pdf)
 - [K. Murphy, Machine Learning: A Probabilistic Perspective, MIT Press, 2012](https://ebookcentral.proquest.com/lib/londonschoolecons/detail.action?docID=3339490)
 - D. Barber, Bayesian Reasoning and Machine Learning, Cambridge University Press 2012
 - S. Rogers and M. Girolami, A First Course in Machine Learning, Second Edition, Chapman and Hall/CRC, 2016
 
 Specific sections are recommended on the sections from each week below.

### Software

**Python** will be used throughout the course. You can either bring your laptop to the computer classes or use the computer room's PC. If you are using your laptop install [Anaconda (Python 3.7 version)](https://www.anaconda.com/download/)

### Formative coursework

Problem sets will be assigned **each week**. They will include theoretical exercises as well as computer-based assignments. They will be **marked** and returned with **feedback**. Also the marks will appear on LSE FOR YOU.

**Immportant Notes**
 - Submit your problem set in **Columbia House Box 34** 
 - Write the **number of your class group** in the first page

### Assessment

An **individual** project will be assigned on **week 7** and will be **due Tuesday, May 12th noon**. You will be required to analyse data of your choice using the taught Bayesian Machine Learning techniques and present your findings through a paper-like report.

During summer term the course is assessed by a 2 hour **written exam**.

The final grade will be determined by the above with equal weights (**50-50\%**)

### Schedule

---
#### Week 1. Bayesian Inference Concepts

*Topics coverd in Lecture*: 
 - Machine Learning and Bayesian Inference
 - Bayes Estimators, 
 - Credible Intervals
 - Bayesian Forecasting
 - Bayesian Inference via Monte Carlo methods
 
*Reading*:
 - Murphy, Sections 2.1-2.7, 5.2.1, 5.2.2, 6.6.1 and 6.6.2

*Computer Class*: 
 - Introduction to Python, e.g.working with arrays, basic operation and plotting
 - Pseudo-Random numbers
 - Bayesian Inference (Point and Interval Estimation, Forecasting) with Monte Carlo
 
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


