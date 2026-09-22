# Discrete sine transform Poisson solver

↑ **Parent:** [Discrete sine transform](discrete-sine-transform.md)

For $-\Delta u=f$ on a square with homogeneous [Dirichlet boundary conditions](dirichlet-boundary-condition.md), the five-point [finite difference](finite-difference-split.md) operator on a mesh $h=1/N$ is diagonalized by $\sin(\pi ki/N)\sin(\pi\ell j/N)$. Its eigenvalues are $\lambda_{k\ell}=4h^{-2}[\sin^2(\pi k/(2N))+\sin^2(\pi\ell/(2N))]$. A two-dimensional [discrete sine transform](discrete-sine-transform.md), division by these nonzero eigenvalues and the inverse transform give the solution. Odd extension realizes each one-dimensional transform by a [Fast Fourier transform](cooley-tukey-fft-algorithm.md) of length $2N$, making the total cost $O(N^2\log N)$ and storage $O(N^2)$. These finite-difference eigenvalues should not be confused with the continuous spectral eigenvalues $\pi^2(k^2+\ell^2)$.

## ↑ Ancestors (7)

1. [Discrete sine transform](discrete-sine-transform.md)
2. [Discrete Fourier transform](discrete-fourier-transform.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/8/solution.md)
