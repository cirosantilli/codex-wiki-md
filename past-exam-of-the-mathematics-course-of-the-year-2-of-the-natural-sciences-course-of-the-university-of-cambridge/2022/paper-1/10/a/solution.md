<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) $\psi(a)=\psi(b)=0$, and take a nonzero real admissible trial $\psi$. Write the numerator as $F[\psi]$ and denominator as $G[\psi]>0$. For an endpoint-zero [variation](../../../../../variation.md) $\eta$, [integration by parts](../../../../../integration-by-parts.md) gives

$$
\delta F=2\int_a^b[p\psi'\eta'+q\psi\eta]dx=2\int_a^b[-(p\psi')'+q\psi]\eta\,dx,\qquad\delta G=2\int_a^bw\psi\eta\,dx.
$$

Thus the [first variation](../../../../../first-variation.md) of the [Rayleigh quotient](../../../../../rayleigh-quotient.md) is

$$
\delta\Lambda=\frac2G\int_a^b[-(p\psi')'+q\psi-\Lambda[\psi]w\psi]\eta\,dx.
$$

By the [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md), stationarity is equivalent to

$$
\boxed{-(p\psi')'+q\psi=\lambda w\psi,\qquad\lambda=\Lambda[\psi],\qquad\psi(a)=\psi(b)=0.}
$$

Conversely, multiplying an [eigenfunction](../../../../../eigenfunction.md) equation by $\psi$ and integrating gives $F=\lambda G$, so its [first variation](../../../../../first-variation.md) vanishes. This establishes the equivalence for the chosen [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md). Homogeneous [Neumann boundary conditions](../../../../../neumann-boundary-condition.md), or a mixed Dirichlet-Neumann pair, also cancel the boundary term; general [Robin boundary conditions](../../../../../robin-boundary-condition.md) require adding the corresponding boundary contribution to the numerator.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
