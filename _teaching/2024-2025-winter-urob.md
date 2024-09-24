---
title: "B241 - Robot Learning - UROB"
collection: teaching
type: "Undergraduate course"
permalink: /teaching/2024-2025-winter-urob
venue: "CTU FEE, Department of Cybernetics"
date: 2024-09-23
location: "Prague, CZE"
share: false
---

2024/2025 Winter semester

## Course description

The course will teach deep learning methods for well-known robotic problems, such as semantic segmentation or reactive robot motion control. The overall goal is timeless universal knowledge rather than an enumeration of all known deep learning architectures. Students are assumed to have prior knowledge of mathematics (gradient, jacobian, hessian, gradient descend, Taylor polynomial) and machine learning (Bayesian risk minimization, linear classifier). The labs are divided into two parts, in the first part students will solve basic deep ML problems from scratch (including reimplementing autograd backpropagation), in the second part students will build on existing templates to solve complex problems including RL, transformers and generative networks.

All relevant information is available on courseware [here](https://cw.fel.cvut.cz/wiki/courses/b3b33urob/start).

Course's main github repository is available [here](https://github.com/urob-ctu).

Unofficial course materials are available [here](https://urob-ctu.github.io/docs/). Still in development, for extra points you can help us with the development.

## Lab 4: Convolutional Neural Networks

TBA

## Lab 5: Backpropagation

TBA

## HW 2: Autograd

Courseware page is available [here](https://cw.fel.cvut.cz/wiki/courses/b3b33urob/tutorials/hw2).

Github repository of homework is available [here](https://github.com/urob-ctu/hw2-autograd)

In this assignment, it would be your task to implement your own autograd library, similar to the one shown in the lab. The difference is that while in the lab, we showed autograd for scalar values, your solution shall work with vectors and tensors as well.

### Task (10 pts)

The task is to complete the engine.py file. Here, you will find ellipses (…), where you should complete the functions to compute forward and backward passes correctly. There are also starting and ending with recognizable comments. Inside them, you should provide your own code. These are used for longer sections of code. In this homework, they are inside higher-level functions of the autograd.

You will be using the `numpy` library; its documentation may be found [here](https://numpy.org/doc/stable/index.html). Do NOT use any libraries with autograd, such as `PyTorch` or `Tensorflow`.

Most of the functions should be elementary. However, if you are unsure how to proceed with more complex ones, consult the lab materials before contacting tutors.

Please be aware that the variable `other` in function `__pow__` is either `int` or `float` and, therefore, cannot be put in the parent set of output. Backpropagation is available only for objects in the class `Tensor`.

Another tip is that the `reshape_gradient` function is only needed in `__add__` and `__mul__` functions. Only in these two functions do we have the possibility of broadcasting. The `reshape_gradient` function aims to solve the problem of calculating the gradient for broadcasted values.

### Getting started

1. **Get files:** Either download the files as a zip or clone the repository:

```bash
git clone https://github.com/urob-ctu/hw2-autograd.git
```

2. **Install requirements:** There are some Python requirements you need to have installed:

```bash
pip install -r requirements.txt
```

3. **Complete homework:** You may work on the assignment.

### Testing

You may use the provided file `test.py` to test your implementation. Similar but slightly different tests will be used for grading. Make sure to test your implementation thoroughly. The testing file is not exhaustive.

To run the tests, you may use the following command:

```bash
python test.py
```

### Submission and evaluation

The whole directory with all files provided in the assignment file must be zipped and uploaded to BRUTE. You may use the provided bash script to zip the directory:

```bash
./submit.sh
```

The maximum amount of points you may get is 10. The whole assignment will be auto-evaluated in BRUTE. The tutors may later re-evaluate any submission.

You will receive minus one point for every 24 hours after the deadline. However, no more than 9 points will be deducted for late submission.

Good luck, do not forget to play with the task a bit, and in the case of any questions or concerns please contact me.
