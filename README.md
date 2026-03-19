# Van der Pol Oscillator: Numerical and Machine Learning Methods

This repository contains code and experiments for solving the **Van der Pol oscillator** using both **numerical solvers** and **machine learning models**. It explores **accuracy**, **noise robustness**, and performance across a range of oscillation parameters. Development was supported by generative AI tools.

---

## Repository Structure

### `ml/`  
Contains machine learning implementations for solving the Van der Pol oscillator.  

- **`solver.py`** – Solves the oscillator using the following methods:  
  - Euler  
  - RK4  
  - RK45  
  - BDF  

- **`error.py`** – Computes the **RMSE** across different values of `mu` compared to a highly accurate RK45 solver.

---

### `numerical/`  
Contains neural network-based solvers for the Van der Pol oscillator.  

- **`solver.py`** – Implements the following models:  
  - Baseline Neural Network (NN)  
  - Residual Network (ResNet)  
  - Physics-Informed Neural Network (PINN)  

- **`error.py`** – Computes the **RMSE** across different `mu` values compared to a highly accurate RK45 solver.

---

### `experiments/`  
Contains scripts for exploring oscillator behavior and training robustness.  

- **`amplitude_period.py`** – Computes amplitude and period as functions of `mu`.  
- **`noise.py`** – Introduces noise into the training data and compares performance of different machine learning methods.

---

## Getting Started

1. Clone the repository:  
```bash
git clone <your-repo-url>
