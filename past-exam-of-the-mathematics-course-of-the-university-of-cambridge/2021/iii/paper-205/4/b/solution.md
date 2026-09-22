<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [kernel ridge regression](../../../../../../kernel-ridge-regression.md) estimator minimizes

$$
\sum_{i=1}^n\{y_i-f(x_i)\}^2+\lambda\lVert f\rVert_{\mathcal H}^2.
$$

By the [representer theorem](../../../../../../representer-theorem.md), its fitted-value vector is

$$
\widehat f=K(K+\lambda I)^{-1}y.
$$

Writing $f$ for the true value vector, the variance contribution to $\mathbb E\lVert f-\widehat f\rVert_2^2$ is

$$
\sigma^2\operatorname{tr}\{K^2(K+\lambda I)^{-2}\}
=\sigma^2\sum_{i=1}^n\frac{d_i^2}{(d_i+\lambda)^2}.
$$

The squared bias is $\lVert\lambda(K+\lambda I)^{-1}f\rVert_2^2$. In an orthonormal eigenbasis of $K$, the scalar inequality

$$
\frac{\lambda^2}{(d+\lambda)^2}\leq\frac{\lambda}{4d},
$$

which is equivalent to $4d\lambda\leq(d+\lambda)^2$, yields

$$
\boxed{
\mathbb E\sum_{i=1}^n\{f^0(x_i)-\widehat f_\lambda(x_i)\}^2
\leq\sigma^2\sum_{i=1}^n\frac{d_i^2}{(d_i+\lambda)^2}
+\frac\lambda4f^TK^{-1}f}.
$$

For $\lVert f\rVert_2=1$, only the last term varies. The [Rayleigh quotient](../../../../../../rayleigh-quotient.md) of $K^{-1}$ is maximized by a unit eigenvector associated with its largest eigenvalue $1/d_n$, equivalently an eigenvector of $K$ associated with $d_n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
