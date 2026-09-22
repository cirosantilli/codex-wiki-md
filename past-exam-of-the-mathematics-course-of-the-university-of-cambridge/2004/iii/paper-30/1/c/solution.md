<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each fixed horizon $t$, the stipulated property is the [Class D process](../../../../../../class-d-process.md) condition on $[0,t]$, and imposing it for every finite horizon gives a [Class DL process](../../../../../../class-dl-process.md).

First suppose $M$ is a true [martingale](../../../../../../martingale-split.md). For every [stopping time](../../../../../../stopping-time.md) $T\le t$, the bounded-time [optional sampling theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives

$$
M_T=\mathbb E(M_t\mid\mathcal F_T).
$$

The [conditional expectations](../../../../../../conditional-expectation.md) of one integrable variable form a [uniformly integrable](../../../../../../uniform-integrability.md) family. To see the uniformity explicitly, put $V=\mathbb E(U\mid\mathcal H)$. For any $r,K>0$, conditional Jensen and Markov inequalities give

$$
\mathbb E\bigl[|V|\mathbf1_{\{|V|>K\}}\bigr]
\le\mathbb E\bigl[|U|\mathbf1_{\{|U|>r\}}\bigr]+\frac{r\mathbb E|U|}{K}.
$$

Choose $r$ large and then $K$ large. The bound does not depend on the conditioning [sigma-algebra](../../../../../../sigma-algebra.md). This proves the required [uniform integrability](../../../../../../uniform-integrability.md). Bounded-time optional sampling here can also be justified directly: approximate $T$ from above by finite-grid [stopping times](../../../../../../stopping-time.md), use discrete optional sampling with terminal value $M_t$, and use this same conditional-expectation [uniform integrability](../../../../../../uniform-integrability.md) and right continuity to pass to the limit.

Conversely, take a [localizing sequence](../../../../../../localizing-sequence.md) $\tau_n$ for the [local martingale](../../../../../../local-martingale.md). For fixed $s\le t$, both families $M_{t\wedge\tau_n}$ and $M_{s\wedge\tau_n}$ are [uniformly integrable](../../../../../../uniform-integrability.md), because their times are bounded by $t$. They converge almost surely to $M_t$ and $M_s$, and therefore converge in $L^1$. The stopped [martingale](../../../../../../martingale-split.md) identity

$$
\mathbb E(M_{t\wedge\tau_n}\mid\mathcal F_s)=M_{s\wedge\tau_n}
$$

passes to the limit by $L^1$ contractivity of [conditional expectation](../../../../../../conditional-expectation.md). Thus $\mathbb E(M_t\mid\mathcal F_s)=M_s$, and all time values are integrable. Hence **a [local martingale](../../../../../../local-martingale.md) is a true [martingale](../../../../../../martingale-split.md) exactly when it is of [Class DL](../../../../../../class-dl-process.md)**. This is a finite-horizon criterion, not a claim of [uniform integrability](../../../../../../uniform-integrability.md) over all times simultaneously.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
