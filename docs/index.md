---
title: "RealAIGym: Education and Research Platform for Studying Athletic Intelligence"
author: Felix Wiebe, Shubham Vyas, Lasse Maywald, Shivesh Kumar
youtube: JVvwMGYiH3A
github: https://github.com/dfki-ric-underactuated-lab/torque_limited_simple_pendulum
pdf: https://github.com/dfki-ric-underactuated-lab/torque_limited_simple_pendulum
---

## Motivation

Traditional robots today (such as the ones used in factories) have a fixed base and are fully actuated under their operating conditions. However, modern robots inspired by animals are not bound to one place and are always under-actuated. Like animals, these robots can perform dynamic movements, demonstrate compliance, and are robust to contact during their movements. The interest in dynamic robot behaviors has increased significantly due to the impressive athletic behaviors shown by robots developed by *Boston Dynamics*, *MIT Mini Cheetah*, *Agility Robotics* etc. This gives rise to the need for canonical robotic hardware setups for studying underactuation and comparing learning and control algorithms for their performance and robustness. These hardware setups and the accompanying software should be affordable, open and accessible. Similar to *OpenAIGym* and *Stable Baselines* which provide simulated benchmarking environments and baselines for Reinforcement Learning (RL) algorithms, the concept of **RealAIGym**  is introduced with a set of reproducible robotic hardware platforms, for establishing a baseline for the application of dynamic control algorithms on real hardware.

## Gym Equipment
The intention of the RealAIGym is to study dynamic control of underactuated systems. On one hand, the studied systems should be simple in order to be easily reproducible and accessible, whereas on the other hand the complexity of the control problems they offer should be non-trivial, so that qualitative and quantitative results can be obtained by testing, comparing and benchmarking various control methods. The current version of the RealAIGym accommodates five robotic systems of varying Degrees of Freedom (DoF): 

![The gym equipment currently available in the RealAIGym include (from left to right) simple and double pendulum, hopping leg, acromonk and, boomstick hopper](static/figures/gym.png)

### Simple Pendulum [<i class="fa fa-github" style="font-size:24px"></i>](https://github.com/dfki-ric-underactuated-lab/torque_limited_simple_pendulum)
A torque-limited simple pendulum is arguably the simplest underactuated robotic system one could imagine. With only one motor, a link and a weight it can be reproduced easily. A natural control problem for the pendulum is to swing up from the hanging position to the upright position and stabilize the pendulum there with a torque limitation. Setting a torque limitation on the motor output makes it impossible to directly swing up and instead the pendulum needs to built up energy by first swinging back and forth.

### Double Pendulum
A double pendulum is a simple 2-DoF system with chaotic dynamics. The system consists of two links and two motors at the joints. By disabling one of the motors and using it as a passive joint, the system can be operated either as an acrobot or as a pendubot system. Similar to the simple pendulum case, a natural control problem is to swing up the double pendulum from the hanging position to the upright position and stabilize it there.

### Hopping Leg
The hopping leg is a 3-DoF system with two motors and one passive vertical DoF. The leg is able to jump by pushing itself off from the ground. Interesting control problems are maintaining a constant jumping height and performing a backflip during the air phase.

### Acromonk 
An acromonk consists of two links which are joined together by a single motor. Two hooks at the external ends of both links facilitate the acromonk to hold onto horizontal bars. As a free and wireless system the acromonk is capable of performing brachiation behavior similar to primates. The system is similar to an acrobot system from dynamics perspective but provides an additional control challenge due to the brachiation task.

### Boomstick Hopper
The boomstick hopper is similar to the hopping leg but instead of the upright pole the hopper is attached to a boomstick which allows it to hop along a circle.

## Formatting Examples
<mark>Marked text</mark>. **Fat Text** *Cursive text* Footnote [^1]

$$1+1+2+\pi$$


Column A | Column B | Column C
---------|----------|---------
 A1 | B1 | C1
 A2 | B2 | C2
 A3 | B3 | C3

[^1]: test 123
