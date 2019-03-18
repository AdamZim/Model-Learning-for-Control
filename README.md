# Model Learning for Control

This repository explores the implementation of a neural network for model learning control. A basic neural network shall be constructed from scratch in plain Python. All algorithims shall be implemented from scratch without the addition of any machine learning libraries.

The goal is to train a neural network to model the phyiscal system describing a robotic arm.  The trained model will then be used in a feed-forward control system to compute the torque inputs that will move the robot along a specified trajectory.

The robotic arm being modeled is the Barrett Upper-extremity Robotic Trainer, or [Burt®](https://www.barrett.com/burt-research).  
(Formerly known as [Proficio™](https://www.youtube.com/watch?v=-JHwO8LvRvo))
  
>Burt® is the world's first advanced and affordable end-effector robotic manipulator for upper-extremity rehabilitation training and robotics research which is based on the proven WAM technology developed by Barrett Technology.  With transparent dynamics, low inertia, and mass, Burt® is designed to be a 3D haptic device of choice for those who desire high-fidelity force feedback throughout a human-sized work volume.  Burt® supports researchers with new hardware and software modalities necessary for robotics research.* 

Training data provided 