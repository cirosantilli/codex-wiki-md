# Equality in Minkowski inequality

↑ **Parent:** [Minkowski inequality](minkowski-inequality.md)

For $1<p<\infty$ and nonzero elements $f,g$ of the same real or complex [Lp space](lp-space.md), equality in the [Minkowski inequality](minkowski-inequality.md) holds if and only if

$$
\frac{f}{\lVert f\rVert_p}=\frac{g}{\lVert g\rVert_p}\quad\text{almost everywhere}.
$$

Equivalently, $g=cf$ [almost everywhere](almost-everywhere.md) for a single positive [real number](real-number.md) $c$. The multiplier must be constant across $X$; matching signs at each input alone is insufficient. For [complex numbers](complex-number.md), an arbitrary complex [scalar multiple](scalar-multiple.md) is also insufficient: $g=if$ gives $\lVert f+g\rVert_p=\sqrt2\lVert f\rVert_p<2\lVert f\rVert_p$ for nonzero $f$. If either element is zero in [Lp space](lp-space.md), equality holds automatically, even if a representative has nonzero values on a [null set](null-set.md).

The reason is [strictly convex normed space](strictly-convex-normed-space.md) geometry. Normalize $f,g$ to unit [Lp norm](lp-norm.md) and use weights $\lVert f\rVert_p/(\lVert f\rVert_p+\lVert g\rVert_p)$ and $\lVert g\rVert_p/(\lVert f\rVert_p+\lVert g\rVert_p)$. Distinct normalized [functions](function-split.md) give a [convex combination](convex-combination.md) of [Lp norm](lp-norm.md) strictly below one. This follows by integrating the strict [convexity](convex-function.md) of $z\mapsto|z|^p$ on the [real numbers](real-number.md) or [complex numbers](complex-number.md); equality therefore forces the normalized [functions](function-split.md) to agree [almost everywhere](almost-everywhere.md).

At $p=1$, equality instead means $|f+g|=|f|+|g|$ [almost everywhere](almost-everywhere.md): the nonnegative difference has zero [integral](integral-split.md). For real [functions](function-split.md), this is $fg\geq0$ [almost everywhere](almost-everywhere.md). For complex [functions](function-split.md), their nonzero values must have the same [argument](argument-complex-analysis.md) wherever both are nonzero, but their magnitude ratio may vary. The disjoint-coordinate [vectors](vector.md) $(1,0)$ and $(0,1)$ illustrate equality without constant proportionality.

At $p=\infty$, no such constant proportionality condition is necessary: $(1,0)$ and $(1,1)$ have [L-infinity norms](l-infinity-norm.md) one and a sum of [L-infinity norm](l-infinity-norm.md) two. Nor must an [essential supremum](essential-supremum.md) be attained: under [Lebesgue measure](lebesgue-measure.md) on $(0,1)$, $f(x)=g(x)=x$ give equality $2=1+1$, although neither [function](function-split.md) takes the value one. The endpoint [Lp spaces](lp-space.md) need not be [strictly convex normed spaces](strictly-convex-normed-space.md).

## ↑ Ancestors (7)

1. [Minkowski inequality](minkowski-inequality.md)
2. [Lp norm](lp-norm.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Minkowski inequality](minkowski-inequality.md)
