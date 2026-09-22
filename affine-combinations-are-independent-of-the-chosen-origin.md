# Affine combinations are independent of the chosen origin

↑ **Parent:** [Affine combination](affine-combination.md)

Keep the [basis](basis.md) fixed and replace the origin by a point with old coordinates $o$. Each point's coordinates change from $p_i$ to $p_i-o$. For coefficients with [sum](sum.md) one, the weighted coordinates become

$$
\sum_i\lambda_i(p_i-o)=\sum_i\lambda_ip_i-o.
$$

Adding the new origin $o$ gives the original point. This proves origin independence rather than asserting that the coordinate tuples themselves stay unchanged.

The requirement cannot be omitted. In the example $A=(0,0)$, $B=(2,0)$, blindly treating $A+B$ as a point gives $(2,0)$ in the old coordinates. If the new origin is $o=(1,1)$, the two coordinates become $(-1,-1)$ and $(1,-1)$; adding them and restoring $o$ instead gives $(1,-1)$. The coefficients sum to two, so this procedure has no origin-independent interpretation as a weighted point.

## ↑ Ancestors (7)

1. [Affine combination](affine-combination.md)
2. [Affine space](affine-space.md)
3. [Affine geometry](affine-geometry.md)
4. [Geometry and topology](geometry-and-topology-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
