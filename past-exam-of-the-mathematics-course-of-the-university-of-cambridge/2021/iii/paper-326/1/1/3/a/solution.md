<h1 id="1/1/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Repeated substitution in [Landweber iteration](../../../../../../../../landweber-iteration.md) from $u_0=0$ gives

$$
u_k
=\tau\sum_{j=0}^{k-1}(I-\tau A^*A)^jA^*f.
$$

On the $i$th singular vector, $A^*A$ has [eigenvalue](../../../../../../../../eigenvalue.md) $\sigma_i^2$ and $A^*y_i=\sigma_ix_i$. The finite [geometric series](../../../../../../../../geometric-series.md) therefore gives

$$
\boxed{
u_k=\sum_i
\frac{1-(1-\tau\sigma_i^2)^k}{\sigma_i}
\langle f,y_i\rangle x_i}.
$$

This is a [spectral regularization method](../../../../../../../../spectral-regularization-method.md) with filter

$$
\boxed{g_k(\lambda)=\frac{1-(1-\tau\lambda)^k}{\lambda},
\qquad
u_k=g_k(A^*A)A^*f.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [1](../../../1.md)
4. [1](../../../../1.md)
5. [Paper 326](../../../../../paper-326-split.md)
6. [Iii](../../../../../split.md)
7. [2021](../../../../../../split.md)
8. [Past exam of the mathematics course of the University of Cambridge](../../../../../../../split.md)
9. [Mathematics course of the University of Cambridge](../../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../../split.md)
