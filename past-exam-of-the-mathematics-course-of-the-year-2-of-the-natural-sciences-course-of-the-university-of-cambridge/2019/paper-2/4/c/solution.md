<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the simple-contour form of the [residue theorem](../../../../../residue-theorem.md), let $C$ be a positively oriented, simple, closed, piecewise smooth [contour](../../../../../complex-integration-contour.md). Assume $f$ is [holomorphic](../../../../../holomorphic-function-split.md) on a neighbourhood of $C$ and its interior except at finitely many isolated singularities $z_1,\ldots,z_s$, all strictly inside $C$, with none on $C$. Then

$$
\oint_C f(z)\,dz=2\pi i\sum_{j=1}^s\operatorname{Res}_{z=z_j}f.
$$

The more general version weights each [residue](../../../../../residue.md) by the contour's [winding number](../../../../../winding-number.md), with the usual requirement that the contour be homologous to zero in the domain of analyticity containing it and the nonsingular region.

For the requested application, assume $f$ is [holomorphic](../../../../../holomorphic-function-split.md) on a neighbourhood of the contour and its closed interior, and $z_0$ is strictly inside it. Its [Taylor series](../../../../../taylor-series.md) shows

$$
\frac{f(z)}{(z-z_0)^2}
=\frac{f(z_0)}{(z-z_0)^2}+\frac{f'(z_0)}{z-z_0}+O(1).
$$

Only the second term contributes a [residue](../../../../../residue.md). The [residue theorem](../../../../../residue-theorem.md) therefore proves the derivative form of the [Cauchy integral formula](../../../../../cauchy-integral-formula.md):

$$
\boxed{\frac1{2\pi i}\oint_C\frac{f(z)}{(z-z_0)^2}\,dz=f'(z_0)}.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
