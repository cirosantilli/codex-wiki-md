# Riemannian metric

↑ **Parent:** [Differential geometry](differential-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemannian_metric)

A Riemannian metric is a smoothly varying [positive-definite](bilinear-form.md#positive-definite-bilinear-form) [inner product](inner-product.md) $g_p$ on each [tangent space](tangent-vector.md#tangent-space) $T_pM$ of a [smooth manifold](smooth-manifold.md). It measures [tangent vectors](tangent-vector.md) before measuring entire journeys:

$$
\|v\|_g=\sqrt{g_p(v,v)},\qquad
\cos\theta=\frac{g_p(u,v)}{\|u\|_g\|v\|_g}\quad(u,v\ne0).
$$

Integrating this speed along a [curve](topology.md#curve) gives [arc length](riemannian-geometry.md#arc-length); taking the [infimum](real-analysis.md#infimum) over routes gives [Riemannian distance](riemannian-geometry.md#riemannian-distance). A [smooth manifold](smooth-manifold.md) together with this measuring rule is a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold).

In a [coordinate chart](differential-geometry.md#manifold-chart) $(x^1,\ldots,x^n)$, the rule is represented by a smooth [positive-definite symmetric matrix](linear-algebra.md#symmetric-positive-definite-matrix) $G=(g_{ij})$:

$$
ds^2=\sum_{i,j}g_{ij}(x)\,dx^i\,dx^j,\qquad
g(v,v)=\sum_{i,j}g_{ij}(x)v^iv^j.
$$

The notation $ds^2$ describes the squared infinitesimal line element, rather than an ordinary distance between distinct points. Changing coordinates changes the [matrix](vector-space.md#matrix) entries; it preserves the measured [norm](normed-vector-space.md#norm) of the same [tangent vector](tangent-vector.md).

For the plane with $ds^2=4dx^2+dy^2$, the [vector](vector-space.md#vector) $(1,0)$ has [norm](normed-vector-space.md#norm) $2$ and $(0,1)$ has [norm](normed-vector-space.md#norm) $1$. The coordinate change $X=2x,Y=y$ turns this into $ds^2=dX^2+dY^2$: coefficients that look different can describe the same geometry. On a [circular cylinder](differential-geometry.md#circular-cylinder) the [induced metric](riemannian-geometry.md#induced-metric) $R^2d\theta^2+dz^2$ similarly becomes Euclidean when unrolled. On a round [sphere](euclidean-geometry.md#sphere), polar coordinates give $R^2d\phi^2+R^2\sin^2\phi\,d\theta^2$, away from the poles; the apparent degeneracy at a pole belongs to this coordinate choice, not to the [Riemannian metric](riemannian-metric.md).

The point of the construction is that measurements make sense intrinsically, even without a chosen surrounding [Euclidean space](normed-vector-space.md#euclidean-norm). It gives a common starting point for [geodesics](riemannian-geometry.md#geodesic), [curvature](differential-geometry.md#curvature) encoded by the [Riemann curvature tensor](riemann-curvature-tensor.md), and the [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator). [Peter Petersen, Riemannian Geometry, §1.1: smoothly varying tangent-space inner products](https://www.math.ucla.edu/~petersen/RG.pdf).

**Table of contents**

- [Rotationally symmetric surface metric](#rotationally-symmetric-surface-metric)
  - [Cyclic angular momentum in a rotational metric](#cyclic-angular-momentum-in-a-rotational-metric)
- [Line element](#line-element)
  - [Line element on a sphere](#line-element-on-a-sphere)
- [Riemannian orthonormal frame](#riemannian-orthonormal-frame)
  - [Normal orthonormal frame](#normal-orthonormal-frame)
- [Nowhere locally homogeneous metric](#nowhere-locally-homogeneous-metric)
  - [Sunada local isometry lemma](#sunada-local-isometry-lemma)
- [Local flattening of a Riemannian metric](#local-flattening-of-a-riemannian-metric)
- [Riemannian gradient](#riemannian-gradient)
- [Euclidean metric](#euclidean-metric)
- [Product Riemannian metric](#product-riemannian-metric)
- [Musical isomorphism](#musical-isomorphism)
- [Pullback of a Riemannian metric](#pullback-of-a-riemannian-metric)
- [Conformal rescaling of a Riemannian metric](#conformal-rescaling-of-a-riemannian-metric)
  - [Levi-Civita connection under conformal rescaling](#levi-civita-connection-under-conformal-rescaling)
    - [Critical-point criterion for equal conformal connections](#critical-point-criterion-for-equal-conformal-connections)
  - [Scalar curvature under conformal rescaling](#scalar-curvature-under-conformal-rescaling)
- [Riemannian volume form](#riemannian-volume-form)
  - [Riemannian volume](#riemannian-volume)
  - [Coordinate invariance of the Riemannian volume form](#coordinate-invariance-of-the-riemannian-volume-form)
  - [Interior contraction of the Riemannian volume form](#interior-contraction-of-the-riemannian-volume-form)
    - [Exterior derivative of contracted volume form](#exterior-derivative-of-contracted-volume-form)
      - [Integration by parts for Riemannian divergence](#integration-by-parts-for-riemannian-divergence)
  - [Parallelism of the Riemannian volume form](#parallelism-of-the-riemannian-volume-form)
  - [Localized volume perturbation](#localized-volume-perturbation)
  - [Volume of a Euclidean unit sphere](#volume-of-a-euclidean-unit-sphere)
  - [Parallel differential form](#parallel-differential-form)
  - [Dirichlet energy on a Riemannian manifold](#dirichlet-energy-on-a-riemannian-manifold)
    - [Dirichlet energy of a map](#dirichlet-energy-of-a-map)

## Rotationally symmetric surface metric

↑ **Parent:** [Riemannian metric](riemannian-metric.md)

An intrinsic two-dimensional metric locally written $ds^2=dr^2+f(r)^2d\phi^2$ with positive $f$. Rotation of the angular coordinate is an [isometry](riemannian-geometry.md#isometry). Such a metric need not have a global realization as a surface of revolution in three-dimensional Euclidean space.

### Cyclic angular momentum in a rotational metric

↑ **Parent:** [Rotationally symmetric surface metric](#rotationally-symmetric-surface-metric)

For the affinely parametrized [geodesic Lagrangian](riemannian-geometry.md#geodesic-lagrangian) $\mathcal L=(\dot r^2+f(r)^2\dot\phi^2)/2$, the conserved cyclic momentum is $J=f(r)^2\dot\phi$. Its [Euler-Lagrange equations](analysis.md#euler-lagrange-equation) are $\ddot r-ff^{\prime}\dot\phi^2=0$ and $\ddot\phi+2f^{\prime}\dot r\dot\phi/f=0$.

## Line element

↑ **Parent:** [Riemannian metric](riemannian-metric.md)

The line element of a [Riemannian metric](riemannian-metric.md) is its local expression for squared infinitesimal length. Along a parametrized [curve](topology.md#curve) $x(t)$, the [arc length](riemannian-geometry.md#arc-length) is $\int\sqrt{g_{ij}(x(t))\dot x^i\dot x^j}\,dt$. For a [circular cylinder](differential-geometry.md#circular-cylinder) of radius $R$ parametrized by angle $\theta$ and axial position $z$, the [induced metric](riemannian-geometry.md#induced-metric) gives $ds^2=R^2d\theta^2+dz^2$. Unrolling with $u=R\theta$ yields the Euclidean form $du^2+dz^2$, explaining the straight unrolled descriptions of [geodesics on a circular cylinder](differential-geometry.md#geodesics-on-a-circular-cylinder).

### Line element on a sphere

↑ **Parent:** [Line element](#line-element)

In [spherical coordinates](multivariable-calculus.md#spherical-coordinate-system) on a [sphere](euclidean-geometry.md#sphere) of radius $R$, the position is $X=R(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta)$. Its coordinate tangent [vectors](vector-space.md#vector) satisfy $X_\theta\cdot X_\phi=0$, $|X_\theta|^2=R^2$, and $|X_\phi|^2=R^2\sin^2\theta$. Expanding $|dX|^2$ proves the displayed [line element](#line-element), the [first fundamental form](differential-geometry.md#first-fundamental-form) of the sphere. Along a parametrized path it gives the [arc length](riemannian-geometry.md#arc-length) by integrating $R\sqrt{\dot\theta^2+\sin^2\theta\,\dot\phi^2}$. The vanishing azimuthal coefficient at a pole is a [coordinate singularity](general-relativity.md#coordinate-singularity), not a singularity of the [sphere](euclidean-geometry.md#sphere).

## Riemannian orthonormal frame

↑ **Parent:** [Riemannian metric](riemannian-metric.md)

A smooth local basis of [vector fields](multivariable-calculus.md#vector-field) whose [inner products](inner-product.md) under a [Riemannian metric](riemannian-metric.md) are the identity matrix. Tracing the [Riemannian Hessian](riemannian-geometry.md#riemannian-hessian) in such a frame gives the [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator), with the chosen sign.

### Normal orthonormal frame

↑ **Parent:** [Riemannian orthonormal frame](#riemannian-orthonormal-frame)

At any point of a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), choose [geodesic normal coordinates](riemannian-geometry.md#geodesic-normal-coordinates) and orthonormalize their coordinate fields smoothly. At the point, the metric is the identity and its first derivatives vanish, so the orthonormalization coefficients have zero first derivatives. The [Christoffel symbols](riemannian-geometry.md#christoffel-symbol) also vanish there. This gives a local [Riemannian orthonormal frame](#riemannian-orthonormal-frame) with the displayed property, useful for invariant identities evaluated at one point.

## Nowhere locally homogeneous metric

↑ **Parent:** [Riemannian metric](riemannian-metric.md)

A smooth [Riemannian metric](riemannian-metric.md) with no nonidentity [local isometry](differential-geometry.md#local-isometry) between open subsets. Equivalently distinct nonempty open subsets never have isometric induced metrics. This strong local rigidity is also called bumpy in some spectral-geometry treatments; it is distinct from the closed-geodesic nondegeneracy convention for bumpy metrics.

### Sunada local isometry lemma

↑ **Parent:** [Nowhere locally homogeneous metric](#nowhere-locally-homogeneous-metric)

On a compact smooth manifold without boundary of dimension at least two, a [residual set](topological-analysis.md#residual-set) of smooth [Riemannian metrics](riemannian-metric.md) consists of [nowhere locally homogeneous metrics](#nowhere-locally-homogeneous-metric). Thus such metrics are dense in the smooth topology by the [Baire category theorem](topological-analysis.md#baire-category-theorem). In dimension one, arclength coordinates always provide nontrivial [local isometries](differential-geometry.md#local-isometry).

## Local flattening of a Riemannian metric

↑ **Parent:** [Riemannian metric](riemannian-metric.md)

A [smooth bump function](partial-differential-equation.md#smooth-bump-function) supported in a chosen coordinate neighborhood and equal to one near a chosen point allows a [Riemannian metric](riemannian-metric.md) to be replaced locally by a flat one. The displayed convex combination stays positive definite and glues smoothly to the original metric outside the support. This is a local modification of the metric, not a claim that the original metric is flat.

## Riemannian gradient

↑ **Parent:** [Riemannian metric](riemannian-metric.md)

For a smooth function $f$ on a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), its Riemannian gradient is the unique [vector field](multivariable-calculus.md#vector-field) satisfying $g(\nabla_gf,V)=df(V)$ for every [vector field](multivariable-calculus.md#vector-field) $V$. It depends on the [Riemannian metric](riemannian-metric.md), and its negative generates the downward [gradient flow](analysis.md#gradient-flow).

## Euclidean metric

↑ **Parent:** [Riemannian metric](riemannian-metric.md)

The Euclidean metric is the constant [Riemannian metric](riemannian-metric.md) on $\mathbb R^n$ given in Cartesian coordinates by $g=\sum_i(dx^i)^2$. Its [Levi-Civita connection](general-relativity.md#levi-civita-connection) has zero [Christoffel symbols](riemannian-geometry.md#christoffel-symbol) in those coordinates, so it is flat and its geodesics are straight lines. The [Euclidean norm](normed-vector-space.md#euclidean-norm) is the pointwise length determined by this metric.

## Product Riemannian metric

↑ **Parent:** [Riemannian metric](riemannian-metric.md)

The product of [Riemannian manifolds](riemannian-geometry.md#riemannian-manifold) has metric

$$
g=p_1^*g_1+p_2^*g_2,\qquad g((u_1,u_2),(v_1,v_2))=g_1(u_1,v_1)+g_2(u_2,v_2).
$$

The tangent summands are orthogonal, and positivity follows because a nonzero product tangent vector has a nonzero component. Its [Levi-Civita connection](general-relativity.md#levi-civita-connection) is the [product affine connection](vector-bundle.md#product-affine-connection) of the two factor [Levi-Civita connections](general-relativity.md#levi-civita-connection): mixed torsion is zero and metric compatibility follows from independence of the two coordinate sets.

## Musical isomorphism

↑ **Parent:** [Riemannian metric](riemannian-metric.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Musical_isomorphism)

A [Riemannian metric](riemannian-metric.md) gives inverse [vector bundle isomorphisms](vector-bundle.md#vector-bundle-isomorphism)

$$
\flat_g:TM\to T^*M,\quad v\mapsto g(v,\cdot),\qquad
\sharp_g:T^*M\to TM.
$$

In coordinates they have [matrices](vector-space.md#matrix) $g_{ij}$ and $g^{ij}$. Every [smooth manifold](smooth-manifold.md) admits a [Riemannian metric](riemannian-metric.md) by a [partition of unity](smooth-manifold.md#partition-of-unity), so its tangent and [cotangent bundles](symplectic-geometry.md#cotangent-bundle) are isomorphic as real smooth [vector bundles](vector-bundle.md). This isomorphism depends on the metric, not merely on the manifold.

## Pullback of a Riemannian metric

↑ **Parent:** [Riemannian metric](riemannian-metric.md)

For a smooth map $f:M\to N$, the pullback of a [Riemannian metric](riemannian-metric.md) is $(f^*g)_p(u,v)=g_{f(p)}(df_pu,df_pv)$. It is positive definite precisely when $df_p$ is injective at every point, that is, when $f$ is an [immersion](differential-geometry.md#immersion). In coordinates, $(f^*g)_{ij}=g_{ab}(f(y))\partial_i f^a\partial_j f^b$.

## Conformal rescaling of a Riemannian metric

↑ **Parent:** [Riemannian metric](riemannian-metric.md)

A conformal rescaling multiplies a Riemannian metric by a positive scalar function. It preserves angles while changing lengths and volumes; in two dimensions, $\widetilde g=e^{2\omega}g$ gives $\Delta_{\widetilde g}=e^{-2\omega}\Delta_g$ on scalar functions.

### Levi-Civita connection under conformal rescaling

↑ **Parent:** [Conformal rescaling of a Riemannian metric](#conformal-rescaling-of-a-riemannian-metric)

For $\widetilde g=e^{2\sigma}g$, the displayed correction is a symmetric tensor, so adding it to $\nabla$ gives a [torsion-free connection](vector-bundle.md#torsion-free-connection). The two extra metric-compatibility pairings sum to $2d\sigma(X)g(Y,Z)$; this is exactly the derivative of the conformal factor. Uniqueness of the [Levi-Civita connection](general-relativity.md#levi-civita-connection) proves the formula. It also yields the [critical-point criterion for equal conformal connections](#critical-point-criterion-for-equal-conformal-connections).

#### Critical-point criterion for equal conformal connections

↑ **Parent:** [Levi-Civita connection under conformal rescaling](#levi-civita-connection-under-conformal-rescaling)

On a positive-dimensional [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), equality means equality of the two covariant derivatives at $p$ for every pair of vector fields. A [critical point](analysis.md#critical-point) of $\sigma$ annihilates the conformal correction. Conversely, writing that correction as $A$, the identity $g(A(v,v),v)=g(v,v)d\sigma(v)$ for all tangent vectors forces $d\sigma=0$ if $A=0$. A smooth function on a nonempty compact boundaryless manifold has a critical point, so conformally related connections coincide somewhere. Compact manifolds with boundary need not have one.

### Scalar curvature under conformal rescaling

↑ **Parent:** [Conformal rescaling of a Riemannian metric](#conformal-rescaling-of-a-riemannian-metric)

In dimension $N$, the [conformal rescaling of a Riemannian metric](#conformal-rescaling-of-a-riemannian-metric) $\widetilde g=e^{2\omega}g$ changes the [Ricci scalar](general-relativity.md#ricci-scalar) by the displayed formula. In two dimensions the gradient-square term vanishes; for a flat base metric, $\widetilde R=-2e^{-2\omega}\Delta\omega$.

## Riemannian volume form

↑ **Parent:** [Riemannian metric](riemannian-metric.md)

On an oriented Riemannian $n$-manifold, the volume form is the unique positive $n$-form taking value one on every positively oriented orthonormal frame. In positive local coordinates,

$$
d\operatorname{vol}_g=\sqrt{\det(g_{ij})}\,dx^1\wedge\cdots\wedge dx^n.
$$

### Riemannian volume

↑ **Parent:** [Riemannian volume form](#riemannian-volume-form)

The total Riemannian volume is the integral of the [Riemannian volume form](#riemannian-volume-form), or its density on a nonorientable manifold. In local coordinates the density is $\sqrt{\det g}\,dx^1\cdots dx^d$. It is preserved by [Riemannian isometries](differential-geometry.md#riemannian-isometry). On a closed manifold it is the leading coefficient among the integrated [heat invariants](diffusion-equation.md#heat-invariants), and on a surface it is the [surface area](differential-geometry.md#surface-area).

### Coordinate invariance of the Riemannian volume form

↑ **Parent:** [Riemannian volume form](#riemannian-volume-form)

For positive coordinate charts put $J=\partial y/\partial x$. The [metric tensor](general-relativity.md#metric-tensor) transforms by $g_x=J^Tg_yJ$, giving $\det g_x=(\det J)^2\det g_y$. The top [wedge product of differential forms](differential-form.md#wedge-product-of-differential-forms) transforms by $dy^1\wedge\cdots\wedge dy^n=(\det J)dx^1\wedge\cdots\wedge dx^n$. Since $\det J>0$, the two factors match. Thus the local expressions define one global [Riemannian volume form](#riemannian-volume-form).

### Interior contraction of the Riemannian volume form

↑ **Parent:** [Riemannian volume form](#riemannian-volume-form)

In a positive [Riemannian orthonormal frame](#riemannian-orthonormal-frame) $X=\sum_i f_iE_i$ with dual coframe $\omega_i$, the [Riemannian volume form](#riemannian-volume-form) is $\omega_1\wedge\cdots\wedge\omega_n$. Inserting $E_i$ in its first slot omits $\omega_i$ and produces sign $(-1)^{i-1}$, giving the displayed [interior product](differential-form.md#interior-product) formula.

#### Exterior derivative of contracted volume form

↑ **Parent:** [Interior contraction of the Riemannian volume form](#interior-contraction-of-the-riemannian-volume-form)

At a point in a [normal orthonormal frame](#normal-orthonormal-frame), torsion-freeness makes the frame brackets vanish there, hence the dual one-forms have zero [exterior derivative](differential-form.md#exterior-derivative) there. Differentiating the [interior product](differential-form.md#interior-product) formula then leaves only $\sum_iE_i(f_i)\omega_g$, the [divergence of a Riemannian vector field](multivariable-calculus.md#divergence-of-a-riemannian-vector-field). Since the point is arbitrary, the identity holds globally.

##### Integration by parts for Riemannian divergence

↑ **Parent:** [Exterior derivative of contracted volume form](#exterior-derivative-of-contracted-volume-form)

On a compact oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) without boundary, the [Generalized Stokes theorem](differential-form.md#generalized-stokes-theorem) applied to $f\iota_X\omega_g$ gives the displayed identity. The product expansion is $d(f\iota_X\omega_g)=[X(f)+f\operatorname{div}X]\omega_g$. With boundary, the omitted boundary integral is $\int_{\partial M}f\iota_X\omega_g$.

### Parallelism of the Riemannian volume form

↑ **Parent:** [Riemannian volume form](#riemannian-volume-form)

The [Levi-Civita connection](general-relativity.md#levi-civita-connection) of an oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) preserves its [Riemannian volume form](#riemannian-volume-form). In a positively oriented orthonormal frame its connection matrix is skew-symmetric. Differentiating the wedge of the dual coframe gives minus the trace of that matrix times the [volume form](differential-form.md#volume-form), which is zero. Equivalently [parallel transport](vector-bundle.md#parallel-transport) preserves the metric and orientation, so it preserves the normalized [volume form](differential-form.md#volume-form).

### Localized volume perturbation

↑ **Parent:** [Riemannian volume form](#riemannian-volume-form)

For a nonnegative smooth [bump function](analysis.md#bump-function) supported in an open set, multiplying a [Riemannian metric](riemannian-metric.md) by $1+t\eta$ increases volume there for $t>0$ while leaving the metric elsewhere fixed. For distinct regular compact domains a perturbation supported in the interior of one outside the other breaks equal volume, and therefore breaks any [isometry](riemannian-geometry.md#isometry) between the domains. The perturbations tend to the original metric in the smooth topology.

### Volume of a Euclidean unit sphere

↑ **Parent:** [Riemannian volume form](#riemannian-volume-form)

The $(n-1)$-dimensional [volume](geometry-and-topology.md#volume) of the Euclidean unit sphere equals $n$ times the $n$-dimensional volume of its unit ball. If $R=\sum_i x^i\partial_i$ is the radial vector field and $\omega=dx^1\wedge\cdots\wedge dx^n$, then $d(\iota_R\omega)=n\omega$, and the [Generalized Stokes theorem](differential-form.md#generalized-stokes-theorem) proves the formula.

### Parallel differential form

↑ **Parent:** [Riemannian volume form](#riemannian-volume-form)

A differential form is parallel when its [covariant derivative](general-relativity.md#covariant-derivative) vanishes. Parallel transport then preserves it, and every parallel form is harmonic.

The form is preserved by [parallel transport](vector-bundle.md#parallel-transport); this is the alternating-tensor case of vanishing [covariant derivative](general-relativity.md#covariant-derivative).

### Dirichlet energy on a Riemannian manifold

↑ **Parent:** [Riemannian volume form](#riemannian-volume-form)

For a function $u$ on a compact Riemannian manifold, its Dirichlet energy is $\frac12\int_M|\nabla u|_g^2d\operatorname{vol}_g$. Adding a linear source term $-\int_Mfu\,d\operatorname{vol}_g$ gives Euler-Lagrange equation $-\Delta_gu=f$.

For a scalar function $u$ on a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), the [Dirichlet energy](differential-geometry.md#dirichlet-energy) is $E(u)=\tfrac12\int_M|\nabla u|_g^2\,d\mathrm{vol}_g$.

#### Dirichlet energy of a map

↑ **Parent:** [Dirichlet energy on a Riemannian manifold](#dirichlet-energy-on-a-riemannian-manifold)

For a smooth map between [Riemannian manifolds](riemannian-geometry.md#riemannian-manifold), its Dirichlet energy is half the integral of the squared [norm](normed-vector-space.md#norm) of its differential, using the source and target metrics. When the source is two-dimensional, a conformal change of its metric leaves this energy unchanged. For a [J-holomorphic curve](symplectic-geometry.md#pseudoholomorphic-curve) into a [symplectic manifold](symplectic-geometry.md#symplectic-manifold) with a [compatible almost complex structure](complex-geometry.md#compatible-almost-complex-structure), the [Energy identity for a J-holomorphic curve](symplectic-geometry.md#energy-identity-for-a-j-holomorphic-curve) identifies it with the pulled-back [symplectic area](symplectic-geometry.md#symplectic-area). The norm of a differential here is the full tensor norm, summing its squared values on an orthonormal source frame.

## ↑ Ancestors (5)

1. [Differential geometry](differential-geometry.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (214)

- [Arc length](riemannian-geometry.md#arc-length)
- [Betti-number obstruction to nonnegative Ricci curvature](differential-form.md#betti-number-obstruction-to-nonnegative-ricci-curvature)
- [Bi-invariant Riemannian metric](lie-theory.md#bi-invariant-riemannian-metric)
- [C1 metric on a smooth mapping space](differential-geometry.md#c1-metric-on-a-smooth-mapping-space)
- [Cartan-Ambrose-Hicks theorem](riemannian-geometry.md#cartan-ambrose-hicks-theorem)
- [Clifford multiplication](algebra-over-a-field.md#clifford-multiplication)
- [Compact-core completeness for a Euclidean end](riemannian-geometry.md#compact-core-completeness-for-a-euclidean-end)
- [Compact elliptic spectral theorem](compact-operator.md#compact-elliptic-spectral-theorem)
- [Compatible triple](complex-geometry.md#compatible-triple)
- [Complete positively curved paraboloid](second-fundamental-form.md#complete-positively-curved-paraboloid)
- [Conformal metric](riemann-surfaces.md#conformal-metric)
- [Conformal structure](geometry-and-topology.md#conformal-structure)
- [Contractibility of compatible almost complex structures](complex-geometry.md#contractibility-of-compatible-almost-complex-structures)
- [Critical point of a smooth map](differential-geometry.md#critical-point-of-a-smooth-map)
- [Curvature markers distinguishing finite-cover quotients](riemannian-geometry.md#curvature-markers-distinguishing-finite-cover-quotients)
- [Density bundle](vector-bundle.md#density-bundle)
- [Differential geometry](differential-geometry.md)
- [Differential geometry of surfaces](differential-geometry.md#differential-geometry-of-surfaces)
- [Divergence of a Riemannian vector field](multivariable-calculus.md#divergence-of-a-riemannian-vector-field)
- [Euclidean metric](#euclidean-metric)
- [Euclidean plane](geometry-and-topology.md#euclidean-plane)
- [Existence and uniqueness of the Levi-Civita connection](vector-bundle.md#existence-and-uniqueness-of-the-levi-civita-connection)
- [Exponential convergence of a Morse gradient flow](differential-geometry.md#exponential-convergence-of-a-morse-gradient-flow)
- [Fenchel–Nielsen twist](hyperbolic-geometry.md#fenchel-nielsen-twist)
- [Fiber metric](vector-bundle.md#fiber-metric)
- [Flat circular metrics with trivial holonomy](fiber-bundle.md#flat-circular-metrics-with-trivial-holonomy)
- [Fundamental form of a Hermitian manifold](complex-geometry.md#fundamental-form-of-a-hermitian-manifold)
- [Fundamental theorem of Riemannian geometry](general-relativity.md#fundamental-theorem-of-riemannian-geometry)
- [Gaussian curvature](second-fundamental-form.md#gaussian-curvature)
- [Geodesic metric space](topological-analysis.md#geodesic-metric-space)
- [Harmonic coordinate](numerical-relativity.md#harmonic-coordinate)
- [Heat equation energy identity](diffusion-equation.md#heat-equation-energy-identity)
- [Heat equation maximum principle](diffusion-equation.md#heat-equation-maximum-principle)
- [Heisenberg metric Kaluza-Klein reduction](killing-vector-field.md#heisenberg-metric-kaluza-klein-reduction)
- [Hermitian manifold](complex-geometry.md#hermitian-manifold)
- [Holonomy around circular fibres](fiber-bundle.md#holonomy-around-circular-fibres)
- [Horizontal lift of a vector field through a submersion](differential-geometry.md#horizontal-lift-of-a-vector-field-through-a-submersion)
- [Hyperbolic surface](hyperbolic-geometry.md#hyperbolic-surface)
- [Induced metric](riemannian-geometry.md#induced-metric)
- [Initial data in general relativity](general-relativity.md#initial-data-in-general-relativity)
- [Inner product on exterior powers of a cotangent space](tangent-vector.md#inner-product-on-exterior-powers-of-a-cotangent-space)
- [Integrated second scalar heat coefficient](diffusion-equation.md#integrated-second-scalar-heat-coefficient)
- [Isometric immersion](differential-geometry.md#isometric-immersion)
- [Isometry group](riemannian-geometry.md#isometry-group)
- [Left-invariant group metric](topological-group.md#left-invariant-group-metric)
- [Length of a curve](riemannian-geometry.md#length-of-a-curve)
- [Line element](#line-element)
- [Local flattening of a Riemannian metric](#local-flattening-of-a-riemannian-metric)
- [Localized volume perturbation](#localized-volume-perturbation)
- [Lorentzian metric](general-relativity.md#lorentzian-metric)
- [Metric construction of a compatible almost complex structure](complex-geometry.md#metric-construction-of-a-compatible-almost-complex-structure)
- [Moduli-space approximation for solitons](classical-field-theory-soliton.md#moduli-space-approximation-for-solitons)
- [Musical isomorphism](#musical-isomorphism)
- [Normal bundle of a regular fibre is trivial](differential-geometry.md#normal-bundle-of-a-regular-fibre-is-trivial)
- [Nowhere locally homogeneous metric](#nowhere-locally-homogeneous-metric)
- [One-form](differential-form.md#one-form)
- [Parallel metrics with a common Levi-Civita connection](general-relativity.md#parallel-metrics-with-a-common-levi-civita-connection)
- [Parallel vector field](vector-bundle.md#parallel-vector-field)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1.md#4b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-12.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-12.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-12.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-15.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-9.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-14.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-18.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-74.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1.md#13f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-14.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-14.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-16.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-16.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-16.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-16.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-28.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-57.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1.md#3g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-14.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-18.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-18.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-19.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-19.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2.md#12a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#3g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-15.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-19.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-20.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-20.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-15.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-20.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-23.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-23.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4.md#12a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-15.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-15.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-22.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-17.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-19.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-20.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-20.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-20.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-22.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#24h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-17.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-19.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-22.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-22.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-22.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-14.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-14.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-14.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-14.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#5/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-19.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-19.md#5/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-19.md#5/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-19.md#5/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-19.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#1/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-12.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-14.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-15.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-17.md#5/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#1/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#1/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#1/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-15.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-16.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-16.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-50.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-50.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-51.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-15.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-15.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-16.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-16.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-17.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-17.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1.md#3f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1.md#3f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1.md#3f/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-115.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-116.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-116.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-117.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-117.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-313.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-132.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-308.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-309.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-309.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-1.md#3e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-115.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-307.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-146.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-308.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1.md#2e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-118.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#12e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#2e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-115.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-115.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-118.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-131.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-131.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1.md#10/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1.md#1/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2019.md#section-a/3/solution)
- [Poincare ball model](hyperbolic-geometry.md#poincare-ball-model)
- [Product Laplacian eigenspace decomposition](riemannian-geometry.md#product-laplacian-eigenspace-decomposition)
- [Projected ambient connection](vector-bundle.md#projected-ambient-connection)
- [Pseudo-Riemannian metric](differential-geometry.md#pseudo-riemannian-metric)
- [Pullback of a Riemannian metric](#pullback-of-a-riemannian-metric)
- [Rank-two Killing tensor](riemannian-geometry.md#rank-two-killing-tensor)
- [Ricci soliton](riemannian-geometry.md#ricci-soliton)
- [Riemannian distance](riemannian-geometry.md#riemannian-distance)
- [Riemannian distance induces the manifold topology](riemannian-geometry.md#riemannian-distance-induces-the-manifold-topology)
- [Riemannian divergence theorem](multivariable-calculus.md#riemannian-divergence-theorem)
- [Riemannian geometry](riemannian-geometry.md)
- [Riemannian gradient](#riemannian-gradient)
- [Riemannian heat kernel](diffusion-equation.md#riemannian-heat-kernel)
- [Riemannian manifold](riemannian-geometry.md#riemannian-manifold)
- [Riemannian metric](riemannian-metric.md)
- [Riemannian orthonormal frame](#riemannian-orthonormal-frame)
- [Riemannian product](riemannian-geometry.md#riemannian-product)
- [Riemannian volume density](vector-bundle.md#riemannian-volume-density)
- [Right-invariant Riemannian metric](lie-theory.md#right-invariant-riemannian-metric)
- [Skew-adjoint difference criterion for metric connections](vector-bundle.md#skew-adjoint-difference-criterion-for-metric-connections)
- [Spectral expansion of the Riemannian heat kernel](diffusion-equation.md#spectral-expansion-of-the-riemannian-heat-kernel)
- [Stable minimal surface](second-fundamental-form.md#stable-minimal-surface)
- [Sunada local isometry lemma](#sunada-local-isometry-lemma)
- [Surface Laplacian](differential-geometry.md#surface-laplacian)
- [Tangent vector](tangent-vector.md)
- [Theorema Egregium](differential-geometry.md#theorema-egregium)
- [Top de Rham cohomology of a compact connected oriented manifold](differential-form.md#top-de-rham-cohomology-of-a-compact-connected-oriented-manifold)
- [Tubular neighborhood theorem](differential-geometry.md#tubular-neighborhood-theorem)
- [Upward stability of Riemannian completeness](riemannian-geometry.md#upward-stability-of-riemannian-completeness)
- [Wedge product of differential forms](differential-form.md#wedge-product-of-differential-forms)
- [Weyl law](riemannian-geometry.md#weyl-law)
