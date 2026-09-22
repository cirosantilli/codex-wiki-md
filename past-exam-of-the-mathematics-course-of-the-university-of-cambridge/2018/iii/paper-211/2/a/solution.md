<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\tau_n\uparrow\infty$ be a [localizing sequence](../../../../../../localizing-sequence.md) for the discrete-time [local martingale](../../../../../../local-martingale.md) $X$. For $t\geq1$, the increment of the stopped [martingale](../../../../../../martingale-split.md) is

$$
X_{t\wedge\tau_n}-X_{(t-1)\wedge\tau_n}=\mathbf1_{\{\tau_n\geq t\}}(X_t-X_{t-1}),
$$

and $\{\tau_n\geq t\}\in\mathcal F_{t-1}$. Thus, for any $A\in\mathcal F_{t-1}$,

$$
\mathbb E[\mathbf1_A\mathbf1_{\{\tau_n\geq t\}}(X_t-X_{t-1})]=0.
$$

The assumed integrability gives the dominating [random variable](../../../../../../random-variable-split.md) $|X_t|+|X_{t-1}|$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) now yields $\mathbb E[\mathbf1_A(X_t-X_{t-1})]=0$, or $\mathbb E[X_t\mid\mathcal F_{t-1}]=X_{t-1}$. Iterating the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) proves **an integrable discrete-time [local martingale](../../../../../../local-martingale.md) is a true [martingale](../../../../../../martingale-split.md).** The proof uses the discrete-time increment indicator; the conclusion does not extend to continuous time.

## ↑ Ancestors (11)

1. [A](../a.md)
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
