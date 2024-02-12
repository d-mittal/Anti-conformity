Population Dynamics with Heterogeneous Preferences on Networks
This repository contains Python code for simulating population dynamics with heterogeneous preferences on networks. The code implements a model where individuals make choices influenced by their preferences and the choices of their neighbors in a network.

Overview
The provided code simulates the dynamics of a population where individuals have heterogeneous preferences and are connected through a network. Key features of the model include:

Modeling of individual preferences: Individuals in the population have heterogeneous preferences represented by a parameter O.
Network structure: The population is represented as a network where agents are connected to each other. The network structure influences the dynamics of individual choices.
Fermi update rule: Individual choices are updated using a Fermi update rule, which takes into account the individual's preference and the influence of their neighbors' choices.
Conformity and anti-conformity: The model includes parameters representing the degree of conformity (frac_w) and anti-conformity (frac_oA) in the population.
Usage
To use the code, follow these steps:

Ensure you have Python installed on your system.
Install the required dependencies using pip install -r requirements.txt.
Run the main.py script with appropriate parameters to conduct simulations.
Parameters
N: Population size.
num_of_iter: Maximum number of iterations for each simulation.
num_of_replicates: Number of replicates for each simulation.
x0A: Initial fraction of the population with choice A.
O: Strengths of the two preferences in the population (e.g., [10, -10]), where a positive (negative) value indicates a preference for A (B).
frac_w: Fraction of anti-conformists in the population.
frac_oA: Fraction of the population preferring A.
beta: Inverse temperature of the Fermi update function.
A: Adjacency matrix of the network of the population.
w: List of conformities of agents.
Output
The code provides the following outputs for each simulation run:

Average equilibrium value of choice A (avg_xa).
Mean volatility of choices during the simulation (volatility).
Average alignment of choice and preference for the entire population (avg_align_a).
Average alignment of choice and preference for conformists (avg_align_c).
Mean time taken to reach equilibrium (time_taken).
License
This project is licensed under the MIT License.

Acknowledgments
This code was developed by Dhruv.
