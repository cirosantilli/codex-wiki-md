<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

At the origin, the [Taylor series](../../../../../taylor-series.md) $\sin z=z+O(z^3)$ and $1-\cos z=z^2/2+O(z^4)$ give

$$
f_1(z)=z^{-3}(1+O(z)),\qquad f_2(z)=2z^{-4}(1+O(z^2)).
$$

Thus **$f_1$ has a pole of order three and $f_2$ a pole of order four at zero**. For the third function, the [Laurent series](../../../../../laurent-series.md)

$$
f_3(z)=\sum_{k=0}^{\infty}\frac{(-1)^k z^{1-2k}}{(2k+1)!}
$$

has infinitely many nonzero negative-power terms, so **zero is an essential singularity of $f_3$**.

To classify the point at infinity on the [Riemann sphere](../../../../../riemann-sphere.md), use the coordinate $w=1/z$. Then

$$
f_3(1/w)=w^{-2}\sin w=w^{-1}-\frac w6+O(w^3),
$$

so **$f_3$ has a simple pole at infinity**.

For the other two functions, an important qualification is necessary. The [poles](../../../../../pole.md) of $f_1$ at nonzero integer multiples of $\pi$, and those of $f_2$ at nonzero integer multiples of $2\pi$, approach infinity. Equivalently, their images in the $w$ coordinate accumulate at zero. Hence **infinity is a non-isolated singularity of $f_1$ and $f_2$**. Neither function is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on any punctured neighbourhood of infinity, so the [classification of isolated singularities](../../../../../classification-of-isolated-singularities.md) into removable singularities, poles and essential singularities does not apply there.

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
