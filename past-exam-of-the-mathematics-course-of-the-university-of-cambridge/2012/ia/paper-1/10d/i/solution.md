<h1 id="10d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $d_j=a_{j+1}-a_j$ and suppose $d_j\to L$. Telescoping gives

$$
\frac{a_n}{n}=\frac{a_1}{n}+\frac1n\sum_{j=1}^{n-1}d_j.
$$

To justify the [Cesaro mean](../../../../../../cesaro-mean.md) limit directly, choose $J$ so that $|d_j-L|<\varepsilon$ for $j\geq J$. The finite initial sum contributes at most $n^{-1}\sum_{j<J}|d_j-L|$, which tends to zero. The remaining terms contribute at most $\varepsilon$, and replacing $(n-1)L/n$ by $L$ contributes $|L|/n$. Consequently **$\boxed{a_n/n\to L}$**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [10D](../../10d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
