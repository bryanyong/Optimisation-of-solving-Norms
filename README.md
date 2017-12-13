# Optimisation-of-solving-Norms
4th year module in Practical Optimisation coursework for Cambridge University Engineering Department

This code was for coursework on a 4th year module on practical optimisation. In particular, it dicusses the different approaches of tackling unconstrained optimisation problems. The objective is to approximate solutions to norms using three different approaches (Gradient Descent, Conjugate Gradient and Newton). It discusses the effects of parameters of the theory by considering the efficiency (iterations and speed). It analayses the depence on epsilon on the convergence rate. Finally, it considers a heuristic approach to an optimisation problem with an additional constraint of sparsity. All the code provided in this document is written solely by me, by considering how the unconstrained problem can be described as a summation of Matrix algebra. 

# Code
Functions

F1 is the objective function of a basic unconstrained optimisation problem.
F2 is the same objective function, except evaluated at X+alpha * dk, ie. after considering the search direction.
F3 is the objective function in F1 but with the additional consideration of a small error epsilon.
F4 is the objective function F3, except evaluated at X+alpha * dk.
dk1 is the gradient of the function
dk2 is the gradient of the function, including the small error epsilon
H1 is the Hessian, used for the Newton method

Lab Sections
1C uses Matlab's built in linprog to compute the L1, L2 and L-inf norms. This is to compare true solutions and to discuss the spread of errors and computational times.

2B is the code for finding the optimal solution using Gradient Descent method.
2C is the code for finding the optimal solution using Conjugate Gradient method.
2D is the code for finding the optimal solution using Newton method.
Part 3 is the code for solving the problem with an added constraint of sparsity.
