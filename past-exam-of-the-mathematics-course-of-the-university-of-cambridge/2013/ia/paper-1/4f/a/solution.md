<h1 id="4f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $s_N=\sum_{n=1}^N(-1)^{n-1}b_n$. Pairing consecutive terms shows $s_{2m}\geq0$ and

$$
s_{2m+2}-s_{2m}=b_{2m+1}-b_{2m+2}\geq0,
\qquad s_{2m+3}-s_{2m+1}=-b_{2m+2}+b_{2m+3}\leq0.
$$

The even [partial sums](../../../../../../partial-sum.md) increase and the odd [partial sums](../../../../../../partial-sum.md) decrease. They satisfy $s_{2m}\leq s_{2m+1}\leq b_1$, while

$$
s_{2m+1}-s_{2m}=b_{2m+1}\longrightarrow0.
$$

Both are [monotone bounded sequences](../../../../../../monotone-bounded-sequence.md) and hence have limits, and the displayed difference makes their limits equal. Every partial sum belongs to one subsequence, so **the alternating series converges**. This is a proof of the [alternating series test](../../../../../../alternating-series-test.md); the monotonicity and zero-limit hypotheses play separate roles.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4F](../../4f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
