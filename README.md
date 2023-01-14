# Two-Link Planar Elbow Arm Trajectory Tracking

This repository contains the Simulink code for tracking a desired trajectory for a two-link planar robotic manipulator arm. The dynamics of the arm are defined using the Euler-Lagrange equation and controlled using a model-based nonlinear control input (Part 1) and a Proportional-Derivative (PD) control input (Part 2).
## Usage

Open the provided Simulink model in MATLAB.
Click the green "Run" button to start the simulation.
The simulation results can be observed in the scope blocks.

## Parameters

The model parameters used in the simulation are:

    m1 = 3.473 kg (mass of first link)
    m2 = 0.196 kg (mass of second link)
    a1 = a2 = 1 m (length of links)
    g = 9.81 m/s^2 (acceleration due to gravity)
    f1 = 5.3 Nm.s (friction coefficient of first link)
    f2 = 1.1 Nm.s (friction coefficient of second link)

## Note

   The desired trajectory for the arm is defined as qd = [π/3 + π/6sin(t), π/4 + π/6cos(t)].
    The controller gains used in the PD control input (Part 2) are chosen as KP = [15,20] and KD = [8,10]. These values can be adjusted for better ## performance.
    The results of the simulation are plotted in the scope blocks.

## References

   Robotics, Vision & Control: Fundamental Algorithms In MATLAB, 2nd edition" by Peter Corke.
   
   Modeling, Identification and Control of Robots" by L. Sciavicco, B. Siciliano, L. Villani.
