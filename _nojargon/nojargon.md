---
layout: single
title: "No Jargon"
permalink: /nojargon/
author_profile: true
---

Given my interdisciplinary work, it's important to me to be able to communicate effectively with researchers in different fields.
For those who are unfamiliar with some aspect of my work but interested in learning more, here are the basic concepts that underly my research, jargon-free.

## What is Control Theory? What is Reinforcment Learning?

Control theory is the field of applied mathematics that engineers use when designing feedback control algorithms.
A feedback control algorithm makes decisions in real-time based upon current measurements from the sensors available to the system.
For example, the control algorithm that implements cruise-control in a car uses the current speed of the car to determine how much throttle or braking to apply to maintain a desired speed.
On commerical flights, more sophisticated control algorithms (colloquially called the autopilot) operate planes between takeoff and landing.

Traditionally, control algorithms have been designed using a differential equation model of the system's physics.
These algorithms are called "model-based" approaches.
By contrast, reinforcement learning (RL) is a "model-free" approach to design control algorithms.
In other words, they learn to control a system by trial-and-error, using either a computational simulator of the system or the real-world system itself.

Deep RL methods use artificial neural networks in the learning process to learn a control algorithm more efficiently than traditional RL methods.
While deep RL methods have demonstrated some impressive feats, including in robotics and self-driving, they are also infamous for producing control algorithms which confidently make bad or unsafe choices.

### What is Hamilton-Jacobi safety analysis?

Hamilton-Jacobi safety analysis (HJSA) is a method by which to design a control algorithm that is optimally safe in a precise mathematical sense.
HJSA comes in model-based and model-free flavors.

The model-based method takes in a differential-equation model of the system, along with information about the locations of goals and hazards in the environment.
As output, it provides a mathematical function, called the value function, which tells the user from which initial states the task can be safely completed and from which the system will fail under worst-case conditions.
The value function also encodes the optimally safe feedback-control algorithm for the system.

### What is Model Reduction?

TBD.

## What is Computational Biology?

TBD.

### What is a Gene Network?

TBD.

## Where do control theory and biology intersect?

TBD.

### How is control theory useful in biology & medicine?

TBD.

### What does biology teach us about control theory?

TBD.
