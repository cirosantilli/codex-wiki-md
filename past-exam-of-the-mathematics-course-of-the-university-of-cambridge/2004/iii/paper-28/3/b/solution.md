<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $\inf\varnothing=\infty$. Since each $Y_j$ is $\mathcal F_j$-measurable, the event

$$
\{\tau_a\leq n\}=\left\{\sum_{j=1}^nY_j>a\right\}
$$

is in $\mathcal F_n$, so $\tau_a$ is a [stopping time](../../../../../../stopping-time.md). The [stopped predictable budget for adapted increments](../../../../../../stopped-predictable-budget-for-adapted-increments.md) is $A_n=a-U_{n\wedge\tau_a}$, for $n\geq1$.

If $\tau_a=k<\infty$, the sum before the overshooting increment is $U_k=\sum_{j<k}Y_j\leq a$. If $\tau_a>n$, the sum through time $n$ is at most $a$, and in particular $U_n\leq a$. Thus

$$
\boxed{0\leq A_n\leq a.}
$$

The process is adapted, and boundedness gives integrability even when the increments have no finite [expectations](../../../../../../expected-value.md). Directly from the one-step-lagged sum,

$$
U_{(n+1)\wedge\tau_a}-U_{n\wedge\tau_a}
=Y_n\mathbf1_{\{\tau_a>n\}}.
$$

This decrement is $\mathcal F_n$-measurable, and $0\leq Y_n\mathbf1_{\{\tau_a>n\}}\leq a$. Therefore

$$
\mathbb E[A_{n+1}\mid\mathcal F_n]
=A_n-Y_n\mathbf1_{\{\tau_a>n\}}\leq A_n.
$$

Hence $A$ is a nonnegative [supermartingale](../../../../../../supermartingale.md); in fact its paths are nonincreasing. At time zero one may set $U_0=0$ and $A_0=a$; then $A_1=a$ too. Stopping the sum including $Y_{\tau_a}$ would lose nonnegativity, which is why the shifted definition of $U$ matters.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
