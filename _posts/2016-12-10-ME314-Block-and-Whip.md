---
layout: post
title: "Simulation of Whip Colliding with Falling Block"
author: "Elton Cheng"
categories: ControlSim
tags: [Simulation, ME313, Northwestern, Mathematica]
image: 
    feature: whipimage.jpg
---

## Overview

##### Project was completed for ME314: Theory of Machines - Dynamics.

The purpose of this project was to simulate the dynamics of a swinging whip hitting a falling block using the material taught in the course. This included describing the dynamics of the system using the Euler-Lagrange equations, how impacts can affect the system, and how rotational inertia can change due to impacts.

The equation below describes the Lagrangian (L), where T represents the kinetic energy of the system and V represents the potential energy of the system.

$$
\begin{equation}
L = T - V
\end{equation}
$$

We use the Euler-Lagrange equations to solve for the equations of motion of the system, described below.

$$
\begin{equation}
\frac{d}{dt}(\frac{\partial L}{\partial \dot{q}}) - \frac{\partial L}{\partial q} = 0
\end{equation}
$$

Finally, in order to describe the impact that occurs between, we must first solve for when the geometries of the block and the tip of the whip overlap. Using this time of impact, we can find the position and velocities of the whip and block at that time, and solve for the change in velocities after impact using the impact equations described below.

$$
\begin{equation}
\frac{\partial L}{\partial \dot{q}}|^{\tau +}_{\tau - } = \lambda \frac{\partial \phi}{\partial q}
\end{equation}
$$

$$
\begin{equation}
[\frac{\partial L}{\partial \dot{q}}\cdot\dot{q} - L(q,\dot{q})]^{\tau +}_{\tau - } = 0
\end{equation}
$$


Plugging in the velocities after impact into the equations of motion of the system will then describe how the system will continue to behave after impact.

The video image links below shows the simulation of this system slowed down so impact and changes in the system are seen. All video and coding done for this project was done in Mathematica. Source code and write up can be found at this [link]{:target="_blank"}.

<div align="center">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/Bayp_y6na8A" frameborder="0" allowfullscreen></iframe>

    <iframe width="560" height="315" src="https://www.youtube.com/embed/BokumHZa_Mo" frameborder="0" allowfullscreen></iframe>
</div>

[link]:<https://github.com/echeng22/ME314-Final-Project>










