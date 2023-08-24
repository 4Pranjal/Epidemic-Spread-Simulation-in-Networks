# Epidemic Spread Simulation in Networks

This repository contains Python code to simulate the spread of infections in networks using the Susceptible-Infected (SI) model. The simulation is performed through a Monte Carlo approach on different types of networks, including Erdos-Renyi and Scale-Free networks. The code analyzes how network structure and parameters influence the dynamics of epidemic spread.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Functions](#functions)
- [Epidemic Spread Simulation](#epidemic-spread-simulation)
- [Results Visualization](#results-visualization)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Susceptible-Infected (SI) model is a basic epidemiological model used to study the spread of infections in a population. This repository demonstrates the simulation of epidemic spread in networks using the SI model. It explores how different network types and parameters (transmission rate and recovery rate) affect the dynamics of infection propagation.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/4Pranjal/epidemic-spread-simulation.git
   cd epidemic-spread-simulation
   ```

2. Install required libraries:
   ```bash
   pip install networkx numpy matplotlib tqdm
   ```

3. Run the provided Python script to perform the simulation and analysis.

## Usage

1. Open the Python script `epidemic_spread_simulation.py` in your preferred Python environment.
2. Run the script to perform simulations and visualize the results.
3. Adjust parameters, network types, and other settings as needed.

## Functions

Several utility functions are defined to facilitate the epidemic spread simulation and analysis:

- `generate_network(network_type, size, *args)`: Generates different types of networks (Erdos-Renyi or Scale-Free) based on provided parameters.
- `initialize_states(G, initial_infected)`: Initializes the states of nodes in the network as 'S' or 'I' (Susceptible or Infected).
- `monte_carlo_simulation(G, beta, mu, time_steps, repetitions)`: Performs Monte Carlo simulations of the SI model on the network.
- `plot_results(results_list)`: Plots simulation results for various parameter combinations.

## Epidemic Spread Simulation

The simulation is carried out using the Monte Carlo method. The following steps are executed:

1. Network generation based on provided network parameters.
2. Initialization of node states (Susceptible or Infected).
3. Iteration through time steps to simulate infection spread.
4. Updates to node states based on transmission and recovery probabilities.

## Results Visualization

Simulation results are visualized using matplotlib. The code generates plots that showcase how infection spreads in different types of networks under varying parameter conditions. Plots illustrate the fraction of infected nodes over time steps.

## Contributing

Contributions to improve code functionality, optimize simulations, or enhance the documentation are welcome. Here's how you can contribute:

1. Fork the repository.
2. Create a new branch.
3. Make your improvements.
4. Open a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
