<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The [partial fraction decomposition](../../../../../partial-fraction-decomposition.md) is $f(z)=1/(z-i)+1/(z+i)$. Put $w=z-1$ and expand each reciprocal by a [geometric series](../../../../../geometric-series.md):

$$
\frac1{1\mp i+w}=\sum_{n=0}^\infty\frac{(-1)^nw^n}{(1\mp i)^{n+1}},\qquad |w|<\sqrt2.
$$

Adding gives **the [Taylor series](../../../../../taylor-series.md)**

$$
\boxed{f(z)=\sum_{n=0}^\infty(-1)^n\left[(1-i)^{-n-1}+(1+i)^{-n-1}\right](z-1)^n.}
$$

Equivalently, since $1\pm i=\sqrt2e^{\pm i\pi/4}$, its coefficient is $(-1)^n2^{(1-n)/2}\cos((n+1)\pi/4)$. The first terms are $1-\frac12w^2+\frac12w^3-\frac14w^4+\cdots$.

The nearest nonremovable [poles](../../../../../pole.md) are $i$ and $-i$, both at distance $\sqrt2$ from the center. The function is [holomorphic](../../../../../complex-differentiability-at-a-point.md) throughout the open disk of that radius and cannot be [holomorphic](../../../../../complex-differentiability-at-a-point.md) across either pole. Therefore **the largest [radius of convergence](../../../../../radius-of-convergence.md) is $r=\sqrt2$**.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
