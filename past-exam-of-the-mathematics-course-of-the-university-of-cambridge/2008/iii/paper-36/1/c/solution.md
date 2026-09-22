<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At a real point $x$ outside the hull's closure, the [Schwarz reflection principle](../../../../../../schwarz-reflection-principle.md) makes the [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) analytic across the boundary and $g_K'(x)>0$. Use the course's Brownian excursion restriction identity: for an excursion from $x$ to infinity in the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md),

$$
\mathbb P_x^{\rm exc}(\widehat B\cap K=\varnothing)=g_K'(x).
$$

One way to obtain this identity is to start its [Doob h-transform](../../../../../../doob-h-transform.md) at $x+i\varepsilon$: its avoidance probability is $\operatorname{Im}g_K(x+i\varepsilon)/\varepsilon$, which tends to $g_K'(x)$ by reflection. Thus the [boundary derivative is an excursion avoidance probability](../../../../../../boundary-derivative-is-an-excursion-avoidance-probability.md), and in particular it is at most one.

Let $D$ be the filled unit half-disc. Since $K\subseteq D$, avoiding $D$ implies avoiding $K$. The [monotonicity of boundary derivatives of mapping-out functions](../../../../../../monotonicity-of-boundary-derivatives-of-mapping-out-functions.md) and part (b) give, for $|x|>1$,

$$
\boxed{1-x^{-2}=g_D'(x)\leq g_K'(x)\leq1.}
$$

The upper bound is attained by the empty hull and the lower by the filled half-disc, so the comparison is sharp on either real tail.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
