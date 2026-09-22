<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a nonzero admissible radial profile define the [radial diffusion Rayleigh quotient](../../../../../radial-diffusion-rayleigh-quotient.md)

$$
\mathcal R[R]=\frac{\int_0^1r\kappa R'^2\,dr}{\int_0^1rR^2\,dr}.
$$

Minimizing the numerator subject to $\int_0^1rR^2\,dr=1$ introduces a multiplier $\nu$. The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) for $r\kappa R'^2-\nu rR^2$ is

$$
(r\kappa R')'+\nu rR=0.
$$

The allowed variations vanish at $r=1$, and the natural condition at the centre is zero radial flux. Thus the minimum, when attained, is the smallest decay [eigenvalue](../../../../../eigenvalue.md) $\nu_0$. Equivalently, expansion in weighted-orthogonal [eigenfunctions](../../../../../eigenfunction.md) makes $\mathcal R[R]$ a weighted average of their decay [eigenvalues](../../../../../eigenvalue.md). The [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) therefore gives

$$
\boxed{\nu_0\leq\mathcal R[R_{\mathrm{trial}}]}.
$$

Admissible trial functions must obey the outer [boundary condition](../../../../../boundary-condition.md), be nonzero and have finite [weighted norm](../../../../../weighted-norm.md) and [energy](../../../../../energy-split.md); they need not solve the differential equation. If the diffusion operator has no lowest [eigenfunction](../../../../../eigenfunction.md), the same variational argument bounds the infimum of its [spectrum](../../../../../spectrum-functional-analysis.md). Existence of a [fundamental diffusion mode](../../../../../fundamental-diffusion-mode.md) is an additional assumption for strongly vanishing diffusivity, not a consequence of the identity alone.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
