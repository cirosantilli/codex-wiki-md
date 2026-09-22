# Tangent space

↑ **Parent:** [Tangent vector](tangent-vector-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tangent_space)

At a fixed point $p$ of an $n$-dimensional [smooth manifold](smooth-manifold-split.md) $M$ without boundary, the [tangent space](tangent-space.md) $T_pM$ is the real [vector space](vector-space-split.md) of all [tangent vectors](tangent-vector-split.md) at $p$. In [manifold charts](manifold-chart.md) $x=(x^1,\ldots,x^n)$ and $y=(y^1,\ldots,y^n)$, a [tangent vector](tangent-vector-split.md) has components

$$
v=\sum_{i=1}^n v_x^i\left.\frac{\partial}{\partial x^i}\right|_p,\qquad
v_y^a=\sum_{i=1}^n\left.\frac{\partial y^a}{\partial x^i}\right|_p v_x^i.
$$

The [coordinate basis](coordinate-basis.md) transforms inversely, so the [tangent vector](tangent-vector-split.md) is unchanged. This invertible [Jacobian matrix](jacobian-matrix.md) also preserves [vector addition](vector-addition.md) and [scalar multiplication](scalar-multiplication.md), giving a [vector space](vector-space-split.md) of [dimension](dimension-vector-space.md) $n$ independently of coordinates. [Eckhard Meinrenken, Differentiable Manifolds, §1.5: tangent spaces and coordinate bases](https://www.math.toronto.edu/mein/teaching/LectureNotes/Man.pdf)

For example, at $(x,y)=(1,0)$ in $\mathbb R^2$, use the alternative [manifold chart](manifold-chart.md) $u=x$, $w=y+x^2$. The [Jacobian matrix](jacobian-matrix.md) sends $(v_x,v_y)=(2,3)$ to $(v_u,v_w)=(2,7)$. Indeed, the [smooth curve](smooth-curve.md) $(x(t),y(t))=(1+2t,3t)$ gives $w(t)=1+7t+4t^2$. Conversely, $\partial_u|_p=\partial_x|_p-2\partial_y|_p$ and $\partial_w|_p=\partial_y|_p$, so $2\partial_u|_p+7\partial_w|_p=2\partial_x|_p+3\partial_y|_p$. The numbers change; their action on every [smooth function](smooth-function.md) does not.

For an [embedded submanifold](embedded-submanifold.md) $M\subseteq\mathbb R^N$, the [tangent space](tangent-space.md) can be identified with the [vector subspace](vector-subspace.md)

$$
T_pM=\{\gamma'(0):\gamma:(-\varepsilon,\varepsilon)\to M\text{ is smooth},\ \gamma(0)=p\}.
$$

A proof outline explains why every coordinate vector is possible: in a [manifold chart](manifold-chart.md) $x$, lift the short straight path $x(p)+ta$ using $x^{-1}$. Its [tangent vector](tangent-vector-split.md) has components $a$. For a regular local parametrization $X:U\subseteq\mathbb R^n\to M$, the same [chain rule](chain-rule.md) gives $T_pM=\operatorname{im}DX_q$, where $X(q)=p$. This is the [tangent space from a local parametrization](tangent-space-from-a-local-parametrization.md).

For the [sphere](sphere.md) $S_R^2=\{p\in\mathbb R^3:p\cdot p=R^2\}$, differentiating that equation gives $p\cdot v=0$. Conversely, for any nonzero $v$ with $p\cdot v=0$, the [smooth curve](smooth-curve.md)

$$
\gamma_v(t)=p\cos\left(\frac{\|v\|t}{R}\right)+R\frac{v}{\|v\|}\sin\left(\frac{\|v\|t}{R}\right)
$$

lies on the [sphere](sphere.md) and has $\gamma_v'(0)=v$; use a constant [smooth curve](smooth-curve.md) for $v=0$. Thus $T_pS_R^2=\{v:p\cdot v=0\}$, not merely a subset of that plane. At $p=(0,0,R)$ this [vector subspace](vector-subspace.md) is $v_z=0$, while the affine [tangent plane](tangent-plane.md) drawn through $p$ is $z=R$.

This also explains a [mechanical constraint](constraint-mechanics.md) without requiring a force calculation. In the ideal mathematical model of a particle confined to a stationary [sphere](sphere.md), its allowed [velocities](velocity.md) at $p$ are exactly $T_pS_R^2$: the radial component must vanish, but either independent tangential direction is available. For a general stationary [holonomic constraint](holonomic-constraint.md) $F(q)=0$ with independent equations, the [regular level set theorem](regular-level-set-theorem.md) gives $T_qM=\ker DF_q$. These are instantaneous kinematic possibilities; they do not determine the actual subsequent motion. On a general [smooth manifold](smooth-manifold-split.md), [tangent spaces](tangent-space.md) at different base points cannot be identified canonically; an [affine connection](affine-connection.md) supplies [parallel transport](parallel-transport.md) when such comparisons are needed.

**Table of contents**

- [Tangent plane](tangent-plane.md)
- [Tangent space by point derivations](tangent-space-by-point-derivations.md)
- [Cotangent space](cotangent-space.md)
  - [Inner product on exterior powers of a cotangent space](inner-product-on-exterior-powers-of-a-cotangent-space.md)
- [Tangent space from a local parametrization](tangent-space-from-a-local-parametrization.md)
- [Closedness of tangent spaces under convergent base points](closedness-of-tangent-spaces-under-convergent-base-points.md)
- [Coordinate basis](coordinate-basis.md)

## ↑ Ancestors (6)

1. [Tangent vector](tangent-vector-split.md)
2. [Differential geometry](differential-geometry-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (94)

- [Ambient restriction formula for the spherical Laplacian](ambient-restriction-formula-for-the-spherical-laplacian.md)
- [Complex Lie group](complex-lie-group.md)
- [Coordinate basis](coordinate-basis.md)
- [Cotangent space](cotangent-space.md)
- [Critical point of a smooth map](critical-point-of-a-smooth-map.md)
- [Critical value](critical-value.md)
- [Derivation at a point](derivation-at-a-point.md)
- [Differential geometry](differential-geometry-split.md)
- [Dimension of a manifold](dimension-of-a-manifold.md)
- [First fundamental form](first-fundamental-form.md)
- [Geodesic trace formula for the Laplace-Beltrami operator](geodesic-trace-formula-for-the-laplace-beltrami-operator.md)
- [Induced metric](induced-metric.md)
- [Isotropic submanifold](isotropic-submanifold.md)
- [Lagrange multiplier](lagrange-multiplier.md)
- [Lagrangian fixed locus of an anti-symplectic involution](lagrangian-fixed-locus-of-an-anti-symplectic-involution.md)
- [Lie algebra](lie-algebra-split.md)
- [Lie bracket](lie-bracket.md)
- [Lie bracket from local group commutators](lie-bracket-from-local-group-commutators.md)
- [Lie group](lie-group.md)
- [Lie theory](lie-theory-split.md)
- [Local isometry](local-isometry.md)
- [Lorentzian manifold](lorentzian-manifold.md)
- [Mean curvature vector](mean-curvature-vector.md)
- [Normal bundle of a regular fibre is trivial](normal-bundle-of-a-regular-fibre-is-trivial.md)
- [Normal vector](normal-vector.md)
- [Orientability](orientability.md)
- [Orientation of a smooth manifold](orientation-of-a-smooth-manifold.md)
- [Oriented atlas](oriented-atlas.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-12/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-12/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-13/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-14/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-14/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-1/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-57/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-19/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-19/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-36/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4/12a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1/24h/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-15/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-20/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-25/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-1/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-23/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-17/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-19/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-17/2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-19/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-19/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-15/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-17/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-16/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-2/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/21g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-17/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-17/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-2/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-102/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-302/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-309/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-309/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/25i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/36d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-131/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-131/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-302/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/26i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/26f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-313/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-102/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-115/1/a/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2014/paper-1/6/b/solution.md)
- [Pseudo-Riemannian manifold](pseudo-riemannian-manifold.md)
- [Riemannian geometry](riemannian-geometry-split.md)
- [Riemannian manifold](riemannian-manifold.md)
- [Riemannian metric](riemannian-metric-split.md)
- [Riemannian submersion](riemannian-submersion.md)
- [Smooth submanifolds with invariant complex tangent spaces are complex](smooth-submanifolds-with-invariant-complex-tangent-spaces-are-complex.md)
- [Surface gradient](surface-gradient.md)
- [Symplectic basis](symplectic-basis.md)
- [Tangent plane](tangent-plane.md)
- [Tangent space](tangent-space.md)
- [Tangent vector](tangent-vector-split.md)
- [Tangential component](tangential-component.md)
- [Transverse preimage theorem](transverse-preimage-theorem.md)
- [Wave map Cauchy data](wave-map-cauchy-data.md)
