<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define

$$
\Delta A_t=U_{t-1}-\mathbb E[U_t\mid\mathcal F_{t-1}],
\qquad
\Delta M_t=U_t-\mathbb E[U_t\mid\mathcal F_{t-1}]
$$

for $t\geq1$, with $A_0=M_0=0$. The supermartingale property makes $\Delta A_t\geq0$, and it is $\mathcal F_{t-1}$-measurable, so $A$ is previsible and nondecreasing. The increments of $M$ have conditional mean zero, so $M$ is a martingale. Finally,

$$
\Delta U_t=\Delta M_t-\Delta A_t,
$$

and summation gives the [Doob decomposition in discrete time](../../../../../../doob-decomposition-theorem.md)

$$
\boxed{U_t=U_0+M_t-A_t.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
