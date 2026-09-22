<h1 id="30k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The process is adapted to its [natural filtration](../../../../../../natural-filtration.md). At each fixed time it has finite support and is therefore integrable. Conditional on $X_{n-1}=0$,

$$
\mathbb E[X_n\mid X_{n-1}=0]
=\frac1{2n}-\frac1{2n}=0=X_{n-1}.
$$

Conditional on $X_{n-1}\ne0$,

$$
\mathbb E[X_n\mid X_{n-1}]
=\frac1n(nX_{n-1})+\left(1-\frac1n\right)0
=X_{n-1}.
$$

The [Markov property](../../../../../../markov-property.md) now gives

$$
\mathbb E[X_n\mid\mathcal F_{n-1}]
=\mathbb E[X_n\mid X_{n-1}]=X_{n-1},
$$

so $(X_n)$ is a [martingale](../../../../../../martingale-split.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
