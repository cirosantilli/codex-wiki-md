<h1 id="30k/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose $N$ with $T\leq N$. By part (d),

$$
M_T=M_0+\sum_{k=1}^NB_k\xi_k\mathbf1_{\{T\geq k\}}.
$$

Each $B_k\mathbf1_{\{T\geq k\}}$ is $\mathcal F_{k-1}$-measurable. Distinct summands are orthogonal: if $j<k$, conditioning on $\mathcal F_{k-1}$ makes every factor except $\xi_k$ known and $\mathbb E[\xi_k\mid\mathcal F_{k-1}]=0$. The cross terms with $M_0$ vanish in the same way, while $\xi_k^2=1$. Expanding the square therefore gives

$$
\begin{aligned}
\mathbb E[M_T^2]
&=M_0^2+\sum_{k=1}^N\mathbb E[B_k^2\mathbf1_{\{T\geq k\}}]\\
&=\boxed{M_0^2+\mathbb E\left[\sum_{k=1}^TB_k^2\right]}.
\end{aligned}
$$

This is the [stopped martingale isometry in a Rademacher filtration](../../../../../../stopped-martingale-isometry-in-a-rademacher-filtration.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [30K](../../30k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
