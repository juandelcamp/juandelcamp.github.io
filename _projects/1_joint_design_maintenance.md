---
layout: page
title: Joint pavement design & maintenance with pre-trained RL
description: One deep RL agent that designs and maintains pavements across many projects, with MIT CSHub.
importance: 1
category: research
---

Pavement design and maintenance are usually decided separately: engineers pick a structure, and an agency later decides when and how to repair it. This project optimizes both together.

In collaboration with the [MIT Concrete Sustainability Hub](https://cshub.mit.edu/) (Dr. Randolph Kirchain and Dr. Haoran Li), we:

- formulated CSHub's life-cycle cost and environmental models as a sequential decision problem;
- trained a **dueling double deep Q-network (D3QN)** with prioritized experience replay on randomized pavement contexts (structure, materials, traffic, stochastic roughness deterioration), so a single maintenance and rehabilitation policy serves many projects without retraining;
- reused the trained value function as a **zero-shot surrogate** to screen thousands of candidate concrete pavement designs, then selected the final design with a Monte Carlo elimination tournament, all on a single workstation;
- extended the agent to take the **discount rate** as an input, so agencies using different rates can apply it directly.

The life-cycle cost scope covers construction, maintenance, pavement–vehicle interaction, and end of life, using neural-network surrogates of mechanistic-empirical distress models.

This work has been accepted for presentation at the Transportation Research Board 106th Annual Meeting (January 2027).
