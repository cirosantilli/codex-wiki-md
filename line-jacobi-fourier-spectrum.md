# Line-Jacobi Fourier spectrum

↑ **Parent:** [Matrix splitting](matrix-splitting.md)

For the five-point Dirichlet Laplacian on an $n\times n$ square grid, a block-Jacobi splitting that solves each horizontal line exactly has blocks $\operatorname{tridiag}(-1,4,-1)$. Its tensor-product sine modes have angles $\theta_r=r\pi/(n+1)$ and the displayed [iteration matrix](iteration-matrix.md) eigenvalues. With $c=\cos(\pi/(n+1))$, its [spectral radius](spectral-radius.md) is $c/(2-c)<1$, so it converges on every fixed grid. However the mode $r=1,s=n$ has multiplier $-c/(2-c)\to-1$. It is highly oscillatory between lines and is barely damped. The undamped method is therefore not a uniformly effective smoother for the [multigrid method](multigrid-method-split.md), even though it converges. Convergence and smoothing test different properties of the error spectrum.

## ↑ Ancestors (8)

1. [Matrix splitting](matrix-splitting.md)
2. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford/2008/2/c/solution.md)
