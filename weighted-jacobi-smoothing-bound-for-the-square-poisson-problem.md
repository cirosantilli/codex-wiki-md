# Weighted Jacobi smoothing bound for the square Poisson problem

↑ **Parent:** [Weighted Jacobi eigenvalues for a square Dirichlet grid](weighted-jacobi-eigenvalues-for-a-square-dirichlet-grid.md)

For the five-point Dirichlet Poisson matrix, [weighted Jacobi iteration](weighted-jacobi-method.md) has sine-mode multiplier $1-\omega+(\omega/2)(\cos\theta_r+\cos\theta_s)$. Call a mode high-frequency if at least one cosine is nonpositive. Then the sum lies in $[-2,1]$, so for $\omega=4/5$ the multiplier lies in $[-3/5,3/5]$. This uniform damping makes the iteration a useful smoother for a [multigrid method](multigrid-method-split.md), even though low-frequency multipliers approach one on fine grids. Balancing $|1-2\omega|$ and $|1-\omega/2|$ shows why $4/5$ is the minimax parameter for this high-frequency interval. The two-dimensional high-frequency set gives a different optimum from the familiar one-dimensional value $2/3$.

## ↑ Ancestors (10)

1. [Weighted Jacobi eigenvalues for a square Dirichlet grid](weighted-jacobi-eigenvalues-for-a-square-dirichlet-grid.md)
2. [Weighted Jacobi method](weighted-jacobi-method.md)
3. [Jacobi method](jacobi-method.md)
4. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
5. [Numerical linear algebra](numerical-linear-algebra-split.md)
6. [Numerical analysis](numerical-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/a/3/b/solution.md)
