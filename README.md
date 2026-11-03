#BIT 2118: Scientific Computing
#1. About this repository

This repository contains my work on the BIT 2118 group work brief, which covers 19 numerical-methods tasks in Python. The tasks were discussed in a group, but this repository is my own individual submission.

#For every task I:

Identified the inputs and the mathematical operation the program performs.
Changed at least one input or parameter and explained how the result changed.
Explained the output in words and interpreted any graph.
Modified the program to solve a different but related real-world case, documenting the new assumptions, input data, output and interpretation.

#2. Repository structure
Folder	Tasks covered
TASK 1-8	Prerequisite, NumPy, vectorization, floating-point errors, matrix algebra, linear systems, LU decomposition, iterative methods
numerical-methods-task-9-12	Eigenvalues, bisection and fixed-point, Newton-Raphson and secant, nonlinear equations
TASK 13-20	Interpolation, curve fitting, differentiation, integration, ODEs, optimization, Monte Carlo

#3. Task overview
Task	Topic	Main tool	Real-world case explored
2	NumPy arrays and numerical computation	numpy	Weather-station / IoT sensor readings
3	Mathematical functions and vectorization	numpy, timeit	Network latency data, loop vs. vectorized speed
4	Floating-point arithmetic and numerical errors	numpy	0.1 + 0.2 comparison, stable vs. unstable formulas
5	Matrix algebra and matrix operations	numpy	2-D graphics rotation and scaling
6	Solution of systems of linear equations	np.linalg.solve	Server CPU and memory usage
7	Gaussian elimination and LU decomposition	scipy.linalg	Repeated solves with one matrix
8	Iterative methods (Jacobi, Gauss-Seidel)	numpy, matplotlib	Steel rod temperature, 200 °C to 25 °C
9	Eigenvalues and eigenvectors	np.linalg.eig	Airport network importance (Nairobi, Mombasa hubs)
10	Root finding: bisection and fixed-point	scipy.optimize	Break-even production quantity
11	Root finding: Newton-Raphson and secant	scipy.optimize	Effective interest rate of a loan
12	Polynomial and nonlinear equations	scipy.optimize.root	Drone flight path vs. radar range
13	Interpolation	scipy.interpolate	Sensor data between measurements
14	Curve fitting and approximation	curve_fit	Server response time vs. load
15	Numerical differentiation	numpy	Speed from GPS position data
16	Numerical integration	scipy.integrate	Energy from smart-meter power readings
17	ODEs: Euler method	numpy	Newton's law of cooling
18	ODEs using SciPy	solve_ivp	RC circuit charging
19	Numerical optimization	minimize	Cloud server cost minimization
20	Random numbers and Monte Carlo	numpy.random	Server overload probability

The real-world cases for Tasks 8 to 12 are my modified versions. For the other tasks the table lists the example from the brief, and my modified case for each is documented in the task's folder.

#4. Key results (Tasks 8 to 12)
Task	Finding
8	Gauss-Seidel needs about half the iterations of Jacobi (75 vs. 150 for the original system). More grid points increase iterations sharply.
9	Dominant eigenvalue 2.5616 for the original network. Adding one link makes all nodes equally important (eigenvalue 3.0).
10	Equilibrium at 27.525 °C. Bisection took 38 iterations, fixed-point 13. In the break-even case, fixed-point only converges near the lower root.
11	IRR is 11.5425%. Newton took 4 iterations, secant 7. The loan example gives a 15.68% nominal and 16.86% effective annual rate.
12	Intersections at (±1.5175, 1.3028). Starting guesses with x = 0 fail because the slope in x is zero there.
5. How to run

Requirements: Python 3.9 or newer (NumPy 2.0 or newer for Task 16, which uses np.trapezoid).

bash
# 1. Clone the repository
git clone https://github.com/WeignstoneC/scientific-computing.git
cd scientific-computing

# 2. (Optional) create a virtual environment
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

# 3. Install the libraries
pip install numpy scipy matplotlib

# 4. Run any script, for example
python "numerical-methods-task-9-12/<script_name>.py"

Scripts that draw graphs open a Matplotlib window. To save a graph instead, replace plt.show() with plt.savefig("name.png", dpi=120).

Libraries used
Library	Purpose
NumPy	Arrays, vectorized maths, linear algebra
SciPy	Root finding, interpolation, curve fitting, integration, ODEs, optimization
Matplotlib	Graphs of convergence, fitted curves and simulation results
timeit	Timing loops against vectorized code
6. Documentation format

Each task's documentation follows the same sections:

B. Inputs and operation: what goes in and what the program computes
C. Parameter change: what I changed and how the result moved
D. Meaning of the output: plain-language explanation and graph interpretation
E. New real-world case: assumptions, input data, output and interpretation
7. Submission
Individual GitHub repository (no group repository used)
Link and documentation uploaded through VLMS
Group discussion for Tasks 2 to 20 completed by Week 10, group project task in Weeks 11 to 13
