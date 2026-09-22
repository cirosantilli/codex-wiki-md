<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

The [Cauchy integral formula](../../../../../cauchy-integral-formula.md) states that if $f$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on a neighbourhood of a simple closed positively oriented contour and its interior, then, for an interior point $z$,

$$
f(z)=\frac1{2\pi i}\oint\frac{f(\xi)}{\xi-z}\,d\xi.
$$

Fix $0<r<1$ and apply it on $|\xi|=r$. For $|z|<r$, the [geometric series](../../../../../geometric-series.md)

$$
\frac1{\xi-z}=\sum_{n=0}^{\infty}\frac{z^n}{\xi^{n+1}}
$$

converges uniformly in $\xi$ and locally uniformly in $z$. Indeed, for $|z|\leq s<r$ its absolute terms are bounded by $s^n/r^{n+1}$. Since $f$ is bounded on the contour, termwise [contour integration](../../../../../contour-integration.md) is valid, giving

$$
f(z)=\sum_{n=0}^{\infty}c_nz^n,\qquad
c_n=\frac1{2\pi i}\oint_{|\xi|=r}\frac{f(\xi)}{\xi^{n+1}}\,d\xi.
$$

Termwise differentiation of this locally convergent [power series](../../../../../power-series.md) gives $f^{(n)}(0)=n!c_n$. Therefore

$$
\boxed{f^{(n)}(0)=\frac{n!}{2\pi i}\oint_{|\xi|=r}\frac{f(\xi)}{\xi^{n+1}}\,d\xi\quad(n\geq0)}.
$$

This also derives the needed [Taylor series](../../../../../taylor-series.md) representation rather than assuming an unjustified interchange at the boundary of the analytic disk.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
