<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite list of real coefficients $(a_j)_{j\leq m}$,

$$
\sum_{j=1}^m a_j\xi_j=\int_0^1\left(\sum_{j=1}^ma_jg_j(t)\right)\,dW_t.
$$

A deterministic [Itô integral](../../../../../../ito-integral.md) is centered Gaussian: first verify it for step functions as a linear combination of independent Gaussian Brownian increments, then pass to an L2 approximation using the [Itô isometry](../../../../../../ito-isometry.md) and characteristic functions. Its [variance](../../../../../../variance-split.md) is the squared L2 norm of the integrand, which is $\sum_ja_j^2$ by the supplied orthonormality. Therefore

$$
\mathbb E\exp\left(i\sum_{j=1}^ma_j\xi_j\right)=\exp\left(-\frac12\sum_{j=1}^ma_j^2\right)
=\prod_{j=1}^m e^{-a_j^2/2}.
$$

This factors as the joint [characteristic function](../../../../../../characteristic-function.md) of independent standard normals. Since every finite subfamily has this law, **the entire sequence is independent and each $\xi_n$ has law N(0,1)**. This is the [Gaussian coordinates of deterministic orthonormal Wiener integrands](../../../../../../gaussian-coordinates-of-deterministic-orthonormal-wiener-integrands.md) principle.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
