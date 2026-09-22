<h1 id="s31/2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $r=\Delta\tau/h^2$ and impose periodic indices modulo $J$. With $\boldsymbol\Phi^n=(\Phi_0^n,\ldots,\Phi_{J-1}^n)^T$, the [linear system](../../../../../system-of-linear-equations.md) is

$$
\boxed{A\boldsymbol\Phi^{n+1}=\boldsymbol\Phi^n-4\pi G\Delta\tau\boldsymbol\rho,\quad
A=(1+2r)I-r(S+S^{-1}),}
$$

where $S$ shifts one grid cell cyclically. For $J\ge3$, $A$ has diagonal $1+2r$, adjacent and corner entries $-r$, and all other entries zero. It is a cyclic tridiagonal [matrix](../../../../../matrix.md), rather than a nonperiodic tridiagonal one.

The periodic Laplacian annihilates the constant [vector](../../../../../vector.md), so its steady equation requires $\boxed{\sum_j\rho_j=0}$. A strictly positive gravitational [density](../../../../../density.md) violates this condition: summing the update gives $\bar\Phi^{n+1}=\bar\Phi^n-4\pi G\Delta\tau\bar\rho$, an indefinitely drifting mean. Periodic gravitational calculations normally solve for $\rho-\bar\rho$ and fix the arbitrary mean [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md). The per-step [matrix](../../../../../matrix.md) $A$ itself remains invertible; the issue is existence of a periodic steady solution of [Poisson's equation](../../../../../poisson-s-equation.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [S31](../../../s31.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
