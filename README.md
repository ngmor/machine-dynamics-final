# ME 314 Machine Dynamics
This repository contains code for my solution to Northwestern University's ME 314 Machine Dynamics final project.

## Introduction
This machine dynamics class teaches analysis of rigid body systems using Lagrangian dynamics, including how to deal with external forces, constraints, and impacts. The class also focuses on using numerical methods and Python's `sympy`, `numpy`, and `plotly` packages to simulate system behavior and then animate that simulation.

For the final project, I chose to model a jack bouncing in a cup. The jack and the cup are subject to gravity, and the cup is subject to two orthogonal external forces and an external torque. To simulate the system, I followed these steps:
1. Define the system state variables.
2. Define frames to describe the system using the state variables.
3. Define kinetic and potential energies in the system using the state variables and other system information.
4. Define external forces/torques.
5. Construct the system Lagrangian.
6. Derive the system Euler-Lagrange equations.
7. Solve the system Euler-Lagrange equations for the second derivatives of the state variables.
8. Define impact conditions based on the system geometry.
9. Derive impact update equations based on the impact conditions and assuming elastic impact.
10. Simulate for a 5 second timespan using a timestep of 0.01 seconds.
    - Calculate the state at each timestep using the solutions to the Euler-Lagrange equations and a Runge-Kutta fourth-order integration scheme.
    - Check all impact conditions at each timestep. If impacts occurred, apply the appropriate impact update and resume the simulation.
11. Animate simulation results.

For details on the system and solution, please see the markdown sections in the project [Jupyter Notebook](final.ipynb), formatted using LaTeX.

## Video
Unfortunately, GitHub cannot render the animation of the simulation at the end of the Jupyter Notebook. In its place, here is a video of the full animation playing, taken after running the Jupyter Notebook code in Google Colaboratory.

[Simulation](https://user-images.githubusercontent.com/113186159/208041850-f88f407a-2f75-4c51-b43a-8c307adc4ab3.mp4)