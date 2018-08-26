# MonteCarlo_Cpp
Fully 3-Dimensional 1-energy-group Monte Carlo neutron transport solver written in C++.

## Basic Theory
A monte carlo simulator simulates a nuclear reactor, or other neutron transport problem, by simulating single neutrons. A single neutron is created by a fission with some velocity and position. Using this information the probability of collision is calculated, and a random number determines if the collision occured. Using more probabilities the neutron's state is updated. This continues until the neutron dies by being absorbed by a material or leaving the reactor.

## Features
- Uses full 3-D quadratic surfaces allowing future expansion.
- Energy is fully tracked simplifying conversion from one-group to point-wise cross-sections.
- Allows source-driven problems
- Supports tallies including:
  - Track length tallies
  -  Collision tallies
 - Mesh tallies
- Can implement:
  - Surface tallies
  - Cell tallies
