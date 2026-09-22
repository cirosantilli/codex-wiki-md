<h1 id="12f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By [Tonelli theorem](../../../../../../tonelli-theorem.md) for the nonnegative indicators,

$$
\mathbb E[N]
=\mathbb E\left[\sum_{n\geq1}\mathbf1_{A_n}\right]
=\sum_{n\geq1}\mathbb P(A_n).
$$

If this is finite, then $N$ is finite almost surely: alternatively, [Markov inequality](../../../../../../markov-inequality.md) gives

$$
\mathbb P(N\geq m)\leq\frac{\mathbb E[N]}m\longrightarrow0.
$$

Since $\{N=\infty\}\subseteq\{N\geq m\}$ for every $m$,

$$
\boxed{\mathbb P(N=\infty)=0}.
$$

This is the first [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
