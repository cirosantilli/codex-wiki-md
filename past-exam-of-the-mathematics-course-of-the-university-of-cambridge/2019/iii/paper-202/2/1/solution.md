<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\Delta_iM=M_{t_i}-M_{t_{i-1}}$ and $Q=\sum_i(\Delta_iM)^2$. The identity

$$
Q=M_t^2-M_0^2-2\sum_iM_{t_{i-1}}\Delta_iM
$$

shows, using the [martingale-difference orthogonality](../../../../../../martingale-difference-orthogonality.md), that

$$
\begin{aligned}
\mathbb E[Q^2]
&\leq2\mathbb E[(M_t^2-M_0^2)^2]
 +8\mathbb E\left[\left(\sum_iM_{t_{i-1}}\Delta_iM\right)^2\right]\\
&\leq2C^4+8C^2\mathbb E[Q].
\end{aligned}
$$

Also $\mathbb E[Q]=\mathbb E[M_t^2]-\mathbb E[M_0^2]\leq C^2$. Hence $\mathbb E[Q^2]\leq10C^4$, which in particular proves the requested bound

$$
\boxed{\mathbb E[Q^2]\leq48C^4.}
$$

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
