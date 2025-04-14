# VM Placement Using Multi-Objective Reinforcement Learning (MORL)

This project demonstrates the Virtual Machine (VM) placement problem in data centers using both heuristic algorithms and a Multi-Objective Reinforcement Learning (MORL) approach. The aim is to minimize **energy consumption** and **resource wastage** while placing VMs on Physical Machines (PMs).

## 📌 Features

- Simulates PMs and VMs with CPU and memory constraints.
- Implements a MORL agent using Chebyshev scalarization to balance energy and wastage objectives.
- Compares MORL agent's performance with classic heuristic algorithms:
  - Best Fit
  - Worst Fit
- Visualizes results with bar charts comparing:
  - Energy consumption
  - Resource wastage

## 🧠 Algorithms Implemented

### ✅ Heuristic Algorithms:
- **Best Fit**: Places VM in the PM with the least remaining space after placement.
- **Worst Fit**: Places VM in the PM with the most remaining space after placement.

### ✅ MORL Agent:
- Learns optimal placement using Q-learning for each objective.
- Scalarizes multiple objectives using Chebyshev method.
- Updates based on simulated episodes of VM placements.

## 📊 Evaluation Metrics

- **Energy Consumption**: Based on CPU utilization and PM power profile.
- **Resource Wastage**: Difference between CPU and memory residuals.

## 🔧 Requirements

- Python 3.x
- NumPy
- Matplotlib

Install requirements:
```bash
pip install numpy matplotlib
