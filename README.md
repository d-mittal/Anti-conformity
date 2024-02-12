# Collective Decision-Making Dynamics with Heterogeneous Preferences on Networks

This repository contains Python code for ABM simulations of collective decision-making dynamics in heterogeneous populations with (evolving) preferences and differing conforming tendencies on networks. The code implements a model where individuals make choices influenced by their preferences and the choices of their neighbors in a network. 


## Code Overview

The repository includes three main Python scripts:

1. `one_run_network.py`: This script simulates population dynamics with heterogenous preferences on networks. It implements a model where individuals update their choices based on their preferences and the choices of their neighbors on a fixed graph.

2. `one_run_well_mixed.py`: This script simulates population dynamics with heterogenous preferences connected probabilistically, mimicking a well-mixed limit. It models a scenario where individuals' choices are influenced by their preferences, the choices of randomly sampled neighbors.

3. `one_run_net_dynamic.py`: This script simulates population dynamics with evolving preferences on networks. It implements a model where individuals update their choices based on their evolving preferences (which are shared by all agents) and the choices of their neighbors on a fixed graph. 

4. `README.md`: This file provides information about the code and how to use it.

## Usage

To use the code:

1. Ensure you have Python installed on your system.
2. These scripts are completely based on Numpy. 
3. Run the desired Python script with appropriate parameters to conduct simulations.

## Parameters

Each Python script takes various parameters to customize the simulation, including population size, number of iterations, initial fraction of the population with a specific choice, strengths of preferences, fractions of conformists and anti-conformists, inverse temperature for the Fermi update function, adjacency matrix of the network, and lists of conformities of agents.

## Output

`one_run_network.py` and `one_run_well_mixed.py` have the following output:

- Equilibrium fraction of choice A in the population
- Equilibrium alignment of choice and preference for the entire population.
- Equilibrium alignment of choice and preference for the conforming subpopulation.
- Time taken for the population to reach equilibrium
- Volatility in choices at the end of the simulation

  
`one_run_net_dynamic.py` has the following output: 

- Time series of the fraction of individuals choosing option A in the conforming and the anti-conforming subpopulations, as well as the entire population.
- Average alignment of choice and preference for the conforming and the anti-conforming subpopulations.
- Average satisfaction of the population over time.
- Average social pressure to choose option A over time.

## License

This project is licensed under the MIT License.

## Acknowledgments

This code was developed by Dhruv.
