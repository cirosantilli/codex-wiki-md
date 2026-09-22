# Tangent vector

↑ **Parent:** [Differential geometry](differential-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tangent_vector)

A [tangent vector](tangent-vector.md) at a point $p$ of a [smooth manifold](smooth-manifold.md) without boundary records an instantaneous [velocity](classical-mechanics.md#velocity) through $p$. Its base point is part of the data; measuring its length additionally requires a [Riemannian metric](riemannian-metric.md). Intrinsically, a [smooth curve](differential-geometry.md#smooth-curve) $\gamma$ with $\gamma(0)=p$ defines its [tangent vector](tangent-vector.md) by how every local [smooth function](analysis.md#smooth-function) changes along it:

$$
v(f)=\left.\frac{d}{dt}f(\gamma(t))\right|_{t=0}.
$$

This is a [derivation at a point](#derivation-at-a-point). Two [smooth curves](differential-geometry.md#smooth-curve) through $p$ represent the same [tangent vector](tangent-vector.md) if these [derivatives](calculus.md#derivative) agree for every such [smooth function](analysis.md#smooth-function); equivalently, their coordinate [velocity vectors](#velocity-vector) agree in one [manifold chart](differential-geometry.md#manifold-chart). The [chain rule](calculus.md#chain-rule) makes that agreement independent of the chosen [manifold chart](differential-geometry.md#manifold-chart). [Loring W. Tu, An Introduction to Manifolds, §8.6: curves and intrinsic velocity](https://www.math.toronto.edu/~jeffrey/matd67/tu.pdf)

For an [embedded submanifold](smooth-manifold.md#embedded-submanifold) of [Euclidean space](normed-vector-space.md#euclidean-norm), the intrinsic [tangent vector](tangent-vector.md) is represented by the ordinary [derivative](calculus.md#derivative) $\gamma'(0)$, with its base point $p$ retained. A drawn arrow starting at $p$ represents that [tangent vector](tangent-vector.md); its endpoint $p+\gamma'(0)$ need not lie on the [embedded submanifold](smooth-manifold.md#embedded-submanifold). Nor is a [tangent vector](tangent-vector.md) required to be a [unit tangent vector](#unit-tangent-vector): a stationary [smooth curve](differential-geometry.md#smooth-curve) gives the [zero vector](vector-space.md#zero-vector), which belongs to the [tangent space](#tangent-space) but has no direction to normalize.

Here are explicit calculations. In $\mathbb R^2$, $\gamma(t)=(t,t^2)$ and $\eta(t)=(t,2t^2)$ have different routes but the same [tangent vector](tangent-vector.md) $(1,0)$ at $(0,0)$. For $f(x,y)=3x+y$, both give $v(f)=3$. For a [circle](topology.md#circle) of [radius](topology.md#radius) $R$, $c(t)=(R\cos(\omega t),R\sin(\omega t))$ has [tangent vector](tangent-vector.md) $(0,R\omega)$ at $(R,0)$: changing $\omega$ changes the [speed](classical-mechanics.md#speed) or reverses travel without changing the [circle](topology.md#circle).

A [reparametrization](differential-geometry.md#reparametrization) $\beta(s)=\gamma(h(s))$ with $h(0)=0$ gives, by the [chain rule](calculus.md#chain-rule), $\beta'(0)=h'(0)\gamma'(0)$. A regular change of [curve parameter](differential-geometry.md#curve-parameter) has $h'(0)\ne0$. The singular choice $h(s)=s^3$ instead gives

$$
\gamma(t)=(t,t^2),\qquad \beta(s)=(s^3,s^6),\qquad \gamma'(0)=(1,0),\qquad \beta'(0)=(0,0).
$$

Both describe the same [parabola](euclidean-geometry.md#parabola), whose [tangent line](calculus.md#tangent-line) at the origin is still the horizontal axis. The zero [velocity](classical-mechanics.md#velocity) diagnoses this singular change of [curve parameter](differential-geometry.md#curve-parameter), whose inverse is not differentiable at zero; it does not show that the geometric [tangent line](calculus.md#tangent-line) is absent. The [regular curve](differential-geometry.md#regular-curve) $\gamma$ supplies its nonzero direction.

<a id="image-one-parabola-different-velocities-a-singular-parameter-change-can-stop-the-arrow"></a>
![](tangent-vectors-spaces-planes-curve-velocities.png)

**[Figure 1](#image-one-parabola-different-velocities-a-singular-parameter-change-can-stop-the-arrow). One parabola, different velocities: a singular parameter change can stop the arrow**.

The diagram is an analytical illustration of these exact [parametric curves](topology.md#parametric-curve), with equal parameter increments marked on each route. It separates geometry from traversal: the [tangent line](calculus.md#tangent-line) depends on the route, while a [velocity vector](#velocity-vector) also depends on how the [curve parameter](differential-geometry.md#curve-parameter) advances.

**Table of contents**

- [Derivation at a point](#derivation-at-a-point)
- [Tangent space](#tangent-space)
  - [Tangent plane](#tangent-plane)
  - [Tangent space by point derivations](#tangent-space-by-point-derivations)
  - [Cotangent space](#cotangent-space)
    - [Inner product on exterior powers of a cotangent space](#inner-product-on-exterior-powers-of-a-cotangent-space)
  - [Tangent space from a local parametrization](#tangent-space-from-a-local-parametrization)
  - [Closedness of tangent spaces under convergent base points](#closedness-of-tangent-spaces-under-convergent-base-points)
  - [Coordinate basis](#coordinate-basis)
- [Unit tangent vector](#unit-tangent-vector)
- [Velocity vector](#velocity-vector)

## Derivation at a point

↑ **Parent:** [Tangent vector](tangent-vector.md)

At $p$ on a [smooth manifold](smooth-manifold.md), a derivation at that point is a real-linear map $v:C_p^\infty(M)\to\mathbb R$ on [germs](sheaf-of-modules.md#germ-of-a-sheaf-section) of smooth functions with $v(fh)=f(p)v(h)+h(p)v(f)$. It defines a [tangent vector](tangent-vector.md). The local factorization $f-f(p)=\sum_i(x^i-x^i(p))f_i$ gives $v(f)=\sum_i v(x^i)\partial_i f(p)$, so the coordinate derivations form a basis of the [tangent space](#tangent-space).

## Tangent space

↑ **Parent:** [Tangent vector](tangent-vector.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tangent_space)

At a fixed point $p$ of an $n$-dimensional [smooth manifold](smooth-manifold.md) $M$ without boundary, the [tangent space](#tangent-space) $T_pM$ is the real [vector space](vector-space.md) of all [tangent vectors](tangent-vector.md) at $p$. In [manifold charts](differential-geometry.md#manifold-chart) $x=(x^1,\ldots,x^n)$ and $y=(y^1,\ldots,y^n)$, a [tangent vector](tangent-vector.md) has components

$$
v=\sum_{i=1}^n v_x^i\left.\frac{\partial}{\partial x^i}\right|_p,\qquad
v_y^a=\sum_{i=1}^n\left.\frac{\partial y^a}{\partial x^i}\right|_p v_x^i.
$$

The [coordinate basis](#coordinate-basis) transforms inversely, so the [tangent vector](tangent-vector.md) is unchanged. This invertible [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) also preserves [vector addition](vector-space.md#vector-addition) and [scalar multiplication](vector-space.md#scalar-multiplication), giving a [vector space](vector-space.md) of [dimension](vector-space.md#dimension-vector-space) $n$ independently of coordinates. [Eckhard Meinrenken, Differentiable Manifolds, §1.5: tangent spaces and coordinate bases](https://www.math.toronto.edu/mein/teaching/LectureNotes/Man.pdf)

For example, at $(x,y)=(1,0)$ in $\mathbb R^2$, use the alternative [manifold chart](differential-geometry.md#manifold-chart) $u=x$, $w=y+x^2$. The [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) sends $(v_x,v_y)=(2,3)$ to $(v_u,v_w)=(2,7)$. Indeed, the [smooth curve](differential-geometry.md#smooth-curve) $(x(t),y(t))=(1+2t,3t)$ gives $w(t)=1+7t+4t^2$. Conversely, $\partial_u|_p=\partial_x|_p-2\partial_y|_p$ and $\partial_w|_p=\partial_y|_p$, so $2\partial_u|_p+7\partial_w|_p=2\partial_x|_p+3\partial_y|_p$. The numbers change; their action on every [smooth function](analysis.md#smooth-function) does not.

For an [embedded submanifold](smooth-manifold.md#embedded-submanifold) $M\subseteq\mathbb R^N$, the [tangent space](#tangent-space) can be identified with the [vector subspace](vector-space.md#vector-subspace)

$$
T_pM=\{\gamma'(0):\gamma:(-\varepsilon,\varepsilon)\to M\text{ is smooth},\ \gamma(0)=p\}.
$$

A proof outline explains why every coordinate vector is possible: in a [manifold chart](differential-geometry.md#manifold-chart) $x$, lift the short straight path $x(p)+ta$ using $x^{-1}$. Its [tangent vector](tangent-vector.md) has components $a$. For a regular local parametrization $X:U\subseteq\mathbb R^n\to M$, the same [chain rule](calculus.md#chain-rule) gives $T_pM=\operatorname{im}DX_q$, where $X(q)=p$. This is the [tangent space from a local parametrization](#tangent-space-from-a-local-parametrization).

For the [sphere](euclidean-geometry.md#sphere) $S_R^2=\{p\in\mathbb R^3:p\cdot p=R^2\}$, differentiating that equation gives $p\cdot v=0$. Conversely, for any nonzero $v$ with $p\cdot v=0$, the [smooth curve](differential-geometry.md#smooth-curve)

$$
\gamma_v(t)=p\cos\left(\frac{\|v\|t}{R}\right)+R\frac{v}{\|v\|}\sin\left(\frac{\|v\|t}{R}\right)
$$

lies on the [sphere](euclidean-geometry.md#sphere) and has $\gamma_v'(0)=v$; use a constant [smooth curve](differential-geometry.md#smooth-curve) for $v=0$. Thus $T_pS_R^2=\{v:p\cdot v=0\}$, not merely a subset of that plane. At $p=(0,0,R)$ this [vector subspace](vector-space.md#vector-subspace) is $v_z=0$, while the affine [tangent plane](#tangent-plane) drawn through $p$ is $z=R$.

This also explains a [mechanical constraint](classical-mechanics.md#constraint-mechanics) without requiring a force calculation. In the ideal mathematical model of a particle confined to a stationary [sphere](euclidean-geometry.md#sphere), its allowed [velocities](classical-mechanics.md#velocity) at $p$ are exactly $T_pS_R^2$: the radial component must vanish, but either independent tangential direction is available. For a general stationary [holonomic constraint](classical-mechanics.md#holonomic-constraint) $F(q)=0$ with independent equations, the [regular level set theorem](differential-geometry.md#regular-level-set-theorem) gives $T_qM=\ker DF_q$. These are instantaneous kinematic possibilities; they do not determine the actual subsequent motion. On a general [smooth manifold](smooth-manifold.md), [tangent spaces](#tangent-space) at different base points cannot be identified canonically; an [affine connection](vector-bundle.md#affine-connection) supplies [parallel transport](vector-bundle.md#parallel-transport) when such comparisons are needed.

### Tangent plane

↑ **Parent:** [Tangent space](#tangent-space)

For an embedded [regular surface](differential-geometry.md#smooth-surface) $M\subseteq\mathbb R^3$ and $p\in M$, the affine [tangent plane](#tangent-plane) is

$$
p+T_pM=\{p+v:v\in T_pM\}.
$$

It is a set of points through $p$, whereas the [tangent space](#tangent-space) $T_pM$ is a [vector space](vector-space.md) of displacements with [zero vector](vector-space.md#zero-vector). Some texts also call that two-dimensional [tangent space](#tangent-space) the [tangent plane](#tangent-plane); here the translation by $p$ distinguishes the two uses. For a regular [parametric surface](differential-geometry.md#parametric-surface) $X(u,v)$ with $p=X(u_0,v_0)$,

$$
T_pM=\operatorname{span}\{X_u,X_v\},\qquad
p+T_pM=\{p+aX_u+bX_v:a,b\in\mathbb R\},
$$

where the [partial derivatives](multivariable-calculus.md#partial-derivative) are evaluated at $(u_0,v_0)$. Regularity means that these [tangent vectors](tangent-vector.md) are [linearly independent](vector-space.md#linear-independence), equivalently $X_u\times X_v\ne0$. Their [cross product](vector-space.md#cross-product) is a [normal vector](differential-geometry.md#normal-vector). [Theodore Shifrin, Differential Geometry: A First Course in Curves and Surfaces, Chapter 2, §1: regular parametrizations and tangent planes](https://www.math.uga.edu/sites/default/files/inline-files/ShifrinDiffGeo.pdf)

For an implicit [regular surface](differential-geometry.md#smooth-surface) $F(x,y,z)=0$, require a [smooth function](analysis.md#smooth-function) $F$ with $\nabla F(p)\ne0$. Then

$$
T_pM=\ker DF_p=\{v:\nabla F(p)\cdot v=0\},\qquad
p+T_pM=\{r:\nabla F(p)\cdot(r-p)=0\}.
$$

Differentiating $F(\gamma(t))=0$ proves that every surface [velocity](classical-mechanics.md#velocity) lies in the displayed [kernel of a linear map](kernel-of-a-linear-map.md); the [implicit function theorem](multivariable-calculus.md#implicit-function-theorem) gives a local graph with two independent coordinates, proving equality. The [gradient](multivariable-calculus.md#gradient) is the [normal vector](differential-geometry.md#normal-vector) with respect to the ambient [dot product](inner-product.md#dot-product). [Eckhard Meinrenken, Differentiable Manifolds, Theorem 1.15: regular level sets](https://www.math.toronto.edu/mein/teaching/LectureNotes/Man.pdf)

For the [sphere](euclidean-geometry.md#sphere) $F(r)=r\cdot r-R^2$, $\nabla F(p)=2p\ne0$, and the affine [tangent plane](#tangent-plane) has equation $p\cdot r=R^2$. At the unit [sphere](euclidean-geometry.md#sphere)'s north pole $p=(0,0,1)$, compare the plane $z=1$ with the displacement [tangent space](#tangent-space) $v_z=0$. The regular [parametric surface](differential-geometry.md#parametric-surface) $X(u,v)=(u,v,\sqrt{1-u^2-v^2})$, for $u^2+v^2<1$, gives $X_u(0,0)=(1,0,0)$ and $X_v(0,0)=(0,1,0)$, confirming the same answer.

<a id="image-the-sphere-s-tangent-plane-passes-through-the-base-point-its-tangent-space-contains-displacements"></a>
![](tangent-vectors-spaces-planes-sphere-plane.png)

**[Figure 2](#image-the-sphere-s-tangent-plane-passes-through-the-base-point-its-tangent-space-contains-displacements). The sphere's tangent plane passes through the base point; its tangent space contains displacements**.

This analytical illustration shows a unit [sphere](euclidean-geometry.md#sphere) and a vertical cross-section. The [smooth curves](differential-geometry.md#smooth-curve) $\gamma_1(t)=(\sin t,0,\cos t)$ and $\gamma_2(t)=(0,\sin t,\cos t)$ give the two displayed [tangent vectors](tangent-vector.md) at $p$. The straight point $p+tv$ for any nonzero $v\in T_pS^2$ is outside the [sphere](euclidean-geometry.md#sphere) when $t\ne0$, since $\|p+tv\|^2=1+t^2\|v\|^2$. A [tangent plane](#tangent-plane) therefore captures first-order motion, not an exact patch of the [regular surface](differential-geometry.md#smooth-surface).

The same idea makes local approximation useful. For the [graph of a function](function.md#graph-of-a-function) $z=f(x,y)$ with $f$ a [smooth function](analysis.md#smooth-function), the affine [tangent plane](#tangent-plane) is $z=f(a,b)+f_x(a,b)(x-a)+f_y(a,b)(y-b)$. [Gilbert Strang and Edwin Herman, OpenStax Calculus Volume 3, §4.4: tangent planes and linear approximations](https://openstax.org/books/calculus-volume-3/pages/4-4-tangent-planes-and-linear-approximations) With continuous second [partial derivatives](multivariable-calculus.md#partial-derivative), the vertical error is $O((x-a)^2+(y-b)^2)$ in [Big O notation](real-analysis.md#big-o-notation). On the unit [sphere](euclidean-geometry.md#sphere) near its north pole, $\sqrt{1-u^2-v^2}=1-\tfrac12(u^2+v^2)+O((u^2+v^2)^2)$: the [tangent plane](#tangent-plane) loses quadratic bending while preserving all first-order [velocities](classical-mechanics.md#velocity).

A failed regularity test needs interpretation. Replacing the [sphere](euclidean-geometry.md#sphere) equation by $G(r)=(r\cdot r-1)^2=0$ makes $\nabla G=0$ everywhere on the same perfectly regular [sphere](euclidean-geometry.md#sphere), so this defining [smooth function](analysis.md#smooth-function) cannot recover its [tangent plane](#tangent-plane). Similarly, the usual spherical [parametric surface](differential-geometry.md#parametric-surface) loses [matrix rank](vector-space.md#matrix-rank) at the poles, while the graph parametrization above remains regular there. A vanishing [gradient](multivariable-calculus.md#gradient) or degenerate parametrization invalidates that calculation; it alone does not prove that the underlying geometry has no [tangent plane](#tangent-plane).

### Tangent space by point derivations

↑ **Parent:** [Tangent space](#tangent-space)

A tangent vector is a [linear map](vector-space.md#linear-map) on [germs](sheaf-of-modules.md#germ-of-a-sheaf-section) of smooth functions satisfying $D(ab)=a(x)D(b)+b(x)D(a)$. In a [manifold chart](differential-geometry.md#manifold-chart), first-order expansion shows $Dh=\sum_iD(u^i)\partial_i h(x)$. Thus the coordinate [derivations](associative-algebra.md#derivation-of-an-algebra) form a [basis](vector-space.md#basis), and the [dimension](vector-space.md#dimension-vector-space) equals the manifold [dimension](vector-space.md#dimension-vector-space). Composition of [germs](sheaf-of-modules.md#germ-of-a-sheaf-section) with a [smooth map](smooth-manifold.md#smooth-map-between-manifolds) defines its [differential of a smooth map](smooth-manifold.md#differential-of-a-smooth-map) without choosing charts.

### Cotangent space

↑ **Parent:** [Tangent space](#tangent-space)

The cotangent space at $p$ is the [dual vector space](dual-space.md) $T_p^*M=(T_pM)^*$. Its elements are [covectors](dual-space.md#covector) on the [tangent space](#tangent-space). In a [manifold chart](differential-geometry.md#manifold-chart) $x$, the basis $dx^i|_p$ is dual to $\partial_i|_p$. Under a coordinate change to $y$, the coefficients of $\alpha=a_i dx^i=b_jdy^j$ obey $b_j=\sum_i a_i\partial x^i/\partial y^j$. The disjoint union of these spaces is the [cotangent bundle](symplectic-geometry.md#cotangent-bundle).

#### Inner product on exterior powers of a cotangent space

↑ **Parent:** [Cotangent space](#cotangent-space)

A [Riemannian metric](riemannian-metric.md) induces a dual [inner product](inner-product.md) on each [cotangent space](#cotangent-space). On decomposable covectors define $\langle\xi_1\wedge\cdots\wedge\xi_p,\zeta_1\wedge\cdots\wedge\zeta_p\rangle=\det(\langle\xi_i,\zeta_j\rangle)$ and extend bilinearly. Increasing wedges of an orthonormal coframe form an orthonormal basis. This positive-definite inner product is the one used to define the [Hodge star operator](differential-form.md#hodge-star-operator).

### Tangent space from a local parametrization

↑ **Parent:** [Tangent space](#tangent-space)

If $\phi:U\subseteq\mathbb R^d\to M\subseteq\mathbb R^n$ is a local parametrization with $\phi(u)=p$, then

$$
T_pM=\operatorname{im}D\phi_u.
$$

The derivative has rank $d$, so this is a $d$-dimensional vector subspace. A change of parametrization composes $D\phi_u$ with an invertible coordinate-change derivative, leaving its image unchanged.

### Closedness of tangent spaces under convergent base points

↑ **Parent:** [Tangent space](#tangent-space)

For an embedded smooth manifold $M\subseteq\mathbb R^n$, if $p_i\to p$, $w_i\in T_{p_i}M$, and $w_i\to w$, then $w\in T_pM$. In a local graph representation $M=\{(u,g(u))\}$, write $w_i=(v_i,Dg(u_i)v_i)$ and use continuity of $Dg$.

### Coordinate basis

↑ **Parent:** [Tangent space](#tangent-space)

A [manifold chart](differential-geometry.md#manifold-chart) with coordinates $x^\mu$ induces a smooth [local frame](vector-bundle.md#frame-of-a-vector-bundle) of the [tangent bundle](vector-bundle.md#tangent-bundle), with [tangent vectors](tangent-vector.md) $\partial_\mu=\partial/\partial x^\mu$ forming a [basis](vector-space.md#basis) of each [tangent space](#tangent-space). Their [Lie brackets of vector fields](differential-geometry.md#lie-bracket-of-vector-fields) vanish because mixed [partial derivatives](multivariable-calculus.md#partial-derivative) of smooth functions commute. Under a change of coordinates they transform by the [chain rule](calculus.md#chain-rule): $\partial/\partial y^\nu=(\partial x^\mu/\partial y^\nu)\partial/\partial x^\mu$, with coefficients given by the [Jacobian matrix](multivariable-calculus.md#jacobian-matrix).

## Unit tangent vector

↑ **Parent:** [Tangent vector](tangent-vector.md)

For a [regular curve](differential-geometry.md#regular-curve) $\mathbf r(t)$ with nonzero [velocity vector](#velocity-vector), its unit tangent vector is

$$
T(t)=\frac{\mathbf r'(t)}{\|\mathbf r'(t)\|}.
$$

The [Euclidean norm](normed-vector-space.md#euclidean-norm) in the denominator removes the traversal [speed](classical-mechanics.md#speed), leaving a [unit vector](vector-space.md#unit-vector) that records direction. A positive change of traversal [speed](classical-mechanics.md#speed) leaves this direction unchanged; reversing the direction of travel reverses $T$. In [arc length](riemannian-geometry.md#arc-length) coordinates, $T=d\mathbf r/ds$.

For the [parabola](euclidean-geometry.md#parabola) $\mathbf r(t)=(t,t^2)$, the [velocity vector](#velocity-vector) is $(1,2t)$ and the [speed](classical-mechanics.md#speed) is $\sqrt{1+4t^2}$. At $t=1$, $T=(1,2)^T/\sqrt5$. The [tangent vector](tangent-vector.md) $(1,2)^T$ and the [unit tangent vector](#unit-tangent-vector) point in the same direction, but only the latter has [Euclidean norm](normed-vector-space.md#euclidean-norm) one. The [principal normal vector](differential-geometry.md#principal-normal-vector) is a further choice based on how this direction changes, where the [curvature](differential-geometry.md#curvature) is nonzero. [OpenStax Calculus Volume 3, §3.3: unit tangent and principal normal](https://openstax.org/books/calculus-volume-3/pages/3-3-arc-length-and-curvature)

## Velocity vector

↑ **Parent:** [Tangent vector](tangent-vector.md)

The velocity vector of a parametrized curve $\mathbf r(t)$ is its tangent vector $\mathbf r'(t)$.

## ↑ Ancestors (5)

1. [Differential geometry](differential-geometry.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (117)

- [Agreement of two path integrals does not imply conservativeness](multivariable-calculus.md#agreement-of-two-path-integrals-does-not-imply-conservativeness)
- [Bézier curve](computer-aided-geometric-design.md#bezier-curve)
- [Chaikin subdivision](computer-aided-geometric-design.md#chaikin-subdivision)
- [Circular torus coordinates](multivariable-calculus.md#circular-torus-coordinates)
- [Closest-point search on a subdivision curve](computer-aided-geometric-design.md#closest-point-search-on-a-subdivision-curve)
- [Continuation method](numerical-analysis.md#continuation-method)
- [Continuation predictor-corrector step](numerical-analysis.md#continuation-predictor-corrector-step)
- [Coordinate basis](#coordinate-basis)
- [Covector](dual-space.md#covector)
- [Derivation at a point](#derivation-at-a-point)
- [Differential form](differential-form.md)
- [Differential geometry of surfaces](differential-geometry.md#differential-geometry-of-surfaces)
- [Differential of a smooth function](smooth-manifold.md#differential-of-a-smooth-function)
- [Differentiating left-invariant matrix fields](lie-theory.md#differentiating-left-invariant-matrix-fields)
- [Directional derivative](multivariable-calculus.md#directional-derivative)
- [Exponential map of a Lie group](lie-theory.md#exponential-map-of-a-lie-group)
- [First fundamental form](differential-geometry.md#first-fundamental-form)
- [Geodesic](riemannian-geometry.md#geodesic)
- [Geodesic conserved quantity from a Killing vector](killing-vector-field.md#geodesic-conserved-quantity-from-a-killing-vector)
- [Holonomy around circular fibres](fiber-bundle.md#holonomy-around-circular-fibres)
- [Hyperbolic parametrization of prolate spheroidal coordinates](general-relativity.md#hyperbolic-parametrization-of-prolate-spheroidal-coordinates)
- [Induced metric](riemannian-geometry.md#induced-metric)
- [Isocline](differential-equation.md#isocline)
- [Isometric immersion](differential-geometry.md#isometric-immersion)
- [Killing equation](killing-vector-field.md#killing-equation)
- [Killing vector field](killing-vector-field.md)
- [Knot](knot-theory.md#knot)
- [Knot diagram](knot-theory.md#knot-diagram)
- [Lecture Notes on General Relativity by Sean M. Carroll](physics-bibliography.md#lecture-notes-on-general-relativity-by-sean-m-carroll)
- [Mean curvature of a catenoid](second-fundamental-form.md#mean-curvature-of-a-catenoid)
- [Normal reversal around the Möbius core](topological-surface.md#normal-reversal-around-the-mobius-core)
- [Normal vector](differential-geometry.md#normal-vector)
- [One-form](differential-form.md#one-form)
- [One-parameter subgroup](lie-theory.md#one-parameter-subgroup)
- [Outward conormal of a surface boundary](differential-geometry.md#outward-conormal-of-a-surface-boundary)
- [Parabolic coordinates](multivariable-calculus.md#parabolic-coordinates)
- [Parametric curve](topology.md#parametric-curve)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-56.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-59.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-59.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-14.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-68.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-68.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-60.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2.md#24h/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-76.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-86.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-17.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-58.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#1/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#4/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-50.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-17.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-17.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-3.md#3c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#36d/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#36d/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-309.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1.md#11f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2.md#11f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#12e/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#12e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-3.md#2g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#26j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-1.md#4c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-105.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-332.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1.md#7/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1.md#7/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2.md#section-b/6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#11/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1.md#19/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2.md#13/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2.md#13/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2.md#19/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2.md#13/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2.md#13/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2.md#16/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1.md#10/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2015/paper-1.md#2/c/solution)
- [Principal curvature](second-fundamental-form.md#principal-curvature)
- [Pseudo-arclength continuation](numerical-analysis.md#pseudo-arclength-continuation)
- [Pullback of a differential form](differential-form.md#pullback-of-a-differential-form)
- [Riemannian distance](riemannian-geometry.md#riemannian-distance)
- [Riemannian metric](riemannian-metric.md)
- [Rotational flux through an ellipsoidal graph patch](multivariable-calculus.md#rotational-flux-through-an-ellipsoidal-graph-patch)
- [Shape operator](second-fundamental-form.md#shape-operator)
- [Spherical geometry](geometry-and-topology.md#spherical-geometry)
- [Spherical law of cosines](geometry-and-topology.md#spherical-law-of-cosines)
- [Spherical law of sines](geometry-and-topology.md#spherical-law-of-sines)
- [Spherical triangle](geometry-and-topology.md#spherical-triangle)
- [Subdivision surface](computer-aided-geometric-design.md#subdivision-surface)
- [Tangent plane](#tangent-plane)
- [Tangent space](#tangent-space)
- [Tangent vector](tangent-vector.md)
- [Tangential boundary derivative](differential-equation.md#tangential-boundary-derivative)
- [Theorema Egregium](differential-geometry.md#theorema-egregium)
- [Timelike curve](special-relativity.md#timelike-curve)
- [Transversal surface intersection tracing](numerical-analysis.md#transversal-surface-intersection-tracing)
- [Unit tangent vector](#unit-tangent-vector)
- [Vector calculus in elliptic cylindrical coordinates](multivariable-calculus.md#vector-calculus-in-elliptic-cylindrical-coordinates)
