<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On the Euclidean [unit ball](../../../../../../unit-ball.md) $D^n$,

$$
\omega_X=dx^1\wedge\cdots\wedge dx^n.
$$

The outward [unit normal](../../../../../../unit-normal.md) along $S^{n-1}$ is the radial vector field $N=\sum_i x^i\partial_i$, so part b gives

$$
\omega_{\partial X}
=\sum_{i=1}^n(-1)^{i-1}x^i\,dx^1\wedge\cdots\wedge\widehat{dx^i}\wedge\cdots\wedge dx^n.
$$

Let $R=\sum_i x^i\partial_i$ on the ball and put $\beta=\iota_R\omega_X$. Direct use of the [exterior derivative](../../../../../../exterior-derivative.md) gives $d\beta=n\omega_X$. Therefore the [Generalized Stokes theorem](../../../../../../generalized-stokes-theorem.md) yields

$$
\int_{\partial X}\omega_{\partial X}
=\int_{\partial X}F^*\beta
=\int_Xd\beta
=n\int_X\omega_X.
$$

This proves the [volume of a Euclidean unit sphere](../../../../../../volume-of-a-euclidean-unit-sphere.md) formula.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
