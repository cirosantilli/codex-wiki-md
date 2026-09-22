<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [kernel ridge regression](../../../../../../kernel-ridge-regression.md) estimator is

$$
\widehat f_\lambda
=\underset{f\in\mathcal H}{\operatorname{argmin}}
\left\{\frac1n\sum_{i=1}^n(Y_i-f(x_i))^2+\lambda\lVert f\rVert_{\mathcal H}^2\right\}.
$$

By the [representer theorem](../../../../../../representer-theorem.md), $\widehat f_\lambda=\sum_{j=1}^n\alpha_jk(x_j,\cdot)$. If $K_{ij}=k(x_i,x_j)$, substitution and differentiation give

$$
(K+n\lambda I)\alpha=Y.
$$

Thus

$$
\alpha=(K+n\lambda I)^{-1}Y,
\qquad
\widehat Y=H_\lambda Y,
\qquad
H_\lambda=K(K+n\lambda I)^{-1}.
$$

The matrix $H_\lambda$ is the [kernel-ridge hat matrix](../../../../../../kernel-ridge-hat-matrix.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
