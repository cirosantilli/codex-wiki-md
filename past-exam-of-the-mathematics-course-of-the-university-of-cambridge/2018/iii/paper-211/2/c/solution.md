<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take an increasing [localizing sequence](../../../../../../localizing-sequence.md) $\tau_n$ for $X$ and define the [stopping times](../../../../../../stopping-time.md)

$$
R_n=\inf\{u\geq0:|K_{u+1}|>n\},\qquad T_n=\tau_n\wedge R_n\wedge n.
$$

The [predictable process](../../../../../../predictable-process.md) condition $K_{u+1}\in\mathcal F_u$ makes $R_n$ a [stopping time](../../../../../../stopping-time.md). For each fixed finite time range, the finitely many coefficients $K_1,\ldots,K_t$ are finite [almost surely](../../../../../../almost-sure-convergence.md); hence $T_n\uparrow\infty$ [almost surely](../../../../../../almost-sure-convergence.md).

The stopped [martingale transform](../../../../../../martingale-transform.md) can be written

$$
M_{t\wedge T_n}=\sum_{s=1}^tK_s\mathbf1_{\{R_n\geq s\}}\mathbf1_{\{n\geq s\}}\bigl(X_{s\wedge\tau_n}-X_{(s-1)\wedge\tau_n}\bigr).
$$

Its coefficient is $\mathcal F_{s-1}$-measurable and bounded in absolute value by $n$. Each summand is consequently integrable with zero [conditional expectation](../../../../../../conditional-expectation.md) given $\mathcal F_{s-1}$, since $X^{\tau_n}$ is a true [martingale](../../../../../../martingale-split.md). Thus $M^{T_n}$ is a true [martingale](../../../../../../martingale-split.md) and

$$
\boxed{M=K\mathbin\cdot X\ \text{is a local martingale}.}
$$

The original PDF fixes $M_0=0$; the TeX extraction omits this equality.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
