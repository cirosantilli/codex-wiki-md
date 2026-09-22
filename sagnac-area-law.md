# Sagnac area law

↑ **Parent:** [Sagnac effect](sagnac-effect.md)

For a rigidly rotating prescribed vacuum path, use spatial coordinates attached to the apparatus and laboratory time $t$. At a path [point](point-geometry.md) $\mathbf r$, the local apparatus [velocity](velocity.md) is $\mathbf v=\boldsymbol\Omega\times\mathbf r$. A [light](light.md) displacement has instantaneous laboratory displacement $d\mathbf r+\mathbf v\,dt$, up to the common rotation of the spatial axes. The [null condition](null-condition.md) is therefore

$$
c^2dt^2=|d\mathbf r+\mathbf v\,dt|^2.
$$

Write $d\ell=|d\mathbf r|$. To first order in $|\mathbf v|/c$, the positive root is

$$
dt\simeq\frac{d\ell}{c}+\frac{\mathbf v\cdot d\mathbf r}{c^2}.
$$

Reversing the path reverses the [dot product](dot-product.md) term but leaves the leading path-length term unchanged. Subtract the two return times and use the [scalar triple product](scalar-triple-product.md) identity:

$$
\Delta t\simeq\frac{2}{c^2}\oint_C(\boldsymbol\Omega\times\mathbf r)\cdot d\mathbf r
=\frac{2}{c^2}\boldsymbol\Omega\cdot\oint_C\mathbf r\times d\mathbf r
=\frac{4\boldsymbol\Omega\cdot\mathbf A}{c^2}.
$$

This is a [line integral](line-integral.md) version of the [Sagnac area law](sagnac-area-law.md); the [vector area](vector-area.md) identity also follows from [Stokes theorem](stokes-theorem.md). For a mirror-defined polygon the actual ray paths move slightly as the [mirrors](mirror.md) rotate; the stationary optical path at zero [rotation](rotation-mathematics.md) gives the same first-order result. The prescribed-path calculation is an idealization, not an exact finite-speed formula for every moving-mirror layout.

The [dot product](dot-product.md) explains the geometry: only the projection of the oriented [vector area](vector-area.md) along the [angular velocity](angular-velocity.md) contributes. A planar loop whose [normal vector](normal-vector.md) is perpendicular to $\boldsymbol\Omega$ has zero leading delay. For repeated traversals with the same orientation, the signed [vector areas](vector-area.md) add; oppositely oriented lobes can cancel even when the total unsigned [area](surface-area.md) is large. Equal perimeter alone does not imply equal response. A constant translational [velocity](velocity.md) contributes nothing to this leading closed-path [line integral](line-integral.md), since $\oint_Cd\mathbf r=0$.

**Table of contents**

- [Sagnac fringe shift worked example](sagnac-fringe-shift-worked-example.md)

## ↑ Ancestors (5)

1. [Sagnac effect](sagnac-effect.md)
2. [Special relativity](special-relativity-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Relativistic Sagnac delay on a circular ring](relativistic-sagnac-delay-on-a-circular-ring.md)
- [Sagnac area law](sagnac-area-law.md)
- [Sagnac effect](sagnac-effect.md)
