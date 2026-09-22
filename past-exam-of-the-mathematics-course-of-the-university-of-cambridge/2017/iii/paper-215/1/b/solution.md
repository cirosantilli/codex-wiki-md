<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [coupling of probability distributions](../../../../../../coupling.md) is a [joint probability distribution](../../../../../../joint-probability-distribution.md) of [random variables](../../../../../../random-variable-split.md) $(X,Y)$ with the specified [marginal distributions](../../../../../../marginal-distribution.md): $\mathbb P(X\in A)=\mu(A)$ and $\mathbb P(Y\in A)=\nu(A)$. No [independence](../../../../../../independent-random-variables.md) is required.

For every [set](../../../../../../set-split.md) $A$, the difference of the two indicator functions vanishes when $X=Y$. Consequently

$$
|\mu(A)-\nu(A)|=\left|\mathbb E\bigl(\mathbf1_A(X)-\mathbf1_A(Y)\bigr)\right|\leq\mathbb P(X\ne Y).
$$

Maximizing over $A$ gives the [coupling inequality for total variation](../../../../../../coupling-inequality-for-total-variation.md):

$$
\boxed{\|\mu-\nu\|_{\mathrm{TV}}\leq\mathbb P(X\ne Y).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
