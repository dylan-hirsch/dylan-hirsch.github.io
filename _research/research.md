---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

My research uses methods from applied mathematics and computer science to develop safer control and reinforcement learning algorithms. These algorithms are usually tailored towards problems in biology and medicine, which are my primary application areas of interest.

## Hamilton-Jacobi safety analysis for designing safety filters
In self-driving cars, neural networks make complex decisions determining how to steer, break, and accelerate. The rapid advancement in robotics has also required neural networks to allow robots to autonomously navigate and operate in factories and industrial settings, often around human workers. Similar to Large Language Models, neural networks used for controlling machines tend to have impressive average performance, but “hallucinations” can result in perplexing and dangerous worst-case performance.

To solve this issue, one can use safety filters, algorithms that predict potential danger and switch to a safer backup algorithm. It is often unclear, however, when to switch algorithms and what the safe algorithm should do. Advances in applied mathematics and computing, in particular the development of Hamilton-Jacobi safety analysis, are now allowing us to use mathematical models of a technological system to automatically synthesize these safety filters. While these algorithms currently work very well for “small” models, they are computationally intractable for more complex, realistic models.

The methodological aspects of my research thus center on making Hamilton-Jacobi safety analysis more capable, flexible, and efficient, with theoretical guarantees.
Doing so involves using ideas from real analysis, general topology, model reduction, reinforcement learning, and partial differential equations.

## Optimal dosing regimens in quantitative pharmacology
TBD.

## Feedback control in biological systems
TBD.
