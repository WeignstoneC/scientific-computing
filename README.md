# Scientific Computing – BIT2118

<p align="center">
  <strong>Numerical Methods and Scientific Computing with Python</strong>
</p>

<p align="center">
  A collaborative academic project demonstrating the application of scientific computing and numerical methods to mathematical and computational problems.
</p>

---

## About the Project

This repository contains the practical coursework and Python implementations developed for **BIT2118 – Scientific Computing**.

The project explores numerical methods, computational techniques, and their applications in solving mathematical problems. It is organised into three sections covering Tasks 1–8, Tasks 9–12, and Tasks 13–20.

The implementations demonstrate how mathematical concepts can be translated into Python programs to obtain numerical solutions, perform calculations, and interpret computational results.

## Project Objectives

The main objectives of this project are to:

- Apply scientific computing concepts using Python.
- Implement numerical methods for solving mathematical problems.
- Develop computational solutions using appropriate Python libraries.
- Analyse and interpret numerical results.
- Explore the accuracy, convergence, and limitations of numerical techniques.
- Develop collaborative programming and version-control skills using Git and GitHub.

## Repository Structure

The repository is organised into the following sections:

```text
scientific-computing/
│
├── TASK 1-8/
│   └── Solutions and resources for Tasks 1–8
│
├── numerical-methods-task-9-12/
│   ├── README.md
│   ├── requirements.txt
│   ├── .gitignore
│   │
│   ├── tasks/
│   │   ├── __init__.py
│   │   ├── task_09_eigenvalues.py
│   │   ├── task_10_bisection_fixed_point.py
│   │   ├── task_11_newton_secant.py
│   │   └── task_12_nonlinear_equations.py
│   │
│   ├── tests/
│   │   └── test_tasks.py
│   │
│   └── outputs/
│       ├── task_09_network_centrality.png
│       ├── task_10_heat_balance.png
│       ├── task_10_fixed_point_convergence.png
│       ├── task_12_intersections.png
│       └── execution_results.md
│
└── TASK 13-20/
    └── Solutions and resources for Tasks 13–20
```

## Project Sections

### 1. Tasks 1–8

Contains the solutions and resources for the first section of the Scientific Computing coursework.

[View Tasks 1–8](./TASK%201-8/)

### 2. Tasks 9–12: Numerical Methods

This section focuses on implementing numerical methods in Python and applying them to practical scenarios.

| Task | Numerical Method | Application |
|---|---|---|
| Task 9 | Eigenvalues and Eigenvectors | Campus network analysis |
| Task 10 | Bisection and Fixed-Point Iteration | Greenhouse temperature equilibrium |
| Task 11 | Newton-Raphson and Secant Methods | Solar-powered water pumping investment |
| Task 12 | Nonlinear Equation Solving | Reservoir and embankment design |

**Key features:**

- Matrix operations and eigenvector centrality.
- Numerical root-finding and convergence analysis.
- Comparison of numerical algorithms.
- Solving systems of nonlinear equations.
- Graphical representation of numerical results.
- Automated testing of implemented methods.

[View Tasks 9–12](./numerical-methods-task-9-12/)

### 3. Tasks 13–20

Contains the solutions and resources for the final section of the Scientific Computing coursework.

[View Tasks 13–20](./TASK%2013-20/)

## Technologies and Tools

The project uses the following technologies where applicable:

| Technology | Purpose |
|---|---|
| Python 3 | Main programming language |
| NumPy | Numerical operations and matrix calculations |
| SciPy | Scientific and numerical algorithms |
| Matplotlib | Data visualisation and plotting |
| Pytest | Automated testing |
| Git | Version control |
| GitHub | Collaborative development and project hosting |

## Getting Started

### Prerequisites

Ensure that you have the following installed:

- Python 3
- Git
- pip (Python package installer)

### Clone the Repository

Open your terminal and run:

```bash
git clone https://github.com/WeignstoneC/scientific-computing.git
```

Navigate into the repository:

```bash
cd scientific-computing
```

### Running Tasks 9–12

Navigate to the numerical methods section:

```bash
cd numerical-methods-task-9-12
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Run the individual programs:

```bash
python -m tasks.task_09_eigenvalues
```

```bash
python -m tasks.task_10_bisection_fixed_point
```

```bash
python -m tasks.task_11_newton_secant
```

```bash
python -m tasks.task_12_nonlinear_equations
```

### Running Automated Tests

From inside `numerical-methods-task-9-12`, execute:

```bash
pytest -v
```

The tests check the implemented numerical methods and verify that the calculated solutions satisfy the relevant mathematical conditions.

## Results and Visualisation

The Tasks 9–12 section includes generated graphs and numerical results.

The `outputs/` directory contains:

- Campus network centrality comparison.
- Greenhouse heat-balance graph.
- Fixed-point iteration convergence graph.
- Reservoir and embankment intersection graph.
- Numerical execution results and interpretations.

These outputs help demonstrate the behaviour of the numerical methods and the effects of changing selected parameters.

## Collaboration and Version Control

This project is maintained collaboratively using Git and GitHub.

Contributors can work on separate branches, implement their assigned tasks, and submit pull requests for review before merging their changes into the main branch.

Suggested branch naming convention:

```text
feature/task-description
```

Example:

```text
feature/bit2118-tasks-09-12
```

Suggested commit message format:

```text
Add solutions for BIT2118 tasks 9-12
```

## Assumptions and Limitations

Numerical solutions depend on the mathematical models, input parameters, initial estimates, and convergence criteria used in each implementation.

Where illustrative scenarios are used, their input values should be treated as assumptions rather than verified real-world measurements.

Results should therefore be interpreted in the context of the models and methods used.

## Academic Information

| Detail | Information |
|---|---|
| Course | BIT2118 |
| Course Name | Scientific Computing |
| Project | Numerical Methods and Scientific Computing |
| Programming Language | Python |
| Repository | scientific-computing |

## Contributors

This repository is a collaborative coursework project.

Contributions are organised according to the task sections and individual responsibilities of the group members.

---

<p align="center">
  <strong>BIT2118 – Scientific Computing</strong><br>
  Numerical Methods • Python • Computational Problem Solving
</p>
