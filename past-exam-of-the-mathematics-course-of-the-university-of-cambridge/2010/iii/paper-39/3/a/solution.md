<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Backward induction first proves that the [Snell envelope](../../../../../../snell-envelope.md) is [adapted](../../../../../../adapted-process.md) and [integrable](../../../../../../integrability.md). At each step, $|U_t|\leq|Y_t|+\mathbb E[|U_{t+1}|\mid\mathcal F_t]$, so integrability follows from that of $Y_t$ and $U_{t+1}$. Its defining maximum immediately gives

$$
\mathbb E[U_{t+1}\mid\mathcal F_t]\leq U_t,
$$

which proves that **$U$ is a supermartingale**.

If $Y$ is a [submartingale](../../../../../../submartingale.md), the sharper backward identity is

$$
\boxed{U_t=\mathbb E[Y_T\mid\mathcal F_t].}
$$

It holds at $T$. If it holds at $t+1$, the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives $\mathbb E[U_{t+1}\mid\mathcal F_t]=\mathbb E[Y_T\mid\mathcal F_t]$. Iterating the submartingale inequalities shows that this is at least $Y_t$, so the maximum chooses this continuation value. The displayed identity then makes $U$ a [martingale](../../../../../../martingale-split.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
