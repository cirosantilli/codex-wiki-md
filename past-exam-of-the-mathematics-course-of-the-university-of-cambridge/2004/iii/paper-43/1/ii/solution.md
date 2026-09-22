<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $K=V^{-1}$, the [precision matrix](../../../../../../precision-matrix.md), with $X_1$ scalar and $X_2$ containing all remaining coordinates. Holding $X_2=x_2$ in the [multivariate normal density](../../../../../../multivariate-normal-density.md), the terms involving $x_1$ in its exponent are

$$
-\frac12\left[K_{11}(x_1-\mu_1)^2+2(x_1-\mu_1)K_{12}(x_2-\mu_2)\right].
$$

Completing the square gives a [normal distribution](../../../../../../normal-distribution.md) with mean $\mu_1-K_{11}^{-1}K_{12}(x_2-\mu_2)$ and

$$
\boxed{\operatorname{Var}(X_1\mid X_2=x_2)=\frac1{(V^{-1})_{11}}.}
$$

Equivalently, the block [matrix inverse](../../../../../../matrix-inverse.md) identity gives $K_{11}=(V_{11}-V_{12}V_{22}^{-1}V_{21})^{-1}$. The [Gaussian conditional variance from precision](../../../../../../gaussian-conditional-variance-from-precision.md) is a reciprocal diagonal entry of the [precision matrix](../../../../../../precision-matrix.md), rather than the marginal [variance](../../../../../../variance-split.md) $V_{11}$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
