<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix $x>0$ and let $A=\{M_0<x\}\in\mathcal F_0$. On $A$, [continuity](../../../../../../continuous-function.md) of the paths implies $0\leq M_{t\wedge T_x}\leq x$, and $M_{T_x}=x$ on $\{T_x<\infty\}$. Bounded-time [optional stopping](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives, for every $t$,

$$
\mathbb E[\mathbf1_A M_{t\wedge T_x}\mid\mathcal F_0]=\mathbf1_A M_0.
$$

On $A\cap\{T_x=\infty\}$, the stopped process is $M_t\to0$; on $A\cap\{T_x<\infty\}$ it eventually equals $x$. The bound by $x$ permits conditional [dominated convergence](../../../../../../dominated-convergence-theorem.md), yielding

$$
x\mathbf1_A\mathbb P(T_x<\infty\mid\mathcal F_0)=\mathbf1_A M_0.
$$

On $A^c$, $T_x=0$, so the conditional hitting probability is one. Finally, a continuous nonnegative path tending to zero attains any positive supremum: after a sufficiently late time it is below half that supremum, and its maximum on the earlier compact interval is attained. Thus $\{M^*\geq x\}=\{T_x<\infty\}$, including equality at the level. We have proved the conditional form of the [maximal identity for a continuous nonnegative local martingale tending to zero](../../../../../../maximal-identity-for-a-continuous-nonnegative-local-martingale-tending-to-zero.md):

$$
\boxed{\mathbb P(M^*\geq x\mid\mathcal F_0)=1\wedge\frac{M_0}{x}.}
$$

The restriction to $A$ before taking the limit is important: $M_0$ need not be bounded, and the unstopped [martingale](../../../../../../martingale-split.md) need not have [uniform integrability](../../../../../../uniform-integrability.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
