<h1 id="30k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The process $M$ is adapted and integrable. Since $A_{n+1}$ is $\mathcal F_n$-measurable,

$$
\begin{aligned}
\mathbb E[M_{n+1}\mid\mathcal F_n]
&=\mathbb E[V_{n+1}\mid\mathcal F_n]+A_{n+1}\\
&=\mathbb E[V_{n+1}\mid\mathcal F_n]+A_n
+V_n-\mathbb E[V_{n+1}\mid\mathcal F_n]\\
&=V_n+A_n=M_n.
\end{aligned}
$$

**Thus $M$ is a martingale. This is the finite-horizon Doob decomposition $V=M-A$.**

## ↑ Ancestors (11)

1. [C](../c.md)
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
