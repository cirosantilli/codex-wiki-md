<h1 id="18h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expanding the exponent gives

$$
f_\mu(x_1,x_2)
=\frac1{2\pi}e^{-(x_1^2+x_2^2)/2}
e^{\mu(x_1+x_2)-\mu^2}.
$$

The [Fisher-Neyman factorization theorem](../../../../../../fisher-neyman-factorization-theorem.md) therefore shows that $T=X_1+X_2$ is sufficient.

It is also minimal sufficient. For two sample points $x,y\in\mathbb R^2$,

$$
\frac{f_\mu(x)}{f_\mu(y)}
=C(x,y)\exp\left(\mu[T(x)-T(y)]\right),
$$

where $C$ is independent of $\mu$. This ratio is independent of $\mu$ exactly when $T(x)=T(y)$. The [likelihood-ratio criterion for minimal sufficiency](../../../../../../likelihood-ratio-criterion-for-minimal-sufficiency.md) applies, proving the claim and the general [normal sample sum with known variance](../../../../../../normal-sample-sum-with-known-variance.md) result in this case.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18H](../../18h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
