---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

My research uses methods from applied mathematics and computer science to develop safer control and reinforcement learning algorithms. These algorithms are usually tailored towards problems in biology and medicine, which are my primary application areas of interest.

## Hamilton-Jacobi safety analysis for designing safety filters
In self-driving cars, neural networks make complex decisions determining how to steer, break, and accelerate. The rapid advancement in robotics has also required neural networks to allow robots to autonomously navigate and operate in factories and industrial settings, often around human workers. Similar to Large Language Models, neural networks used for controlling machines tend to have impressive average performance, but “hallucinations” can result in perplexing and dangerous worst-case performance.

To solve this issue, one can use safety filters, algorithms that predict potential danger and switch to a safer backup algorithm. It is often unclear, however, when to switch algorithms and what the safe algorithm should do. Advances in applied mathematics and computing, in particular the development of Hamilton-Jacobi safety analysis, are now allowing us to use mathematical models of a technological system to automatically synthesize these safety filters. While these algorithms currently work very well for small (i.e. low-dimensional) models, they are computationally intractable for large ones.

The methodological aspects of my research thus center on making Hamilton-Jacobi safety analysis more capable, flexible, and efficient, with theoretical guarantees.
Doing so involves using ideas from real analysis, general topology, model reduction, reinforcement learning, and partial differential equations.

## Optimal dosing regimens in quantitative pharmacology
Consider a control task in robotics in which a drone must navigate to some target location while avoiding crashing into hazards (e.g. trees, people, buildings) despite some uncertain dynamics (e.g. wind).
To accomplish this task, a user can provide a mathematical model of the drone as input to the Hamilton-Jacobi safety analysis algorithm.
The algorithm will then provide the optimal motor control policy for the drone to safely complete the task.

Analogously, suppose one wishes to design a drug regimen for a patient in a medical context.
In this case, one similarly wishes to reach some therapeutic target (e.g. desired downstream molecular activities), while avoiding a hazard (drug toxicity), despite unknown dynamics (e.g. paramater uncertainty).
If one supplies a pharmacokinetic / pharmacodynamic (PKPD) model to the algorithm, Hamtilon Jacobi safety analysis will then provide the optimal dosing policy, namely how much of each drug to give the patient at each time, to reach the target while avoiding toxicity.

While such an approach holds much promise, biological models tend to be much higher-dimensional than drone models and pharmacological tasks can be more intricate.
I am working on biology-motivated model reduction and reinforcement learning algorithms to bridge these gaps.

## Feedback control in biological systems
Biological systems are experts at feedback control.
Brains, for example, are essentially the physical implementation of a highly complex feedback control algorithm, and neuroscience research has led to rapid improvements in reinforcement learning.

Cells also implement control algorithms, especially through transcriptional networks.
I am broadly interested in applications of control in systems \& synthetic biolgy.

