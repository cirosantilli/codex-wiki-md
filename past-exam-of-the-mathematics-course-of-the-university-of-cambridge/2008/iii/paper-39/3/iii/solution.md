<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the tree's natural [filtration](../../../../../../filtration-probability-theory.md). The [stopping times](../../../../../../stopping-time.md) take values in the process horizon $\{0,1,2\}$. Construct a dominating [supermartingale](../../../../../../supermartingale.md) $Y$ by backward comparison, the finite-horizon [Snell envelope](../../../../../../snell-envelope.md). At time two put $Y_2=\xi_2$. At time one the continuation values are

$$
\mathbb E[\xi_2\mid\xi_1=11]=\frac23\,13+\frac13\,10=12,\qquad\mathbb E[\xi_2\mid\xi_1=7]=\frac12\,8+\frac12\,4=6.
$$

Compare these with immediate rewards $11$ and $7$ to obtain $Y_1=12$ on the upper branch and $Y_1=7$ on the lower branch. Finally set

$$
Y_0=\max\{8,\mathbb EY_1\}=\max\left\{8,\frac25\,12+\frac35\,7\right\}=9.
$$

These definitions explicitly give $Y_t\geq\xi_t$, $Y_0=\mathbb EY_1$, and $Y_1\geq\mathbb E[Y_2\mid\mathcal F_1]$. Thus $Y$ is a [supermartingale](../../../../../../supermartingale.md). By part (ii), its [stopped process](../../../../../../stopped-process.md) is a [supermartingale](../../../../../../supermartingale.md), so for every allowed $\tau$,

$$
\boxed{\mathbb E\xi_\tau\leq\mathbb EY_\tau=\mathbb EY_{2\wedge\tau}\leq Y_0=9.}
$$

The reward process itself need not be a [supermartingale](../../../../../../supermartingale.md); the constructed majorant is what proves the bound.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
