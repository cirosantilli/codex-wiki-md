# Minimum roughness property of a clamped cubic spline

↑ **Parent:** [Clamped cubic spline](clamped-cubic-spline.md)

Let $S$ be a [clamped cubic spline](clamped-cubic-spline.md) [interpolant](interpolant.md) and let $T$ have the same values at all [spline knots](spline-knot.md) and the same endpoint slopes. For $T\in C^2[x_0,x_n]$, or more generally $T'$ an [absolutely continuous function](absolutely-continuous-function.md) with [square-integrable](square-integrable-function.md) [second derivative](second-derivative.md), the exact displayed identity holds. In particular $S$ uniquely minimizes the [second derivative roughness penalty](second-derivative-roughness-penalty.md) $J$ among these competitors.

To prove the identity, put $E=T-S$. On each knot [interval](interval-mathematics.md), two applications of [integration by parts](integration-by-parts.md) give $\int S''E''=[S''E'-S'''E]$, since the cubic piece has zero [fourth derivative](fourth-derivative.md). Terms containing $E$ vanish at the [spline knots](spline-knot.md); terms containing $E'$ cancel at interior [spline knots](spline-knot.md) because $S''$ and $E'$ are continuous. The endpoint terms vanish because $E'$ is zero there. Thus $\int S''E''=0$, and expanding $(S''+E'')^2$ proves the identity. Equality makes $E''=0$, so $E$ is an [affine function](affine-function.md); a prescribed endpoint value and slope force $E=0$.

If $T$ also matches the first [derivative](derivative.md) of $S$ at every [spline knot](spline-knot.md), both $E$ and $E'$ vanish at the ends of each knot [interval](interval-mathematics.md). For a sufficiently differentiable $T$, [integration by parts](integration-by-parts.md) separately on that [interval](interval-mathematics.md) gives the stronger local identity $\int ET^{(4)}=\int(E'')^2\geq0$.

## ↑ Ancestors (9)

1. [Clamped cubic spline](clamped-cubic-spline.md)
2. [Cubic spline](cubic-spline.md)
3. [Spline approximation](spline-approximation.md)
4. [Spline (mathematics)](spline-mathematics.md)
5. [Uniform approximation](uniform-approximation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Clamped cubic spline](clamped-cubic-spline.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2017/3/b/i/solution.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2017/3/b/ii/solution.md)
