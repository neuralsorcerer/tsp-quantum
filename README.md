# QUBO Optimization Problem using Qiskit

This project demonstrates how to solve a Quadratic Unconstrained Binary Optimization (QUBO) problem using quantum computing with Python and Qiskit. Specifically, we solve the Traveling Salesman Problem (TSP) for a set of cities.

## Project Structure

- `optimization.ipynb`: Main script containing the implementation of the QUBO optimization problem.
- `requirements.txt`: List of Python packages required to run the project.

## Getting Started

### Prerequisites

Make sure you have Python installed. You can download it from [python.org](https://www.python.org/).

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/neuralsorcerer/tsp-quantum.git
   cd tsp-quantum
   ```

2. Create and activate a virtual environment (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

## Running the Project

Execute the `optimization.ipynb` script to solve the TSP and visualize the results:

```bash
jupyter notebook
```

## Explanation

### Problem Definition

The Traveling Salesman Problem (TSP) is a classic optimization problem where the objective is to find the shortest possible route that visits a set of cities and returns to the origin city. This problem can be formulated as a QUBO problem.

### Solution Approach

1. **Define the Problem:** We start by defining the distances between cities.
2. **Convert to QUBO:** The TSP problem is converted into a QUBO problem using Qiskit.
3. **Solve using QAOA:** The QUBO problem is solved using the Quantum Approximate Optimization Algorithm (QAOA).
4. **Visualize Results:** The results are visualized using _matplotlib_ and _networkx_.

### Visualization

- **Distance Matrix:** Displays the distances between each pair of cities.
- **Optimal Path:** Shows the optimal path found by the quantum algorithm.
