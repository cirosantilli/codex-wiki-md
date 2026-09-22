<h1 id="30k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $n<N$,

$$
A_{n+1}-A_n
=V_n-\mathbb E[V_{n+1}\mid\mathcal F_n]\geq0.
$$

The recursion

$$
V_n=\max\{Z_n,\mathbb E[V_{n+1}\mid\mathcal F_n]\}
$$

shows that if $V_n>Z_n$, then $V_n=\mathbb E[V_{n+1}\mid\mathcal F_n]$ and the increment of $A$ is zero. Conversely, if that increment is positive, the maximum must be attained by $Z_n$, so $V_n=Z_n$. The two nonnegative quantities therefore satisfy

$$
\min\{V_n-Z_n,A_{n+1}-A_n\}=0.
$$

For $n=N$, this also holds because $V_N=Z_N$, regardless of the convention $A_{N+1}=\infty$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [30K](../../30k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
