# Affine maps preserve affine combinations

↑ **Parent:** [Affine map](affine-map.md)

For coefficients with [sum](sum.md) one, the defining identity follows from [linearity](linearity.md):

$$
T\left(\sum_i\lambda_iP_i\right)=M\sum_i\lambda_iP_i+b=\sum_i\lambda_i(MP_i+b)=\sum_i\lambda_iT(P_i).
$$

The [translation](translation-geometry.md) appears once on both sides precisely because $\sum_i\lambda_i=1$. In particular, [midpoints](midpoint.md) map to [midpoints](midpoint.md), and a parameterized [line segment](line-segment.md) $(1-t)P+tQ$, $0\leq t\leq1$, maps to $(1-t)T(P)+tT(Q)$. A whole [line](straight-line.md) has the same formula with $t\in\mathbb R$; its image is a [line](straight-line.md) if $M(Q-P)\ne0$, and a single point otherwise.

## ↑ Ancestors (7)

1. [Affine map](affine-map.md)
2. [Affine space](affine-space.md)
3. [Affine geometry](affine-geometry.md)
4. [Geometry and topology](geometry-and-topology-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Control-point influence on a curve](control-point-influence-on-a-curve.md)
