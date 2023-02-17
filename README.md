# PINN_Monge_Ampère

The main objective of this repository is to provide a proof of concept of a Physics-Informed Neural Network (PINN) to provide a numerical solution to the Dirichlet problem for the Monge-Ampere elliptic equation in 2D. The exemples discussed here are the first & second tests problems exposed in Alexandre Caboussat, Roland Glowinski and Danny C. Sorensen's paper: A least-squares method for the numerical solution of the dirichlet problem for the elliptic Monge-Ampère equation in dimension two. 2013.

The PDE & Dirichlet Boundary Condition are characterized as follow:
$$det \textbf{D}^2 \psi(x_{1},x_{2}) = f(x_{1},x_{2}), \forall(x_{1},x_{2})\in \Omega = (0,1)^2$$

$$\psi(x_{1},x_{2}) = g(x_{1},x_{2}), \forall(x_{1},x_{2})\in \Gamma$$

<br />

Based on DeepXDE library with Tensorflow backend for the implementation, the PINN architecture is highly inspired by the following papers:

- Maziar Raissi, Paris Perdikaris, and George E Karniadakis. Physics Informed Deep Learning (Part I): Data-driven Solutions of Nonlinear Partial Differential Equations. 2017.

- Jialin Chen. Numerical Methods and Deep Learning Frameworks for Solving Monge-Ampere Equation. 2021. 

- Lu Lu, Xuhui Meng, Zhiping Mao, George Em Karniadakis. DeepXDE: A Deep Learning Library for Solving Differential Equations. 2021
<br />

<img width="545" alt="PINN_architecture" src="https://user-images.githubusercontent.com/101275776/219594515-31a56fa6-84f4-4925-b016-ffa1d8536c69.png">
<br />

The notebooks are structured as follow:

- Set Objective
- Work environnement management
- True solution visualization
- Define PDE, BC, domaine
- Define PINN
- Evaluate PINN
<br />

Several points remain to be confirmed such as:
- Data sampling size impact
- FNN architecture impact
- Activation function impact
- PINN Robustness
- Convergence to local minima
- ...
