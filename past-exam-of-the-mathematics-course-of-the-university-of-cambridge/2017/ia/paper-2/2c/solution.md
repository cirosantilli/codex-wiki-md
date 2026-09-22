<h1 id="2c/solution">Solution</h1>

↑ **Parent:** [2C](../2c.md)

The first [partial derivatives](../../../../../partial-derivative.md) are

$$
f_x=\frac1y-\frac{y}{x^2}-\frac{2(x-y)}{a^2},\qquad
f_y=\frac1x-\frac{x}{y^2}+\frac{2(x-y)}{a^2}.
$$

Both vanish at $(\lambda,\lambda)$, so every positive diagonal point is a [stationary point](../../../../../stationary-point.md). The [Hessian matrix](../../../../../hessian-matrix.md) there is

$$
\boxed{H=2\left(\frac1{\lambda^2}-\frac1{a^2}\right)
\begin{pmatrix}1&-1\\-1&1\end{pmatrix}.}
$$

Its [eigenvectors](../../../../../eigenvector.md) $(1,1)$ and $(1,-1)$ have respective [eigenvalues](../../../../../eigenvalue.md)

$$
\boxed{0,\qquad4\left(\frac1{\lambda^2}-\frac1{a^2}\right).}
$$

The zero [eigenvalue](../../../../../eigenvalue.md) reflects the entire line of [nonisolated stationary points](../../../../../nonisolated-stationary-point.md): $f(\lambda,\lambda)=2$. In fact $f-2=(x-y)^2[1/(xy)-1/a^2]$, showing a non-strict [local minimum](../../../../../local-minimum.md) when $\lambda<|a|$, a non-strict [local maximum](../../../../../local-maximum.md) when $\lambda>|a|$, and values on both sides of two near $\lambda=|a|$. At that last point the whole [Hessian matrix](../../../../../hessian-matrix.md) vanishes, so its signs alone cannot classify the point.

## ↑ Ancestors (10)

1. [2C](../2c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
