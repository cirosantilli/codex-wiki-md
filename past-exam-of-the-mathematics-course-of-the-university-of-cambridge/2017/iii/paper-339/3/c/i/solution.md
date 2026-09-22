<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Collect the factor's [coefficients](../../../../../../../coefficient.md) in the column [vector](../../../../../../../vector.md) $q=(q_0,\ldots,q_d)^T$ and set

$$
\boxed{M=qq^*,\qquad M_{ij}=q_i\overline{q_j}}.
$$

This is a [Hermitian matrix](../../../../../../../hermitian-operator.md) and a [positive semidefinite matrix](../../../../../../../positive-semidefinite-matrix.md), because for every complex [vector](../../../../../../../vector.md) $x$,

$$
x^*Mx=|q^*x|^2\geq0.
$$

On the [unit circle](../../../../../../../complex-unit-circle.md), expanding the modulus square gives

$$
|q(z)|^2=\sum_{i,j=0}^d q_i\overline{q_j}z^{i-j}.
$$

Uniqueness of the finite [Laurent polynomial](../../../../../../../laurent-polynomial.md) [coefficients](../../../../../../../coefficient.md), proved as in part (b)(i), therefore gives

$$
\boxed{p_k=\sum_{\substack{0\leq i,j\leq d\\i-j=k}}M_{ij}}.
$$

This is the [rank-one spectral-factor Gram matrix](../../../../../../../rank-one-spectral-factor-gram-matrix.md). The [matrix](../../../../../../../matrix.md) $M$ has [matrix rank](../../../../../../../matrix-rank.md) one when $q\ne0$ and zero when $q=0$. The orientation $i-j=k$ is the PDF's convention: using $\overline{q_i}q_j$ instead would generally interchange $p_k$ and $p_{-k}$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
