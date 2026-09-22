<h1 id="12f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Markov inequality](../../../../../../markov-inequality.md) states that for a nonnegative [random variable](../../../../../../random-variable-split.md) $Z$ and $a>0$,

$$
\mathbb P(Z\geq a)\leq\frac{\mathbb E[Z]}a.
$$

Because $T$ is integer-valued, apply it with $a=1$. With $p=n^{-\alpha}$,

$$
\mathbb P(T>0)=\mathbb P(T\geq1)\leq\binom n3 n^{-3\alpha}\leq\frac16n^{3-3\alpha}\longrightarrow0\quad(\alpha>1).
$$

Therefore

$$
\boxed{\mathbb P(T=0)\longrightarrow1.}
$$

This is the [first moment method](../../../../../../first-moment-method.md): if the expected [triangle count in a binomial random graph](../../../../../../triangle-count-in-a-binomial-random-graph.md) tends to zero, triangles occur with vanishing probability.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
