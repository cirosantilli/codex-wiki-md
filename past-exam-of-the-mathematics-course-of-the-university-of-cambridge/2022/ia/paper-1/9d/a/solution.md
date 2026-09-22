<h1 id="9d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose $a_n\to L$. Given $\varepsilon>0$, choose $N$ such that $|a_k-L|<\varepsilon/2$ for $k>N$. Then

$$
\left|\frac1n\sum_{k=1}^na_k-L\right|
\leq
\frac1n\sum_{k=1}^N|a_k-L|
+\frac1n\sum_{k=N+1}^n|a_k-L|.
$$

The first term tends to zero because its numerator is fixed, and the second is at most $\varepsilon/2$. Thus the [Cesaro mean](../../../../../../cesaro-mean.md) tends to $L$.

The converse is false. For $a_n=(-1)^n$, the Cesaro means tend to $0$, while the original [sequence](../../../../../../sequence.md) alternates between $-1$ and $1$ and does not converge.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9D](../../9d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
