<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A qualification is necessary: **an arbitrary symbolic Gibbs measure does not satisfy the claim**. Consider the doubling map with its two binary branches and a Bernoulli symbolic [Gibbs measure](../../../../../../gibbs-measure.md) with probabilities $2/3$ and $1/3$. This is the Gibbs law for a locally constant [symbolic potential](../../../../../../symbolic-potential.md), while every level-$n$ interval has length $2^{-n}$. Along the nonboundary alternating itinerary, for even $n$,

$$
g_n=\log\frac{(2/3)^{n/2}(1/3)^{n/2}}{2^{-n}}
=\frac n2\log(8/9)\longrightarrow-\infty.
$$

No finite $g$ can approximate these $g_n$ with a decaying uniform error. This proves the reusable fact that [an arbitrary Gibbs measure need not be absolutely continuous](../../../../../../an-arbitrary-gibbs-measure-need-not-be-absolutely-continuous.md).

For the intended geometric version, take the [Gibbs measure](../../../../../../gibbs-measure.md) for the [geometric potential of an expanding map](../../../../../../geometric-potential-of-an-expanding-map.md) $-\log|T'|$, with the standard sufficiently smooth finite full-branch hypotheses. The allowed transfer-operator result supplies a strictly positive [Lipschitz continuous](../../../../../../lipschitz-continuity.md) invariant [probability density function](../../../../../../probability-density-function.md) $h$, normalized by $\int h=1$, and its symbolic weights of [cylinder sets](../../../../../../cylinder-set.md) are $\nu(C_w)=\int_{\Delta_w}h(x)\,dx$. State the needed regularity explicitly: $h\geq h_*>0$ and $|h(x)-h(y)|\leq L_h|x-y|$. Expansion gives $\operatorname{diam}\Delta_w\leq\lambda^{-n}$.

Let $\pi(\epsilon)$ denote the point coded by the infinite sequence, and define $g(\epsilon)=\log h(\pi(\epsilon))$. The expression defining $g_n$ is the logarithm of the average of $h$ over the cylinder. For $x=\pi(\epsilon)\in\Delta_w$,

$$
\left|\frac1{|\Delta_w|}\int_{\Delta_w}h(y)\,dy-h(x)\right|\leq L_h\lambda^{-n}.
$$

Since the [logarithm](../../../../../../logarithm.md) is [Lipschitz continuous](../../../../../../lipschitz-continuity.md) with constant $1/h_*$ on this positive range, the [cylinder averages of an invariant density](../../../../../../cylinder-averages-of-an-invariant-density.md) give

$$
\boxed{|g(\epsilon)-g_n(\epsilon_1,\ldots,\epsilon_n)|\leq\frac{L_h}{h_*}\lambda^{-n}.}
$$

This proves the intended estimate. Expansion alone and an unspecified Gibbs [symbolic potential](../../../../../../symbolic-potential.md) are insufficient; the geometric choice and the regularity producing a positive [Lipschitz continuous](../../../../../../lipschitz-continuity.md) [probability density function](../../../../../../probability-density-function.md) are substantive hypotheses.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
