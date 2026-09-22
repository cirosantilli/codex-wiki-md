<h1 id="30k/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The reflection map from part (d) bijects paths that hit $a$ and finish below $a$ with paths whose reflected endpoint lies strictly above $a$. Since the reflected walk has the same distribution,

$$
\mathbb P(M_n\geq a)
=\mathbb P(X_n\geq a)+\mathbb P(X_n>a)
=\mathbb P(X_n\geq a)+\mathbb P(X_n\geq a+1).
$$

Subtracting the corresponding identity at level $a+1$ gives

$$
\boxed{\mathbb P(M_n=a)
=\mathbb P(X_n=a)+\mathbb P(X_n=a+1)}.
$$

For a simple symmetric random walk,

$$
\mathbb P(X_n=k)
=2^{-n}\binom{n}{(n+k)/2}
$$

when $|k|\leq n$ and $n+k$ is even, and it is zero otherwise. Therefore the explicit answer is

$$
\boxed{
\mathbb P(M_n=a)
=2^{-n}\left[
\binom{n}{(n+a)/2}
+\binom{n}{(n+a+1)/2}
\right]},
$$

where a binomial coefficient is interpreted as zero when its lower argument is not an integer in $\{0,\ldots,n\}$. This is the [point probability for the maximum of simple symmetric random walk](../../../../../../point-probability-for-the-maximum-of-simple-symmetric-random-walk.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
