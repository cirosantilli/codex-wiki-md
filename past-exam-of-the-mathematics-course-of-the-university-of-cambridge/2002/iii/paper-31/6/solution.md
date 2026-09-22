<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Here is a finite-horizon [Girsanov theorem](../../../../../girsanov-theorem.md) statement with the sign fixed explicitly. Let $B$ be a [Brownian motion](../../../../../brownian-motion-split.md) under $P$, and let $\theta$ be [predictable](../../../../../predictable-process.md) with $\int_0^T\theta_s^2ds<\infty$ almost surely. If

$$
L_t=\exp\!\left(\int_0^t\theta_s dB_s-\frac12\int_0^t\theta_s^2ds\right),\qquad 0\le t\le T,
$$

is a true [martingale](../../../../../martingale-split.md) with $\mathbb EL_T=1$, then the measure $Q$ defined by $dQ=L_TdP$ makes $B_t-\int_0^t\theta_sds$ a [Brownian motion](../../../../../brownian-motion-split.md) up to $T$. The sufficient [Novikov condition](../../../../../novikov-s-condition.md) is $\mathbb E\exp(\tfrac12\int_0^T\theta_s^2ds)<\infty$. Merely being a [local martingale](../../../../../local-martingale.md) is not a sufficient density condition.

For a deterministic [absolutely continuous function](../../../../../absolutely-continuous-function.md) $h$ with $h(0)=0$ and [derivative](../../../../../derivative.md) $g\in L^2[0,T]$, take $\theta=g$. [Novikov's condition](../../../../../novikov-s-condition.md) holds because its exponential is deterministic and finite. Under $Q$, the canonical process has the law of a [Brownian motion](../../../../../brownian-motion-split.md) plus $h$. Thus for every bounded measurable path functional $F$,

$$
\boxed{\mathbb E F(B+h)=\mathbb E\left[F(B)\exp\!\left(\int_0^Tg_s dB_s-\frac12\int_0^Tg_s^2ds\right)\right].}
$$

This derives the [Cameron-Martin theorem](../../../../../cameron-martin-theorem.md) density formula from the [Girsanov theorem](../../../../../girsanov-theorem.md), rather than assuming the two measures have the same drift convention. Replacing $h$ by $-h$ changes the sign of the [stochastic integral](../../../../../stochastic-integral.md).

The question's path space is the whole half-line, not just one finite horizon. When $g\in L^2(0,\infty)$, the density [martingale](../../../../../martingale-split.md) satisfies

$$
\mathbb EL_t^2=\exp\!\left(\int_0^tg_s^2ds\right)\le e^{\|g\|_2^2}.
$$

It has a [uniformly integrable](../../../../../uniform-integrability.md) limit $L_\infty=\exp(\int_0^\infty g_s dB_s-\|g\|_2^2/2)$ of mean one, strictly positive almost surely. Integrals here converge in $L^2$ and almost surely. The finite-time identities then identify $L_\infty$ as the density on the full path [sigma-algebra](../../../../../sigma-algebra.md), since finite-time cylinder events generate it. This is [Cameron-Martin shifts on infinite Wiener path space](../../../../../cameron-martin-shifts-on-infinite-wiener-path-space.md). Finite-horizon [absolute continuity of measures](../../../../../absolute-continuity-of-measures.md) alone does not imply infinite-horizon [absolute continuity of measures](../../../../../absolute-continuity-of-measures.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
