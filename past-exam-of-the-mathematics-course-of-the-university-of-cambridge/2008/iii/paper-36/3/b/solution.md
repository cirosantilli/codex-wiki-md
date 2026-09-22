<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $A=\mathbb H\setminus U$. The neighborhood assumptions at zero and infinity mean that $A$ is a bounded hull away from the starting boundary point. For $t<T$, the conjugacy map $h_t$ is the hydrodynamically normalized [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) of the remaining forbidden hull after removing $K_t$. Its closure avoids the driver, so the [boundary derivative is an excursion avoidance probability](../../../../../../boundary-derivative-is-an-excursion-avoidance-probability.md) yields $0<\Sigma_t\leq1$. Thus $0<M_t\leq1$, and the [bounded local martingale criterion](../../../../../../bounded-local-martingale-criterion.md) makes the localized [martingales](../../../../../../martingale-split.md) uniformly bounded and uniformly integrable.

Choose localization times $\tau_n\uparrow T$, also bounded by $n$. Optional stopping gives $\mathbb E M_{\tau_n}=M_0$. The supplied terminal limit and continuity of the power function give

$$
M_{\tau_n}\longrightarrow\mathbf1_{\{T=\infty\}},\qquad
M_0=\Phi'(0)^{5/8}.
$$

Since these variables are bounded by one, dominated convergence yields

$$
\boxed{\mathbb P(\gamma_t\in U\text{ for all positive times})
=\mathbb P(T=\infty)=\Phi'(0)^{5/8}.}
$$

As usual for a chord starting at zero, the time-zero point is understood as the boundary [prime end](../../../../../../prime-end.md) of $U$; the avoidance assertion concerns the subsequent curve. The boundedness step is what upgrades the [local martingale](../../../../../../local-martingale.md) calculation to an equality of probabilities.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
