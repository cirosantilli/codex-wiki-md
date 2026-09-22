<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Condition first on the count in the [random sum of independent claims](../../../../../random-sum-of-independent-claims.md). For $N=k$, [independence](../../../../../independent-random-variables.md) of the summands and independence from $N$ give

$$
\mathbb E[e^{uS}\mid N=k]=\prod_{j=1}^k\mathbb E[e^{uX_j}]=M_X(u)^k.
$$

The empty product is one when $k=0$. Taking [expected values](../../../../../expected-value.md) proves the [random-sum transform identity](../../../../../random-sum-transform-identity.md):

$$
\boxed{M_S(u)=\sum_{k=0}^{\infty}\mathbb P(N=k)M_X(u)^k=G_N(M_X(u)).}
$$

For positive claim sizes this composition is always finite for $u\le0$, and is an identity of [Laplace transforms of nonnegative random variables](../../../../../laplace-transform-of-a-nonnegative-random-variable.md) after writing $u=-s$. For positive $u$, it holds wherever the composed series is finite; no positive [exponential moment](../../../../../exponential-moment.md) is implied merely by positivity of the summands.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
