# Classical to Quantum Systems Simulation

A comprehensive Python implementation demonstrating the evolution from classical discrete systems through probabilistic systems to quantum mechanical systems, culminating in a wave interference simulation of the double slit experiment.

## Overview

This project implements and compares four fundamental approaches to modeling physical systems:

1. **Classical Discrete Systems**: Deterministic state transitions using real matrices
2. **Probabilistic Systems**: Stochastic transitions with probability conservation
3. **Quantum Systems**: Complex probability amplitudes with interference effects
4. **Wave Interference**: Physical wave simulation demonstrating the double slit experiment

## Getting Started

### Prerequisites

- Python 3.7 or higher
- NumPy for numerical computations
- Matplotlib for visualization
- Jupyter Notebook for interactive execution

```bash
pip install numpy matplotlib jupyter
```

### Installation

1. Clone the repository:

```bash
git clone https://github.com/AnderssonProgramming/quantum-systems-py.git
cd quantum-systems-py
```

2. Launch Jupyter Notebook:

```bash
jupyter notebook TallerClasicToQuantum.ipynb
```

3. Run all cells sequentially to see the complete demonstration

## Features

- **Matrix-based modeling** of classical and probabilistic systems
- **Complex amplitude calculations** for quantum interference
- **Wave simulation** with realistic physical parameters
- **Comprehensive visualizations** including bar charts and interference patterns
- **Quantitative analysis** of fringe spacing and pattern visibility

## System Implementations

### 1. Probabilistic Double Slit (Exercise 1)

Models photon behavior through probability matrices:

- **Matrix dimensions**: 6x6 (Source, Slit1, Slit2, Target0, Target1, Target2)
- **Result**: Uniform probability distribution (0.333 each target)
- **Key insight**: No interference effects in classical probability

### 2. Quantum Double Slit (Exercise 2)

Implements quantum superposition with complex amplitudes:

- **Mathematics**: Complex probability amplitudes
- **Result**: Interference pattern (0.667 at Target1, 0.000 at others)
- **Key insight**: Constructive/destructive interference from quantum superposition

### 3. Wave Interference Simulation (Exercise 3)

Physical wave model with realistic parameters:

- **Wavelength**: 500 nm (green light)
- **Slit separation**: 1.0 mm
- **Screen distance**: 1.0 m
- **Result**: Fringe spacing ~0.5 mm (matches theory)

## Performance Metrics

- **Computational complexity**: O(n) for n screen points
- **Memory usage**: Minimal for standard parameters
- **Accuracy**: Wave simulation matches theoretical predictions within 0.01 mm

## Built With

- [NumPy](https://numpy.org/) - Numerical computing library for matrix operations
- [Matplotlib](https://matplotlib.org/) - Plotting library for visualizations
- [Jupyter](https://jupyter.org/) - Interactive notebook environment

## Technical Implementation

### Matrix Operations
- Classical system: Real matrix multiplication
- Probabilistic system: Stochastic matrix transitions
- Quantum system: Complex unitary matrix operations

### Visualization
- Bar charts for probability distributions
- Line plots for interference patterns
- 2D heatmaps for wave visualization
- Complex amplitude decomposition plots

## Educational Value

This project demonstrates:
- **Fundamental physics concepts** from classical to quantum mechanics
- **Mathematical progression** in system modeling complexity
- **Computational physics** implementation techniques
- **Data visualization** best practices

## Authors

- **Systems Engineering Student** - *Complete implementation* - Quantum Systems Simulation

## License

This project is licensed under the MIT License - see the LICENSE file for details

## Acknowledgments

- Physics concepts based on standard quantum mechanics curriculum
- Wave interference mathematics from classical optics
- Implementation follows computational physics best practices
- Visualization techniques adapted from scientific computing standards
