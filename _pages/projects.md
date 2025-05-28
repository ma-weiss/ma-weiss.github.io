---
permalink: /projects/
title: "Projects"
author_profile: true
---

My research explores inductive biases in machine learning as applied to robotics and control problems.
Within this domain, I concentrate on:

What roles do inductive biases play in improving the performance and generalization of robot learning algorithms? How can inductive biases be systematically integrated into generic deep learning frameworks to enhance their applicability to robotic tasks?



A full list of all publications can be found at [Google Scholar](https://scholar.google.com/citations?user=rVmmxF8AAAAJ&hl=de)


________


Real-Time Learning Control for Quadruped Robot Velocity Tracking 
======

<div style="flex: 1; padding: 10px;">
<div style="text-align: center; margin-bottom: 0px; margin-top: 0px;">
    <img src="../images/go1.gif" alt="Image not found" width="450"/>
    <p><em>Animation: Go1 Robot walking</em></p>
</div>
</div>
________


This research presents a control framework for quadruped robots that achieves accurate velocity tracking by combining Proportional-Derivative (PD) control, Iterative Learning Control (ILC), and Gaussian Process Regression (GPR). The PD controller provides real-time feedback using inverse kinematics, while ILC learns feedforward torques from repetitive gait cycles to compensate for unmodeled dynamics. GPR then generalizes these learned torques across different velocities, eliminating the need for relearning at each speed.

