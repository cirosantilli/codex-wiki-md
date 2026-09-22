<h1 id="9/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Introduce a constant [Lagrange multiplier](../../../../../../lagrange-multiplier.md) $\lambda$ for the fixed [arc length](../../../../../../arc-length.md). Up to an irrelevant constant term, the augmented [functional](../../../../../../functional.md) is

$$
J[y]=\int_{-a}^a(y+\lambda)\sqrt{1+y'^2}\,dx.
$$

It has no explicit $x$ dependence, so the [Beltrami identity](../../../../../../beltrami-identity.md) gives

$$
(y+\lambda)\sqrt{1+y'^2}-\frac{(y+\lambda)y'^2}{\sqrt{1+y'^2}}=\frac{y+\lambda}{\sqrt{1+y'^2}}=k.
$$

For the hanging minimum choose $k>0$. Writing $y_0=-\lambda$, this becomes $1+y'^2=(y-y_0)^2/k^2$. Its nonconstant smooth solution is

$$
\boxed{y(x)-y_0=k\cosh\left(\frac{x-x_0}{k}\right).}
$$

One may verify it without dividing by $y'$ at the lowest point: the full [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) gives $(y+\lambda)y''=1+y'^2$, which the expression satisfies everywhere. The branch with negative $k$ is the inverted stationary chain rather than the hanging minimum. The [catenary minimizes the integral of height along a fixed-length curve](../../../../../../catenary-minimizes-the-integral-of-height-along-a-fixed-length-curve.md), so the positive branch is also the global minimum, not merely a stationary candidate.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
