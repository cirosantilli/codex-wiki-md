<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $s_i=\sup_{C_i}f$ and omit empty sets. Since the sets cover the space, boundedness gives

$$
\mathbb E e^{nf(X_n)}\leq\sum_{i=1}^m e^{ns_i}\mathbb P(X_n\in C_i).
$$

For nonnegative numbers $u_{n,i}$, their sum lies between their maximum and m times their maximum. Consequently its scaled logarithmic upper limit is at most $\max_i\limsup_n n^{-1}\log u_{n,i}$; the added $n^{-1}\log m$ vanishes. Each $C_i$ is closed, so the upper bound in the [large deviation principle](../../../../../../large-deviation-principle.md) gives

$$
\boxed{\limsup_n\frac1n\log\mathbb E e^{nf(X_n)}\leq\max_i\left(\sup_{C_i}f-\inf_{C_i}I\right).}
$$

The convention $\log0=-\infty$ also handles sets of zero [probability](../../../../../../probability.md) or infinite [infimum](../../../../../../infimum.md) rate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
