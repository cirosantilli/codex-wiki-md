<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $M(x)=\sum_{n\leq x}\mu(n)$ for the [Mertens function](../../../../../../mertens-function.md). Suppose, to the contrary, that for some $\varepsilon>0$ the quotient $|M(x)|/x^{1/2-\varepsilon}$ were bounded. [Partial summation](../../../../../../abel-s-summation-formula.md) would then make

$$
\sum_{n=1}^{\infty}\frac{\mu(n)}{n^s}
=s\int_1^\infty M(x)x^{-s-1}\,dx
$$

converge and define a [holomorphic function](../../../../../../holomorphic-function.md) throughout $\Re s>1/2-\varepsilon$. In $\Re s>1$ the [Euler product](../../../../../../euler-product.md) identifies this function with $1/\zeta(s)$, so [analytic continuation](../../../../../../analytic-continuation.md) would make $1/\zeta(s)$ holomorphic in that larger half-plane.

By assumption, $\zeta$ has a [nontrivial zero](../../../../../../nontrivial-zero-of-the-riemann-zeta-function.md). The [functional equation of the Riemann zeta function](../../../../../../functional-equation-of-the-riemann-zeta-function.md) reflects one of that zero and its partner into $\Re s\geq1/2$, where $1/\zeta$ must have a pole, a contradiction. Thus $|M(x)|/x^{1/2-\varepsilon}$ is unbounded, which gives an $x\geq1$ exceeding any prescribed constant $C$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
