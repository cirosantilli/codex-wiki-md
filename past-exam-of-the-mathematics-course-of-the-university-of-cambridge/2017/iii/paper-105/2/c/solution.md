<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Test the [weak formulation](../../../../../../weak-formulation.md) with $u$ itself. Uniform ellipticity and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
\lambda\|\nabla u\|_2^2\le\int_\Omega A\nabla u\cdot\nabla u=-\int_\Omega fu\le\|f\|_2\|u\|_2.
$$

The [Poincaré inequality](../../../../../../poincare-inequality.md) for the bounded shell with zero trace gives $\|u\|_2\le C_P\|\nabla u\|_2$. If the [gradient](../../../../../../gradient.md) is nonzero, divide to obtain $\|\nabla u\|_2\le C_P\lambda^{-1}\|f\|_2$; if it is zero the estimate is immediate and the zero trace forces $u=0$. Thus

$$
\boxed{\|u\|_{H^1(\Omega)}\le C_P\sqrt{1+C_P^2}\,\lambda^{-1}\|f\|_2.}
$$

The constant depends on the shell and $g$, not on $u$ or $f$. Subtracting two solutions with the same forcing gives a zero-forcing solution and hence proves uniqueness. This is a coercive energy argument, not an appeal to [real analytic](../../../../../../real-analytic-function.md) Cauchy solvability.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
