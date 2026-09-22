# Even-reflection closure for Neumann diffusion

↑ **Parent:** [Finite difference method](finite-difference-method.md)

For the [heat equation](heat-equation.md) with homogeneous [Neumann boundary conditions](neumann-boundary-condition.md) at both ends of a uniform grid, even reflection supplies ghost values for a centered [finite difference method](finite-difference-method.md). A [fourth-order centered second derivative](fourth-order-centered-second-derivative.md) needs two ghost values at each end, obtained with the displayed rule for $j=1,2$. For a sufficiently smooth compatible solution, differentiating the [Neumann boundary conditions](neumann-boundary-condition.md) in time and using the [heat equation](heat-equation.md) makes every odd spatial derivative vanish at the endpoints. Its even extension therefore retains the smoothness required by the fourth-order stencil; arbitrary incompatible initial data need care at the initial boundary corners.

The discrete cosine modes diagonalize this reflected spatial operator, with [eigenvalues](eigenvalue.md) $-4h^{-2}\sin^2(\theta/2)[1+\sin^2(\theta/2)/3]$ and $\theta=j\pi/N$. Its most negative [eigenvalue](eigenvalue.md) is $-16/(3h^2)$, so the [forward Euler method](euler-method.md) is stable in the corresponding trapezoid-weighted norm when $\Delta t/h^2\leq3/8$. The [Crank-Nicolson diffusion scheme](crank-nicolson-diffusion-scheme.md) is stable for every time step for this closure, but its amplification factor approaches $-1$ on highly damped spatial modes, allowing sign-alternating numerical transients. The ghost values are defined here as auxiliary samples outside the physical interval, rather than additional unknown initial data.

## ↑ Ancestors (7)

1. [Finite difference method](finite-difference-method.md)
2. [Finite difference](finite-difference-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2/11/solution.md)
