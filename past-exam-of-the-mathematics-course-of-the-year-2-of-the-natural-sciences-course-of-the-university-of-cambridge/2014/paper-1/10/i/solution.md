<h1 id="10/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $N[\psi]=\int_a^b(p\psi'^2+q\psi^2)dx$ and $D[\psi]=\int_a^bw\psi^2dx>0$. For a real variation, with $\Lambda=N/D$,

$$
\delta\Lambda=\frac2D\left\{[p\psi'\delta\psi]_a^b+\int_a^b[-(p\psi')'+q\psi-\Lambda w\psi]\delta\psi\,dx\right\}.
$$

Suitable endpoint conditions are homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), homogeneous [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) $p\psi'=0$, or one of each. They remove the variation boundary term and the product $[p\psi\psi']_a^b$. Stationarity for all interior variations is equivalent to

$$
\boxed{-(p\psi')'+q\psi=\Lambda w\psi.}
$$

Conversely, multiplication of an eigenfunction equation by $\psi$ and [integration by parts](../../../../../integration-by-parts.md) gives $N=\lambda D$, hence $\boxed{\Lambda[\psi]=\lambda}$. General Robin data require their boundary-energy contributions unless these endpoint products happen to vanish.

Use an eigenbasis orthonormal with respect to the weight: $\int_a^bw\psi_i^*\psi_jdx=\delta_{ij}$. For complex coefficients use the Hermitian version of the quotient, with absolute squares. Self-adjointness gives

$$
\boxed{\Lambda[\widetilde\psi]=\frac{\sum_{i\geq0}|c_i|^2\lambda_i}{\sum_{i\geq0}|c_i|^2}\geq\lambda_0.}
$$

When $c_0\neq0$, dividing numerator and denominator by $|c_0|^2$ yields

$$
\boxed{\widetilde\lambda=\frac{\lambda_0+\sum_{i\geq1}|a_i|^2\lambda_i}{1+\sum_{i\geq1}|a_i|^2},\qquad a_i=c_i/c_0.}
$$

If $c_0=0$, these ratios are undefined, but the unscaled formula and upper-bound conclusion remain valid. The assumptions are a problem with a [self-adjoint operator](../../../../../self-adjoint-operator.md) bounded below and a complete eigenbasis, with the trial function in its energy-form domain. The [Rayleigh-Ritz method](../../../../../rayleigh-ritz-method.md) minimizes this quotient over an admissible trial family, obtaining an upper bound on $\lambda_0$. Higher eigenfunctions are stationary directions and need not be unrestricted extrema.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
