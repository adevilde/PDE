# PDE And Finite Element Theory

## Laplace Problem Solver

This repository contains code for solving the Laplace problem in two dimensions using the finite element method with mixed boundary conditions (Dirichlet and Neumann).
The Laplace problem involves finding an approximation of the solution to a problem in a domain equipped with mixed boundary conditions.

## Problem Description

We aim to obtain an approximation of the solution to the Laplace problem in a two-dimensional domain with mixed boundary conditions. The domain, denoted by $\Omega$,
is defined as $]0,1[ \times ]0,1[ \subset \mathbb{R}^2$. Its boundary, $\partial\Omega$, is partitioned into two subsets $\partial\Omega_n$ and 
$\partial\Omega_d$, such that $\partial\Omega_n \cup \partial\Omega_d = \partial\Omega$. The Laplace problem is defined by the following equations:

$$
  \left\{
      \begin{cases}
      -\Delta u(x,y) = f(x,y) & \text{on } \Omega, \\
      u(x,y) = u_d(x,y) & \text{on } \partial \Omega_d, \\
      \frac{\partial u(x,y)}{\partial n} = g(x,y) & \text{on } \partial \Omega_n
      \end{cases}
  \right.
$$

where $f \in L^2(\Omega)$, $u_{d} \in H^1(\Omega)$, and $g \in L^2(\partial \Omega_n)$.

## Methodology

We propose to solve the Laplace problem by discretizing it using the Lagrange finite element method with $P_1$ finite elements, which provide a polynomial 
approximation of the first degree on a triangle.

## Usage

To use the code provided in this repository, follow these steps:
1. Clone the repository to your local machine.
2. Install the necessary dependencies as specified in the `requirements.txt` file.
3. Run the main script to solve the Laplace problem and obtain the solution.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

