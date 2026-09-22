<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the first entry into the stopping region:

$$
\tau^*=\inf\{t\leq T:U_t=Z_t\}.
$$

This set is nonempty because $U_T=Z_T$. Before $\tau^*$, the recursion has

$$
U_t=\mathbb E[U_{t+1}\mid\mathcal F_t],
$$

so the stopped process $U_{t\wedge\tau^*}$ is a martingale. Optional sampling and $U_{\tau^*}=Z_{\tau^*}$ give

$$
U_0=\mathbb E U_{\tau^*}=\mathbb E Z_{\tau^*}.
$$

**Thus $\tau^*$ is an [optimal stopping time](../../../../../../optimal-stopping-time.md).**

## ↑ Ancestors (11)

1. [C](../c.md)
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
