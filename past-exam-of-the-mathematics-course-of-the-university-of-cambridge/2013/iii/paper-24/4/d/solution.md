<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix $t$ and put $\sigma=t\wedge\tau$. The [stopping time](../../../../../../stopping-time.md) property implies that $\sigma$ is an $\mathcal F_t$-measurable [random variable](../../../../../../random-variable-split.md) with values in $[0,t]$: for $s<t$,

$$
\{\sigma\leq s\}=\{\tau\leq s\}\in\mathcal F_s\subseteq\mathcal F_t,
$$

and for $s\geq t$ the event is the whole space. By part (c), the restriction of $X$ to $[0,t]\times\Omega$ is $\mathcal B([0,t])\otimes\mathcal F_t$-measurable.

The evaluation map $\omega\mapsto(\sigma(\omega),\omega)$ is measurable from $(\Omega,\mathcal F_t)$ to this product space: the inverse image of a measurable rectangle $A\times C$ is $\{\sigma\in A\}\cap C$. Composing it with the jointly measurable [stochastic process](../../../../../../stochastic-process-split.md) gives an $\mathcal F_t$-measurable [random variable](../../../../../../random-variable-split.md)

$$
X^\tau_t=X_{t\wedge\tau}.
$$

Since this holds for every fixed $t$, **the [stopped process](../../../../../../stopped-process.md) is adapted**. If path regularity holds only [almost surely](../../../../../../almost-sure-convergence.md), first apply the proof to its pathwise regular representative; with a completed filtration, the original stopped variable differs only on a null event and is also $\mathcal F_t$-measurable. The [adaptedness of a stopped right-continuous process](../../../../../../adaptedness-of-a-stopped-right-continuous-process.md) requires neither boundedness of $\tau$ nor a [martingale](../../../../../../martingale-split.md) assumption; $\tau=\infty$ is harmless because $t\wedge\tau\leq t$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
