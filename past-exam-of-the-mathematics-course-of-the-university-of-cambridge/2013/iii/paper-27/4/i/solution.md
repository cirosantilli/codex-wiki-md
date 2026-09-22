<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [compact H-hull](../../../../../../compact-h-hull.md) is a bounded relatively closed subset $K$ of the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) such that $\mathbb H\setminus K$ is a [simply connected domain](../../../../../../simply-connected-domain.md). This does not require its closure to be connected. Its [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) is the unique [conformal map](../../../../../../conformal-map.md) $g_K:\mathbb H\setminus K\to\mathbb H$ with [hydrodynamic normalization at infinity](../../../../../../hydrodynamic-normalization-at-infinity.md),

$$
g_K(z)=z+\frac{a_K}{z}+O(|z|^{-2}).
$$

The [half-plane capacity](../../../../../../half-plane-capacity.md) is

$$
\boxed{\operatorname{hcap}(K)=a_K
=\lim_{z\to\infty}z\bigl(g_K(z)-z\bigr)\ge0.}
$$

The coefficient is zero exactly for the empty hull.

In terms of the least radius of a real-centred enclosing half-disc, the [sharp displacement bound for a compact H-hull](../../../../../../sharp-displacement-bound-for-a-compact-h-hull.md), also called the continuity estimate, is

$$
\boxed{|g_K(z)-z|\le3\operatorname{rad}(K),
\qquad z\in\mathbb H\setminus K.}
$$

The [differentiability estimate for a mapping-out function](../../../../../../differentiability-estimate-for-a-mapping-out-function.md) is a uniform small-hull expansion: there is an absolute constant $C$ such that if $K\subset\{z:|z-\xi|\le r\}$ with $\xi\in\mathbb R$, then

$$
\boxed{\left|g_K(z)-z-\frac{\operatorname{hcap}(K)}{z-\xi}\right|
\le \frac{Cr\,\operatorname{hcap}(K)}{|z-\xi|^2},
\qquad |z-\xi|>2r.}
$$

These are statements of the two requested estimates. The second is not merely a bound for $g_K'$: it controls the first-order change of a [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) when a small hull is removed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
