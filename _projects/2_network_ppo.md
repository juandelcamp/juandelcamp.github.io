---
layout: page
title: Network-level pavement management with PPO
description: Coordinating treatments across hundreds of road segments under annual budget limits.
importance: 2
category: research
---

Managing a road network is more than managing each segment on its own. Treating adjacent segments together creates economies of scale, and every decision competes for the same annual budget.

I developed a **proximal policy optimization (PPO)** agent with a **1-D convolutional actor–critic** that captures these interdependencies between neighbouring segments. On a 159-segment Interstate network (I-95, Virginia, using HPMS data), the learned policy is compared against a two-stage bottom-up benchmark on expected condition and budget exceedance.

Earlier related work with SiYuan Song was presented at the Transportation Research Board 103rd Annual Meeting (2024).
