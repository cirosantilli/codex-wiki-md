<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a [stopping time](../../../../../../stopping-time.md) $\tau$, $U_{t\wedge\tau}$ is adapted: split according to $\{\tau=j\}$ for $j<t$ and $\{\tau\geq t\}$, all events belonging to $\mathcal F_t$. It is integrable because $|U_{t\wedge\tau}|\leq\sum_{j=0}^t|U_j|$. Moreover,

$$
U_{(t+1)\wedge\tau}-U_{t\wedge\tau}=\mathbf1_{\{\tau>t\}}(U_{t+1}-U_t).
$$

The indicator is $\mathcal F_t$-measurable, so conditioning and the [supermartingale](../../../../../../supermartingale.md) property give

$$
\mathbb E[U_{(t+1)\wedge\tau}-U_{t\wedge\tau}\mid\mathcal F_t]=\mathbf1_{\{\tau>t\}}(\mathbb E[U_{t+1}\mid\mathcal F_t]-U_t)\leq0.
$$

Thus $\boxed{(U_{t\wedge\tau})_t\text{ is a supermartingale}}$. This proves [stopping preserves supermartingales in discrete time](../../../../../../stopping-preserves-supermartingales-in-discrete-time.md) without assuming $\tau$ itself bounded or integrable.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
