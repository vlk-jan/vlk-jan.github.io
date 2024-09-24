---
title: "B231 - Robot Learning - UROB"
collection: teaching
type: "Undergraduate course"
permalink: /teaching/2023-2024-winter-urob
venue: "CTU FEE, Department of Cybernetics"
date: 2023-09-23
location: "Prague, CZE"
share: false
---

2023/2024 Winter semester

## Course description

The course will teach deep learning methods for well-known robotic problems, such as semantic segmentation or reactive robot motion control. The overall goal is timeless universal knowledge rather than an enumeration of all known deep learning architectures. Students are assumed to have prior knowledge of mathematics (gradient, jacobian, hessian, gradient descend, Taylor polynomial) and machine learning (Bayesian risk minimization, linear classifier). The labs are divided into two parts, in the first part students will solve basic deep ML problems from scratch (including reimplementing autograd backpropagation), in the second part students will build on existing templates to solve complex problems including RL, transformers and generative networks.

All relevant information is available on courseware [here](https://cw.fel.cvut.cz/b231/courses/b3b33urob/start).

## HW 1: Autograd

Courseware page is available [here](https://cw.fel.cvut.cz/wiki/courses/b3b33urob/tutorials/hw2).

In this assignment, it would be your task to implement your own autograd library, similar to the one shown in the lab. The difference is that while in the lab, we showed autograd for scalar values, your solution shall work with vectors and tensors as well.

The assignment is divided into two parts. In the first one, you will complete the provided autograd library. In the second one, you will use this library to solve a simple dkt problem.

All necessary files are provided [here](/files/hw01.zip).

### Task 1 (6 pts)

The first task is the completion of the engine.py file. Here you will find ellipses (…), where you should complete the functions to correctly compute forward and backward passes.

You will be using the `numpy` library; its documentation may be found [here](https://numpy.org/doc/stable/index.html). Do NOT use any libraries with autograd, such as `PyTorch` or `Tensorflow`.

Most of the functions should be elementary. However, if you are unsure how to proceed with more complex ones, consult the lab materials before contacting tutors.

Please be aware that the variable `other` in function `__pow__` is either `int` or `float` and, therefore, cannot be put in the parent set of output. Backpropagation is available only for objects in the class `Tensor`.

Another tip is that the `reshape_gradient` function is only needed in `__add__` and `__mul__` functions. Only in these two functions do we have the possibility of broadcasting. The `reshape_gradient` function aims to solve the problem of calculating the gradient for broadcasted values.

### Task 2 (4 pts)

The second task is the completion of computational parts of dkt (direct kinematic task). The robot will later utilize the autograd library you completed to tweak the angles of joints and lengths of arms to reach the desired location.

All necessary information is provided in the hw1.ipynb file. The computational parts of dkt that are to be implemented are in the assignments.py file.

### Submission and evaluation

The maximum amount of points you may get is 10. The whole assignment will be auto-evaluated in BRUTE. The tutors may later re-evaluate any submission.

You will receive minus one point for every 24 hours after the deadline. However, no more than 9 points will be deducted for late submission.

Good luck, do not forget to play with the task a bit, and in the case of any questions or concerns please contact me.
