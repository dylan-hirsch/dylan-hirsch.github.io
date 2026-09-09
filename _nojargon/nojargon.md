---
layout: single
title: "No Jargon"
permalink: /nojargon/
author_profile: true
---

Given my interdisciplinary work, it's important to me to be able to communicate effectively with researchers in different fields.
For those who are unfamiliar with some aspect of my work but interested in learning more, here are the basic concepts that underly my research, jargon-free.

### What is control theory? What is reinforcment learning?

Control theory is the field of applied mathematics that engineers across disciplines use when designing feedback control algorithms.
A feedback control algorithm makes decisions in real-time based upon current measurements from the sensors available to the system.
For example, the control algorithm that implements cruise-control in a car uses the current speed of the car to determine how much throttle or braking to apply to maintain a desired speed.
On commerical flights, more sophisticated control algorithms (colloquially called the autopilot) operate planes between takeoff and landing.

Traditionally, control algorithms have been designed using a differential equation model of the system's physics.
These algorithms are called "model-based" approaches.
By contrast, reinforcement learning (RL) is a "model-free" approach to design control algorithms.
In other words, RL approaches learn to control a system by trial-and-error, using either a computational simulator of the system or the real-world system itself.

[Deep RL methods](https://deepmind.google/blog/deep-reinforcement-learning/) use artificial neural networks in the learning process to learn a control algorithm more efficiently than traditional RL methods.
While deep RL methods have demonstrated some impressive feats, including in robotics and self-driving, they are also infamous for producing control algorithms which confidently make bad or unsafe choices.

### What is Hamilton-Jacobi safety analysis?

Hamilton-Jacobi safety analysis (HJSA) is a method by which to design a control algorithm that is optimally safe in a precise mathematical sense.
HJSA comes in both model-based and model-free flavors.

The model-based method takes in a differential-equation model of the system, along with information about the locations of goals and hazards in the environment.
As output, it provides a mathematical function, called the value function, which tells the user from which initial states the task can be safely completed and from which the system will fail under worst-case conditions.

Critically, the value function also encodes the optimally safe feedback-control algorithm for the system, making HJSA a key tool for synthesizing safe controllers.

### What is model reduction?

Model reduction refers to a set of mathematical and ML tools used to take a large mathematical or computational model and produce a smaller one that approximates the behavior of the original.
Some algorithms slow down drastically as model size increases, so model reduction can be used to "pre-process" a model in order to make it more tractable before analyzing it with such algorithms, only minimally sacrificing accuracy in the process.

### How is control theory useful for understanding biology?
Biological systems use sophisticated feedback control mechanisms to maintain homeostasis and respond to perturbations.
The cyclic nature of feedback, however, makes it scientifically difficult to decipher what aspects of a phenotype arise due to an external perturbation (e.g. a disease) versus the organism's response to the perturbation.
Mathematical models and control theoretic analyses can help make sense of these webs of cause and effect.

In addition, these ``dynamical system'' models are useful for understanding what are the minimal components needed to produce some biological phenotype, allowing scientists to reason about complex biological processes.
Such approaches have been useful in understanding [metabolism](https://en.wikipedia.org/wiki/Michaelis–Menten_kinetics), [gene regulation](https://www.google.com/books/edition/An_Introduction_to_Systems_Biology/Lg3MDwAAQBAJ?hl=en&gbpv=1&dq=an+introduction+to+systems+biology&pg=PP1&printsec=frontcover), [action potentials](https://www.nature.com/articles/nn1100_1165), and [reinforcement learning](https://www.annualreviews.org/docserver/fulltext/neuro/35/1/annurev-neuro-062111-150512.pdf?expires=1788981395&id=id&accname=ar-421659&checksum=FF6E3772C287EDDB94D6E382EF8BCB4B).
