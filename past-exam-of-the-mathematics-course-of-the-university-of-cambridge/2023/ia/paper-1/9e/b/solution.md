<h1 id="9e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $S_n=\sum_{i\leq n}a_i$ and $T_n=\sum_{i\leq n}|a_i|$. Conditional convergence gives $S_n\to S$ and $T_n\to\infty$. Since $P_n=T_n+S_n$ and $N_n=T_n-S_n$,

$$
\frac{P_n}{N_n}=\frac{1+S_n/T_n}{1-S_n/T_n}\longrightarrow1.
$$

The alternating-series test says that $b_n\downarrow0$ implies convergence of $\sum(-1)^nb_n$. The hypothesis implies $b_n/b_{n+1}>1$ eventually, so $b_n$ is eventually decreasing. For some $c>0$, eventually $b_n/b_{n+1}\geq1+c/n$; the divergent product of these factors forces $b_n\to0$. The test now applies.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9E](../../9e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
