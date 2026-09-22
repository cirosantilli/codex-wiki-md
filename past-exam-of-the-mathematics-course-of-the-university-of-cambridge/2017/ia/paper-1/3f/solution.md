<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Because $(a_n)$ is a [monotone sequence](../../../../../monotone-sequence.md), every one of its first $n$ terms is at most $a_n$, so

$$
s_n\leq a_n.
$$

On the other hand, every term from $a_n$ through $a_{2n}$ is at least $a_n$, and hence

$$
a_n\leq\frac1{n+1}\sum_{k=n}^{2n}a_k
=\frac{2n s_{2n}-(n-1)s_{n-1}}{n+1}.
$$

Both the lower bound and upper bound tend to $x$ because the [Cesaro means](../../../../../cesaro-mean.md) converge to $x$. The [squeeze theorem](../../../../../squeeze-theorem.md) gives

$$
\boxed{a_n\longrightarrow x}.
$$

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
