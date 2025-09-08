# Code for Grid Based Simulation of Pyrazine

This repository provides the Python code supporting the manuscript titled **[Quantum Resource Assay for the Grid-Based Simulation of the Photodynamics of Pyrazine]**. 

### Repository Contents

- `Main Simulation.ipynb`: The core simulation notebook. This script generates the time-dependent properties and vibronic data used in the study.
- `Time Dependent Properties Visualization.ipynb`: Processes and visualizes outputs from `Main Simulation.ipynb` for the figures and results presented in **Section IV A** and **Section IV B**.
- `Measurement Shot Estimation-Autocorrelation Based Sampling.ipynb` and `Measurement Shot Estimation-Direct Spectrum Sampling.ipynb`: Scripts used for the results in **Section IV D**, also relying on outputs from `Main Simulation.ipynb`.

### Usage Notes

Please begin by running `Main Simulation.ipynb`, which is required before executing any of the downstream analysis scripts (`Time Dependent Properties Visualization.ipynb`, `Measurement Shot Estimation-Autocorrelation Based Sampling.ipynb`, or `Measurement Shot Estimation-Direct Spectrum Sampling.ipynb`).

Please note that the most computationally demanding part is the fifth code block of `Main Simulation.ipynb`. On a standard laptop (Intel i5 processor, 16 GB RAM), this step took just under 2 hours when executed with ninterval=16.

Please refer to the manuscript for details on methods, parameters, and interpretation of the results.

### Requirements
- Python 3.11.4 
- Jupyter Notebook (ipykernel)

### Software Environment
The code has been tested with the following libraries and versions:
- numpy==1.23.5
- scipy==1.10.1
- matplotlib==3.7.1
- jupyter==1.0.0
