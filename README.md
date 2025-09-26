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

## Usage Examples

### Basic Execution

```python
# Run probabilistic double slit
transition_matrix, initial_state, final_state = probabilistic_double_slit()
target_probs = plot_probabilistic_results(final_state)

# Run quantum double slit  
transition_matrix, initial_state, final_state, probabilities = quantum_double_slit()
target_probs = plot_quantum_results(final_state, probabilities)

# Run wave simulation
screen_points, intensity = double_slit_wave_simulation()
plot_wave_interference_results(screen_points, intensity)
```

### Advanced Analysis

```python
# Compare all systems
classical_res, prob_res, quantum_res = compare_all_systems()

# Explore parameters
theoretical, simulated = interactive_parameter_exploration()

# Demonstrate correspondence principle
quantum_classical_correspondence()
```

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

## Results and Validation

### Key Findings

1. **Probabilistic System**: Perfect uniform distribution (0.333 probability each target)
2. **Quantum System**: Strong interference effects (0.667 at center, 0.000 at edges)  
3. **Wave Simulation**: Accurate fringe spacing (0.50 ± 0.01 mm vs theoretical 0.50 mm)
4. **Pattern Visibility**: Excellent contrast (0.995) indicating coherent interference

### Advanced Analysis Results

- **Information Entropy**: Quantum system (0.390 bits) vs Probabilistic (1.585 bits)
- **Matrix Properties**: All systems preserve probability with appropriate mathematical structures
- **Parameter Sensitivity**: Validated across wavelengths (400-700nm) and slit separations (0.5-2.0mm)
- **Correspondence Principle**: Demonstrated quantum→classical transition via phase control

### 🧪 **Quality Assurance**

#### ✅ **Comprehensive Test Suite**
- **Status**: All 5 test categories PASSED ✅
- Probabilistic system validation
- Quantum interference verification  
- Wave simulation accuracy checks
- Matrix properties confirmation
- Information entropy calculations

#### 📋 **Test Results**
```
CLASSICAL TO QUANTUM SYSTEMS - TEST SUITE
==================================================
✓ Probabilistic system tests passed
✓ Quantum system tests passed  
✓ Wave simulation tests passed
✓ Matrix properties tests passed
✓ Information entropy tests passed
==================================================
TEST RESULTS: 5 passed, 0 failed
🎉 All tests passed! System implementation is validated.
```

## Educational Value

This project demonstrates:

- **Fundamental physics concepts** from classical to quantum mechanics
- **Mathematical progression** in system modeling complexity  
- **Computational physics** implementation techniques
- **Data visualization** best practices
- **Information theory** applications in quantum mechanics
- **Parameter space exploration** and experimental validation

## Authors

- **Andersson Programming** - *Complete implementation* - Quantum Systems Simulation

## License

This project is licensed under the GPL-3.0 License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

- Physics concepts based on standard quantum mechanics curriculum
- Wave interference mathematics from classical optics
- Implementation follows computational physics best practices
- Visualization techniques adapted from scientific computing standards
