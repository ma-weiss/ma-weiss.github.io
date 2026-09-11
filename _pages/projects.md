---
permalink: /projects/
title: "Projects"
author_profile: true
---

My research explores inductive biases in machine learning as applied to robotics and control problems. Within this domain, I concentrate on two questions:

- What roles do inductive biases play in improving the performance and generalization of robot learning algorithms?
- How can inductive biases be systematically integrated into generic deep learning frameworks to enhance their applicability to robotic tasks?

A full list of my papers is on the [Publications](/publications/) page.

---

## Using Lagrangian Neural Networks for Computed Torque Control

<figure class="figure-center">
  <img src="/images/teaser_ral26.png" alt="Block diagram: learned inverse dynamics and a PD controller form a computed torque controller that tracks a desired trajectory on a robot arm with unknown dynamics">
  <figcaption>Schematic of the proposed LNN-CTC framework</figcaption>
</figure>

This research presents a physics-informed control framework that integrates Lagrangian Neural Networks (LNNs) into a Computed Torque Control (CTC) architecture for accurate and adaptive robotic trajectory tracking. Instead of relying on precise analytic models, the LNN learns the robot’s inverse dynamics directly from data while enforcing physical consistency through Lagrangian mechanics.

By embedding the learned model inside the feedback-linearization loop (LNN-CTC), the controller shapes the closed-loop error dynamics rather than adding a simple feedforward correction. This results in improved tracking accuracy, robustness to disturbances, and strong generalization with minimal training data, outperforming classical model-based and black-box neural controllers.

An online learning extension continuously updates the LNN during operation, enabling rapid adaptation to dynamic changes such as added payloads. The approach achieves fast gravity compensation, data-efficient learning, and real-time performance without prior model knowledge, making it well suited for robots operating under uncertain and changing conditions.

Papers: [[RA-L 2026](https://doi.org/10.1109/LRA.2026.3653326)] [[CoDIT 2025](https://doi.org/10.1109/CoDIT66093.2025.11321475)]

---

## Real-Time Learning Control for Quadruped Robot Velocity Tracking

<figure class="figure-center">
  <video src="/images/go1-walking.mp4" poster="/images/go1-walking.jpg" autoplay loop muted playsinline aria-label="Go1 quadruped robot walking on a safety tether"></video>
  <figcaption>Go1 quadruped robot walking</figcaption>
</figure>

This research presents a control framework for quadruped robots that achieves accurate velocity tracking by combining Proportional-Derivative (PD) control, Iterative Learning Control (ILC), and Gaussian Process Regression (GPR). The PD controller provides real-time feedback using inverse kinematics, while ILC learns feedforward torques from repetitive gait cycles to compensate for unmodeled dynamics. GPR then generalizes these learned torques across different velocities, eliminating the need for relearning at each speed.

Papers: [[ECC 2024](https://doi.org/10.23919/ECC64448.2024.10590932)] [[ICARCV 2024](https://doi.org/10.1109/ICARCV63323.2024.10821620)]
