# Theoretical Autonomous Satellite Collision Avoidance (TASCA)
A lightweight, Python-based prototype for autonomous collision avoidance in low-Earth orbit using a supervised imitation approach (oracle → neural network) with 3D visualization.

### What this notebook contains
1. Clohessy-Wiltshire relative-motion simulator (LVLH frame) with RK4 propagation.
2. A simple rule-based oracle that computes a single impulsive ∆v to raise the closest-approach distance.
3. Synthetic dataset generation.
4. A small feedforward neural network (numpy) trained to imitate the oracle.
5. 3D visualization of nominal vs NN-avoided vs oracle-avoided trajectories using `matplotlib`.
6. 3D animation generator of how the debris and chaser move together over time.
7. Save/load checkpoint utilities.
8. Two-line element (TLE) ingestion with conversion to LVLH relative state.
