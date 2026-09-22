<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathcal G_n=\sigma(S_n,S_{n+1},\ldots)$. Since $X_{n+j}=S_{n+j}-S_{n+j-1}$,

$$
\mathcal G_n=\sigma(S_n,X_{n+1},X_{n+2},\ldots).
$$

Permuting $X_1,\ldots,X_n$ preserves their [joint probability distribution](../../../../../../joint-probability-distribution.md) and leaves every generator of $\mathcal G_n$ unchanged. Therefore, for each bounded $\mathcal G_n$-measurable $H$,

$$
\mathbb E[X_1H]=\mathbb E[X_jH]\qquad(1\leq j\leq n).
$$

This is the symmetry of [exchangeable random variables](../../../../../../exchangeable-random-variables.md). By the defining identity of [conditional expectation](../../../../../../conditional-expectation.md), all $\mathbb E[X_j\mid\mathcal G_n]$ are equal [almost surely](../../../../../../almost-sure-convergence.md). Summing these [conditional expectations](../../../../../../conditional-expectation.md) and using that $S_n$ is $\mathcal G_n$-measurable gives

$$
n\mathbb E[X_1\mid\mathcal G_n]=\mathbb E[S_n\mid\mathcal G_n]=S_n.
$$

Hence the [conditional expectation of a summand given future partial sums](../../../../../../conditional-expectation-of-a-summand-given-future-partial-sums.md) is

$$
\boxed{\mathbb E[X_1\mid S_n,S_{n+1},\ldots]=\frac{S_n}{n}\quad\text{almost surely}.}
$$

The [integrability](../../../../../../integrable-random-variable.md) of each $X_j$ justifies every [conditional expectation](../../../../../../conditional-expectation.md) above.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
