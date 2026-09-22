<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) gives an almost-sure limit $M_\infty$, because $|M_n|\leq1$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) also gives $M_n\to M_\infty$ in $L^1$.

To identify the limit, take $A\in\bigcup_n\mathcal F_n$. For some $N$, $A\in\mathcal F_N$, and for every $n\geq N$,

$$
\mathbb E[M_n\mathbf1_A]=\mathbb E[Z\mathbf1_A].
$$

Passing to the $L^1$ limit preserves this equality. The sets for which $\mathbb E[M_\infty\mathbf1_A]=\mathbb E[Z\mathbf1_A]$ form a monotone class containing the algebra $\bigcup_n\mathcal F_n$, so the equality holds throughout $\mathcal F_\infty=\sigma(\bigcup_n\mathcal F_n)$. Since $M_\infty$ is $\mathcal F_\infty$-measurable, it is $\mathbb E[Z\mid\mathcal F_\infty]$. This proves the [conditional-expectation convergence along a filtration](../../../../../../conditional-expectation-convergence-along-a-filtration.md) both almost surely and in $L^1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
