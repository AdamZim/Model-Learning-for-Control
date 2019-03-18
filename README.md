# Model Learning for Control

This repository explores the implementation of a neural network for model learning control. A basic neural network shall be constructed from scratch in plain Python. All algorithims shall be implemented from scratch without the addition of any machine learning libraries.

The goal is to train a neural network to model the phyiscal system describing a robotic arm.  The trained model will then be used in a feed-forward control system to compute the torque inputs that will move the robot along a specified trajectory.

The robotic arm being modeled is the Barrett Upper-extremity Robotic Trainer, or [Burt®](https://www.barrett.com/burt-research).  
(Formerly known as [Proficio™](https://www.youtube.com/watch?v=-JHwO8LvRvo))
  
>Burt® is the world's first advanced and affordable end-effector robotic manipulator for upper-extremity rehabilitation training and robotics research which is based on the proven WAM technology developed by Barrett Technology.  With transparent dynamics, low inertia, and mass, Burt® is designed to be a 3D haptic device of choice for those who desire high-fidelity force feedback throughout a human-sized work volume.  Burt® supports researchers with new hardware and software modalities necessary for robotics research.*

The training data in "traning.csv" contains ten different trajectories.  
Formatted:

| $t$ | $x_1$ | $x_2$ | $x_3$ | $\dot{x_1}$ | $\dot{x_2}$ | $\dot{x_3}$ | $\tau_1$ | $\tau_2$ | $\tau_3$ |
| :--- | :---- | :---- | :---- | :---------- | :---------- | :---------- | :------- | :------- | :------- |

$t$ is time (seconds), $x$ is the angular position (radians) for each joint, $\dot{x}$ is the angular velocity (radians/s) for each joint, and $\tau$ is the torque for each joint.

The test data in "training1.csv" and "training2.csv" describe two new and distinct trajectories. Each file consists of the series of joint angles, velocities, and times when the robot should be at each vector of joint angles.