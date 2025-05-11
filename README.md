# Fluorescence of a Two-Level Atom

This project simulates the fluorescence of a two-level atom using Julia. The simulation involves solving the time evolution of a quantum system under the influence of a laser field and visualizing the excited state population over time.

## Overview

The Hamiltonian of the system is defined as:

$$
H = -\frac{\hbar\delta}{2}\sigma_z + \frac{\hbar\Omega}{2}(\sigma_+ + \sigma_-),
$$

where:
- $\hbar\omega_0$ is the energy difference between the ground and excited states,
- $\omega_L$ is the laser frequency,
- $\delta = \omega_L - \omega_0$ is the detuning,
- $\Omega$ is the Rabi frequency.

For computational purposes, $\hbar$ is set to 1.

## Features

- Define the Hamiltonian and jump operators for the system.
- Simulate the time evolution of the quantum state using the master equation.
- Compute the expectation value of the excited state population.
- Visualize the results using plots.

## Requirements

The following Julia packages are required:
- `QuantumOptics`
- `CairoMakie`
- `LaTeXStrings`
- `Plots`

## Installation

To install the required packages, run the following commands in Julia:

```julia
using Pkg

Pkg.add("QuantumOptics")
Pkg.add("CairoMakie")
Pkg.add("LaTeXStrings")
Pkg.add("Plots")