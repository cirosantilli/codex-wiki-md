# Trapped spheres as a model for nonspherical collapse

↑ **Parent:** [Penrose singularity theorem](penrose-singularity-theorem.md)

A concrete example separates a [trapped surface](trapped-surface.md) from a failure of coordinates. Use [geometrized units](geometrized-units.md) $G=c=1$, [metric signature](metric-signature.md) $(-,+,+,+)$, and the regular [ingoing Eddington-Finkelstein coordinates](ingoing-eddington-finkelstein-coordinates.md) of a [Schwarzschild black hole](schwarzschild-spacetime-split.md) with [mass](mass.md) $M>0$:

$$
ds^2=-f(r)\,dv^2+2\,dv\,dr+r^2d\Omega^2,\qquad f(r)=1-\frac{2M}{r}.
$$

For a round sphere, choose future [null vector](null-vector.md) normals

$$
k_+=\partial_v+\frac f2\partial_r,\qquad k_-=-\partial_r,
\qquad g(k_+,k_-)=-1.
$$

The [spherical null expansion in ingoing coordinates](spherical-null-expansion-in-ingoing-coordinates.md) follows directly from $A=4\pi r^2$: $\theta_k=2k(r)/r$. At $r=3M$, $(\theta_+,\theta_-)=(1/(9M),-2/(3M))$; at $r=3M/2$, it is $(-2/(9M),-4/(3M))$. Both future light fronts shrink in the second case. At $r=2M$, $\theta_+=0$, so this sphere is [marginally outer trapped surface](marginally-outer-trapped-surface.md), not a strict [trapped surface](trapped-surface.md). In the spherical model this boundary is an [event horizon](event-horizon.md); that identification does not extend to arbitrary geometries.

<a id="image-both-future-null-families-contract-at-a-trapped-surface"></a>
![](penrose-trapped-null-congruences.png)

**[Figure 2](#image-both-future-null-families-contract-at-a-trapped-surface). Both future null families contract at a trapped surface**. The schematic compares signs of [null expansion](null-expansion.md). The horizontal separation represents transverse beam width, not a radial [spacetime](spacetime.md) coordinate; the ellipses represent two-dimensional sections. No horizon location or endpoint of a [null geodesic](null-geodesic.md) is encoded by the drawing.

Although $k_-$ is affine as written, $k_+$ generally obeys $\nabla_{k_+}k_+=(M/r^2)k_+$. These are valid initial normals for the sign test; use [affine rescaling of a null normal](affine-rescaling-of-a-null-normal.md) before applying the affine [Null Raychaudhuri equation](null-raychaudhuri-equation.md). Regularity of the displayed [metric tensor](metric-tensor.md) at $r=2M$ shows why a divergence in another chart would not establish [null geodesic incompleteness](null-geodesic-incompleteness.md).

On a [compact](compact-space.md) [trapped surface](trapped-surface.md), both [null expansions](null-expansion.md) have a uniform negative margin. Sufficiently small smooth perturbations controlling the relevant [metric tensor](metric-tensor.md) and surface derivatives preserve trapping. This conditional robustness does not prove that every nonspherical [gravitational collapse](gravitational-collapse.md) creates a [trapped surface](trapped-surface.md).[p. 58, small departures from symmetry](gravitational-collapse-and-space-time-singularities-by-roger-penrose.md)

## ↑ Ancestors (6)

1. [Penrose singularity theorem](penrose-singularity-theorem.md)
2. [Null geodesic completeness](null-geodesic-completeness.md)
3. [General relativity](general-relativity-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
