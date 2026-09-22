<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An invertible $4\times4$ [matrix](../../../../../matrix.md) $M$, modulo scalar multiples, acts linearly on [homogeneous coordinates](../../../../../homogeneous-coordinate.md). In an affine chart its [projective transformation](../../../../../projective-linear-transformation.md) has the form

$$
x'=\frac{Ax+b}{c^Tx+d},
$$

where the denominator must be nonzero for a finite image. The important nested groups are [Euclidean motions](../../../../../euclidean-motion-of-euclidean-three-space.md), [Euclidean similarities](../../../../../euclidean-similarity.md), invertible [affine maps](../../../../../affine-map.md), and general [projective transformations](../../../../../projective-linear-transformation.md). Their defining preserved structures become progressively weaker.

A [Euclidean motion](../../../../../euclidean-motion-of-euclidean-three-space.md) has $x'=Rx+b$ with $R^TR=I$. It preserves all distances and angles, hence lengths, areas and volumes. Proper motions have $\det R=1$ and preserve orientation as well; allowing reflections preserves unsigned measurements but can reverse signed ones. A [Euclidean similarity](../../../../../euclidean-similarity.md) has $x'=sRx+b$ with $s>0$. It preserves angles and all ratios of lengths; lengths, areas and volumes scale by $s,s^2,s^3$. Thus rigid shape is preserved up to one overall scale.

An invertible [affine map](../../../../../affine-map.md) has $c=0$ and preserves the plane at infinity. It preserves incidence, parallelism, collinear ratios, [affine combinations](../../../../../affine-combination.md), and ratios of volumes. Absolute volume scales by $|\det A|$; the volume-preserving affine subgroup has $|\det A|=1$. Lengths and angles are not affine invariants. A general [projective transformation](../../../../../projective-linear-transformation.md) preserves incidence, collinearity, concurrence, tangency, and the [cross-ratio](../../../../../cross-ratio.md) of four collinear points, but can move the plane at infinity. The [cross-ratio](../../../../../cross-ratio.md), rather than a three-point affine ratio, survives arbitrary projective changes. For a homogeneous [quadric hypersurface](../../../../../quadric-algebraic-geometry.md) $X^TQX=0$, its transformed matrix is $M^{-T}QM^{-1}$, so its rank and projective degeneracy are preserved.

For surface _classes_, rather than a fixed numerical radius or curvature, the consequences are:

| Transformation class | [Sphere](../../../../../sphere.md) | [Circular cylinder](../../../../../circular-cylinder.md) | Finite-apex [general conical surface](../../../../../general-conical-surface.md) | [Elliptic paraboloid](../../../../../elliptic-paraboloid.md) or [hyperbolic paraboloid](../../../../../hyperbolic-paraboloid.md) |
| --- | --- | --- | --- | --- |
| [Euclidean motion](../../../../../euclidean-motion-of-euclidean-three-space.md) | Yes | Yes | Yes | Yes |
| [Euclidean similarity](../../../../../euclidean-similarity.md) | Yes, with scaled radius | Yes, with scaled radius | Yes | Yes, with changed scale |
| Invertible [affine map](../../../../../affine-map.md) | Not generally: an ellipsoid | Not generally: an elliptic cylinder | Yes | Yes, preserving the elliptic/hyperbolic type |
| General [projective transformation](../../../../../projective-linear-transformation.md) | Not generally | Not generally | Concurrence survives, but the apex can move to infinity | Not generally |

For example, the affine stretch $(x,y,z)\mapsto(2x,y,z)$ changes a unit [sphere](../../../../../sphere.md) to $x'^2/4+y'^2+z'^2=1$ and a unit [circular cylinder](../../../../../circular-cylinder.md) to $x'^2/4+y'^2=1$. A [general conical surface](../../../../../general-conical-surface.md) written $P+tD(s)$ transforms affinely into $T(P)+tAD(s)$, so every generator still passes through a finite apex. A nonsingular [elliptic paraboloid](../../../../../elliptic-paraboloid.md) or [hyperbolic paraboloid](../../../../../hyperbolic-paraboloid.md) has quadratic part of rank two and a nonzero linear component in its null direction. An invertible [affine map](../../../../../affine-map.md) preserves that rank, inertia and nonzero null-direction coupling, so translation and linear coordinate changes again put it in elliptic or hyperbolic paraboloid form.

Under a genuinely projective change, these Euclidean classifications depend on which plane is designated as infinity. For the map $(x,y,z)\mapsto(x,y,z)/(1+\alpha z)$, a [circular cylinder](../../../../../circular-cylinder.md) $x^2+y^2=1$ becomes

$$
x'^2+y'^2=(1-\alpha z')^2,
$$

a cone whose apex is finite. The inverse map sends that apex to infinity and produces the cylinder. Thus **a cone is projectively invariant as a family of concurrent generators if an ideal apex is allowed, but finite-apex cones and cylinders are not separately invariant**. Likewise a projective image of a [sphere](../../../../../sphere.md) or either type of paraboloid remains a nonsingular [quadric hypersurface](../../../../../quadric-algebraic-geometry.md), but need not retain its affine or metric type. The distinction between general cones and _circular_ cones matters: circularity is a metric property and is not preserved by arbitrary affine changes.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
