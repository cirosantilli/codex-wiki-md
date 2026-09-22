# Killing vector field

↑ **Parent:** [General relativity](general-relativity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Killing_vector_field)

A [Killing vector field](killing-vector-field.md) describes a direction in which geometry has a continuous [symmetry](physics.md#symmetry-physics): moving points together along its [flow of a vector field](multivariable-calculus.md#flow-of-a-vector-field) preserves the [metric tensor](general-relativity.md#metric-tensor), including its pairing of [tangent vectors](tangent-vector.md). Such a [symmetry](physics.md#symmetry-physics) gives a [geodesic conserved quantity from a Killing vector](#geodesic-conserved-quantity-from-a-killing-vector), often a component of [momentum](momentum.md) or [angular momentum](momentum.md#angular-momentum). The direction may vary with position: [rotation](riemannian-geometry.md#rotation-mathematics) provides the basic example.

On a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) or [Lorentzian manifold](topological-manifold.md#lorentzian-manifold) with [metric tensor](general-relativity.md#metric-tensor) $g$, a smooth [vector field](multivariable-calculus.md#vector-field) $K$ is a [Killing vector field](killing-vector-field.md) when its [Lie derivative](differential-form.md#lie-derivative-of-a-differential-form) of $g$ vanishes. If $\Phi_s$ is its local [flow of a vector field](multivariable-calculus.md#flow-of-a-vector-field), the equivalent statements are

$$
\mathcal L_Kg=0\quad\Longleftrightarrow\quad\Phi_s^*g=g
\quad\Longleftrightarrow\quad\nabla_{(\mu}K_{\nu)}=0.
$$

The middle equality uses the [pullback of a covariant tensor](smooth-manifold.md#pullback-of-a-covariant-tensor): the local flow maps are [isometries](riemannian-geometry.md#isometry) on their domains. The last equality is the [Killing equation](#killing-equation), using the [Levi-Civita connection](general-relativity.md#levi-civita-connection). The infinitesimal condition holds throughout an open domain and integrates to exact local [isometries](riemannian-geometry.md#isometry); it is stronger than making the first [derivatives](calculus.md#derivative) of $g$ vanish at a single point. See [Tong, section 4.3.1, equation (4.29)](https://davidtong.org/pdfs/teaching/general-relativity/gr.pdf#page=167).

For example, on the interval $0<x<1$ with [Euclidean metric](riemannian-metric.md#euclidean-metric) $dx^2$, $K=\partial_x$ translates points by $x\mapsto x+s$. This is a local [isometry](riemannian-geometry.md#isometry), but a point reaches the end of the interval in finite flow parameter. A local [flow of a vector field](multivariable-calculus.md#flow-of-a-vector-field) can be incomplete; see [Killing fields on incomplete manifolds need not generate global isometries](#killing-fields-on-incomplete-manifolds-need-not-generate-global-isometries). The full-plane [translation](geometry-and-topology.md#translation-geometry) and [rotation](riemannian-geometry.md#rotation-mathematics) examples under [Euclidean Killing vector field](#euclidean-killing-vector-field) instead have flows for every real $s$.

**Table of contents**

- [Two-dimensional Killing algebra with a periodic generator is abelian](#two-dimensional-killing-algebra-with-a-periodic-generator-is-abelian)
- [Bochner identity for Killing vector fields](#bochner-identity-for-killing-vector-fields)
- [Killing fields on incomplete manifolds need not generate global isometries](#killing-fields-on-incomplete-manifolds-need-not-generate-global-isometries)
- [Killing transport](#killing-transport)
  - [Dimension bound for Killing vector fields](#dimension-bound-for-killing-vector-fields)
- [Killing field is determined by its value and first covariant derivative](#killing-field-is-determined-by-its-value-and-first-covariant-derivative)
- [Killing-flow four-acceleration](#killing-flow-four-acceleration)
- [Papapetrou electromagnetic field](#papapetrou-electromagnetic-field)
- [Kaluza-Klein decomposition along a Killing field](#kaluza-klein-decomposition-along-a-killing-field)
  - [Kaluza-Klein geodesic Lorentz force](#kaluza-klein-geodesic-lorentz-force)
    - [Sign of the projected Kaluza-Klein Lorentz force](#sign-of-the-projected-kaluza-klein-lorentz-force)
    - [Affine normalization in a Kaluza-Klein geodesic reduction](#affine-normalization-in-a-kaluza-klein-geodesic-reduction)
  - [Heisenberg metric Kaluza-Klein reduction](#heisenberg-metric-kaluza-klein-reduction)
- [Euclidean Killing vector field](#euclidean-killing-vector-field)
  - [Helical orbit of a Euclidean Killing vector](#helical-orbit-of-a-euclidean-killing-vector)
- [Killing equation](#killing-equation)
  - [Killing derivative contraction identity](#killing-derivative-contraction-identity)
  - [Second covariant derivative of a Killing vector](#second-covariant-derivative-of-a-killing-vector)
    - [Curvature-sign convention in Killing derivative identities](#curvature-sign-convention-in-killing-derivative-identities)
    - [Killing vector preserves scalar curvature](#killing-vector-preserves-scalar-curvature)
- [Geodesic conserved quantity from a Killing vector](#geodesic-conserved-quantity-from-a-killing-vector)
  - [Killing energy](#killing-energy)
    - [Killing energy with positive time signature](#killing-energy-with-positive-time-signature)
  - [Charged-particle conserved quantity from a Killing symmetry](#charged-particle-conserved-quantity-from-a-killing-symmetry)
- [Stress-energy current from a Killing vector](#stress-energy-current-from-a-killing-vector)
- [Komar charge](#komar-charge)
  - [Komar current from trace-reversed stress-energy](#komar-current-from-trace-reversed-stress-energy)
  - [Komar angular momentum](#komar-angular-momentum)
    - [Angular momentum conservation in an axisymmetric vacuum region](#angular-momentum-conservation-in-an-axisymmetric-vacuum-region)
    - [Komar angular momentum with inner boundaries](#komar-angular-momentum-with-inner-boundaries)
  - [Komar mass](#komar-mass)
    - [Komar mass normalization in higher dimensions](#komar-mass-normalization-in-higher-dimensions)
    - [Static spherical Komar mass in reciprocal radial gauge](#static-spherical-komar-mass-in-reciprocal-radial-gauge)
  - [Background-subtracted Komar energy](#background-subtracted-komar-energy)

## Two-dimensional Killing algebra with a periodic generator is abelian

↑ **Parent:** [Killing vector field](killing-vector-field.md)

Suppose the full [Lie algebra](lie-algebra.md) of [Killing fields](killing-vector-field.md) has basis $T,\Phi$ and the flow of $\Phi$ has a nonzero period $P$. Write $[T,\Phi]=aT+b\Phi$ with constant coefficients. The [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra) of the periodic flow satisfies $e^{P\operatorname{ad}\Phi}=1$. Its real eigenvalues are $-a$ and zero, so $a=0$. The remaining adjoint operator is nilpotent and its exponential is $1+P\operatorname{ad}\Phi$, forcing $b=0$. This proves commutation from genuine periodic axial symmetry, without differentiating mere asymptotic component limits.

## Bochner identity for Killing vector fields

↑ **Parent:** [Killing vector field](killing-vector-field.md)

On a closed [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), a [Killing vector field](killing-vector-field.md) $X$ satisfies $\nabla^*\nabla X=\operatorname{Ric}^{\sharp}X$ for the nonnegative [rough Laplacian](vector-bundle.md#rough-laplacian). This follows by differentiating $\nabla_iX_j+\nabla_jX_i=0$, contracting and commuting [covariant derivatives](general-relativity.md#covariant-derivative); the contraction also gives $\operatorname{div}X=0$. Taking the [inner product](inner-product.md) with $X$ and using [integration by parts](calculus.md#integration-by-parts) gives the displayed identity. If [Ricci curvature](second-fundamental-form.md#ricci-curvature) is nonpositive, the nonnegative left side must vanish, so $X$ is a [parallel vector field](vector-bundle.md#parallel-vector-field). In particular every [Killing vector field](killing-vector-field.md) on a closed [flat Riemannian manifold](second-fundamental-form.md#flat-manifold) is a [parallel vector field](vector-bundle.md#parallel-vector-field).

## Killing fields on incomplete manifolds need not generate global isometries

↑ **Parent:** [Killing vector field](killing-vector-field.md)

On a geodesically complete [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), every [Killing vector field](killing-vector-field.md) is complete and integrates to a global one-parameter subgroup of its [isometry group](riemannian-geometry.md#isometry-group). On the incomplete interval $(0,1)$ with its Euclidean metric, $\partial_x$ satisfies the [Killing equation](#killing-equation), but translations leave the interval in finite time. The full isometry group is only the identity and reflection. Local solutions of the Killing equation therefore need not equal the Lie algebra of global isometries without completeness.

## Killing transport

↑ **Parent:** [Killing vector field](killing-vector-field.md)

The [Killing equation](#killing-equation) and the [second covariant derivative of a Killing vector](#second-covariant-derivative-of-a-killing-vector) transport a Killing field and its antisymmetric derivative along any curve. Here $L_{ab}=\nabla_b\xi_a$ and the curvature convention is the one in [curvature-sign convention in Killing derivative identities](#curvature-sign-convention-in-killing-derivative-identities). In a parallel frame the equations form a homogeneous linear system of ordinary differential equations. Initial value zero has unique zero continuation. Thus on a connected [pseudo-Riemannian manifold](differential-geometry.md#pseudo-riemannian-manifold), not just on a Riemannian manifold, the field is determined by its value and first derivative at one point.

### Dimension bound for Killing vector fields

↑ **Parent:** [Killing transport](#killing-transport)

On a connected $n$-dimensional [pseudo-Riemannian manifold](differential-geometry.md#pseudo-riemannian-manifold), evaluation of a [Killing vector field](killing-vector-field.md) and its first derivative is injective by [Killing transport](#killing-transport). The value has $n$ components and the [Killing equation](#killing-equation) makes the derivative an antisymmetric two-tensor with $n(n-1)/2$ components. Their sum gives the bound. Flat metrics attain it through $\xi_a=A_a+B_{ab}x^b$ with $B_{ab}=-B_{ba}$. Connectedness is essential for a uniform global bound in terms of $n$: independent fields can be supported on different connected components.

## Killing field is determined by its value and first covariant derivative

↑ **Parent:** [Killing vector field](killing-vector-field.md)

On a [connected](geometry-and-topology.md#connected-space) [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), these data determine a [Killing field](killing-vector-field.md) uniquely, without a completeness assumption. The [second covariant derivative of a Killing vector](#second-covariant-derivative-of-a-killing-vector) makes its restriction to every [geodesic](riemannian-geometry.md#geodesic) a [Jacobi field](riemann-curvature-tensor.md#jacobi-field). The difference of two fields with identical data has zero Jacobi initial values and vanishes in a [convex normal neighborhood](riemannian-geometry.md#convex-normal-neighbourhood). The set on which both its value and [covariant derivative](general-relativity.md#covariant-derivative) vanish is closed by continuity and open by the same local argument, so connectedness makes it the whole manifold.

## Killing-flow four-acceleration

↑ **Parent:** [Killing vector field](killing-vector-field.md)

With [metric signature](topological-manifold.md#metric-signature) $(+---)$, normalize a timelike [Killing vector field](killing-vector-field.md) by $U^a=K^a/N$, $N^2=K^aK_a$. The [Killing equation](#killing-equation) gives $K^b\nabla_bK_a=-\tfrac12\nabla_aN^2$, while $K^b\nabla_bN=0$. Thus the [four-acceleration](special-relativity.md#four-acceleration) of its normalized flow is the displayed gradient. With [metric signature](topological-manifold.md#metric-signature) $(-+++)$ the corresponding lower-index formula has the opposite sign.

## Papapetrou electromagnetic field

↑ **Parent:** [Killing vector field](killing-vector-field.md)

For a [Killing vector field](killing-vector-field.md) $K$, its metric-dual [differential one-form](differential-form.md#one-form) produces the [electromagnetic field](electromagnetism.md#electromagnetic-field) $F_{ab}=2\nabla_{[a}K_{b]}=2\nabla_aK_b$. The [exterior derivative](differential-form.md#exterior-derivative) gives $dF=0$, while the [second covariant derivative of a Killing vector](#second-covariant-derivative-of-a-killing-vector) gives $\nabla^aF_{ab}=-2R_{bd}K^d$. Thus this construction solves the source-free [Maxwell equations](maxwell-equations.md) in a [vacuum spacetime](einstein-field-equations.md#vacuum-spacetime) with zero [cosmological constant](cosmology.md#cosmological-constant). The field is a test field: adding its [stress-energy tensor](stress-energy-tensor.md) would generally change the original [metric tensor](general-relativity.md#metric-tensor).

## Kaluza-Klein decomposition along a Killing field

↑ **Parent:** [Killing vector field](killing-vector-field.md)

Where a [Killing vector field](killing-vector-field.md) is $\partial_x$ and its squared norm $V=h_{xx}$ is nonzero, an invariant [metric tensor](general-relativity.md#metric-tensor) decomposes as $h=V(dx+A)^2+\gamma$. The quotient one-form has $A_i=h_{xi}/V$ and the quotient metric has $\gamma_{ij}=h_{ij}-h_{xi}h_{xj}/V$. All coefficients are independent of $x$. Changing the fibre coordinate to $x'=x+\lambda$ sends $A$ to $A-d\lambda$. A null Killing direction requires a different decomposition.

### Kaluza-Klein geodesic Lorentz force

↑ **Parent:** [Kaluza-Klein decomposition along a Killing field](#kaluza-klein-decomposition-along-a-killing-field)

For $ds_5^2=\gamma_{ij}dx^idx^j+(dz+A_idx^i)^2$ with $z$-independent coefficients, the [geodesic Lagrangian](riemannian-geometry.md#geodesic-lagrangian) makes $k=\dot z+A_i\dot x^i$ constant. Its remaining [Euler-Lagrange equations](analysis.md#euler-lagrange-equation) give the displayed [Lorentz force](relativistic-electromagnetism.md#lorentz-force), where $F=dA$ and $D$ uses the [Levi-Civita connection](general-relativity.md#levi-civita-connection) of $\gamma$. For a particle of five-dimensional mass $M$ with proper-time parameter $s$, the conserved momentum is $p_z=Mk$ and the four-dimensional rest mass is $m=M\sqrt{1+k^2}$. Reparametrizing by four-dimensional proper time gives $Du^i/d\tau=(p_z/m)F^i{}_ju^j$.

#### Sign of the projected Kaluza-Klein Lorentz force

↑ **Parent:** [Kaluza-Klein geodesic Lorentz force](#kaluza-klein-geodesic-lorentz-force)

Take $L=[\eta_{ab}\dot x^a\dot x^b+W^2]/2$ with $W=\dot y+A_a\dot x^a=\xi$ constant. The [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) for $x^a$ is

$$
\eta_{ab}\ddot x^b+\xi(\partial_cA_a-\partial_aA_c)\dot x^c=0.
$$

Thus, with $F_{bc}=\partial_bA_c-\partial_cA_b$,

$$
\ddot x^a=\xi\eta^{ab}(\partial_bA_c-\partial_cA_b)\dot x^c=\xi F^a{}_c\dot x^c.
$$

Reversing the explicit derivative order while retaining this metric and the same definition of $\xi$ changes the equation rather than merely changing a field-tensor naming convention. More generally, a fibre term $\sigma W^2$, $\sigma=\pm1$, gives $\sigma\xi F^a{}_b\dot x^b$; its conserved canonical fibre momentum is $p_y=\sigma\xi$.

In the normalized positive-fibre case with $|\xi|<1$, four-dimensional [proper time](special-relativity.md#proper-time) gives $du^a/d\tau=c\xi F^a{}_bu^b/\sqrt{1-\xi^2}$. This has the [Lorentz force](relativistic-electromagnetism.md#lorentz-force) form. The scale relating the geometrical $A$ to a physical [electromagnetic four-potential](relativistic-electromagnetism.md#electromagnetic-four-potential) fixes the conversion to an SI charge-to-mass ratio.

#### Affine normalization in a Kaluza-Klein geodesic reduction

↑ **Parent:** [Kaluza-Klein geodesic Lorentz force](#kaluza-klein-geodesic-lorentz-force)

For $ds_5^2=\eta_{ab}dx^adx^b+(dy+A_adx^a)^2$, with $A$ independent of $y$, an [affine parameter](riemannian-geometry.md#affine-parameter) $\lambda$ makes $\xi=dy/d\lambda+A_a dx^a/d\lambda$ and the tangent norm $\mathcal N=g_{AB}\dot x^A\dot x^B$ constant. The four-dimensional interval satisfies

$$
du^2=(\mathcal N-\xi^2)d\lambda^2.
$$

Consequently the formula $d\lambda^2=du^2/(1-\xi^2)$ assumes the additional normalization $\mathcal N=1$; affine parametrization alone does not set this value. With base [metric signature](topological-manifold.md#metric-signature) $+---$ and $u=c\tau$, the projected curve is timelike only for $\mathcal N>\xi^2$. The normalized case gives $d\tau/d\lambda=\sqrt{1-\xi^2}/c$. The positive fibre term and the $+---$ base together have two positive directions; the same sign convention must be retained when interpreting the reduction.

### Heisenberg metric Kaluza-Klein reduction

↑ **Parent:** [Kaluza-Klein decomposition along a Killing field](#kaluza-klein-decomposition-along-a-killing-field)

For $h=\alpha dx^2+\beta dy^2+\chi(dz-y\,dx)^2$, the [Kaluza-Klein decomposition along a Killing field](#kaluza-klein-decomposition-along-a-killing-field) $\partial_x$ has $V=\alpha+\chi y^2$, $A=-\chi y\,dz/V$ and $\gamma=\beta dy^2+\alpha\chi\,dz^2/V$. For a [Riemannian metric](riemannian-metric.md), positive constants make the fibre norm and quotient metric positive everywhere.

## Euclidean Killing vector field

↑ **Parent:** [Killing vector field](killing-vector-field.md)

On [Euclidean space](normed-vector-space.md#euclidean-norm), every [Killing vector field](killing-vector-field.md) is a constant [translation](geometry-and-topology.md#translation-geometry) generator plus a constant infinitesimal [rotation](riemannian-geometry.md#rotation-mathematics) generator:

$$
K(\mathbf x)=A+B\mathbf x,\qquad B^T=-B.
$$

Here $A$ is a constant vector and $B$ is an [antisymmetric matrix](linear-algebra.md#skew-symmetric-matrix). The [second covariant derivative of a Killing vector](#second-covariant-derivative-of-a-killing-vector) vanishes for the [Euclidean metric](riemannian-metric.md#euclidean-metric), so the components are affine functions of [Cartesian coordinates](linear-algebra.md#cartesian-coordinate-system); the [Killing equation](#killing-equation) makes the linear coefficient antisymmetric.

In the [Euclidean plane](geometry-and-topology.md#euclidean-plane) with [metric tensor](general-relativity.md#metric-tensor) $g=dx^2+dy^2$, two useful examples are

$$
K_{\mathrm{tr}}=\partial_x,\qquad
K_{\mathrm{rot}}=-y\partial_x+x\partial_y.
$$

The notation $\partial_x$ denotes a [coordinate basis](tangent-vector.md#coordinate-basis) vector; $dx$ denotes a [differential one-form](differential-form.md#one-form). The corresponding [flow of a vector field](multivariable-calculus.md#flow-of-a-vector-field) maps are

$$
\Phi_s^{\mathrm{tr}}(x,y)=(x+s,y),\qquad
\Phi_s^{\mathrm{rot}}(x,y)=(x\cos s-y\sin s,\ x\sin s+y\cos s).
$$

For [translation](geometry-and-topology.md#translation-geometry), all arrows have the same direction and length. For [rotation](riemannian-geometry.md#rotation-mathematics), arrows are tangent to [circles](topology.md#circle), have length $\sqrt{x^2+y^2}$, and vanish at the origin. The [rotation](riemannian-geometry.md#rotation-mathematics) flow keeps $x^2+y^2$ fixed, and its nonstationary [integral curves of a vector field](multivariable-calculus.md#integral-curve-of-a-vector-field) are [circles](topology.md#circle). Both flows preserve the [Euclidean metric](riemannian-metric.md#euclidean-metric). See [Carroll's original notes, section 5, equations (5.45)-(5.46)](https://arxiv.org/pdf/gr-qc/9712019#page=148).

<a id="image-euclidean-killing-vector-fields-translation-arrows-and-straight-flow-orbits-rotation-arrows-and-circular-flow-orbits"></a>
![](killing-vector-translation-and-rotation.png)

**[Figure 1](#image-euclidean-killing-vector-fields-translation-arrows-and-straight-flow-orbits-rotation-arrows-and-circular-flow-orbits). Euclidean Killing vector fields: translation arrows and straight flow orbits, rotation arrows and circular flow orbits**.

The circular [integral curves of a vector field](multivariable-calculus.md#integral-curve-of-a-vector-field) are symmetry orbits, whereas [geodesics](riemannian-geometry.md#geodesic) of the [Euclidean plane](geometry-and-topology.md#euclidean-plane) are straight [lines](euclidean-geometry.md#straight-line). A [Killing vector field](killing-vector-field.md) does not require its own orbits to be [geodesics](riemannian-geometry.md#geodesic). The [geodesic conserved quantity from a Killing vector](#geodesic-conserved-quantity-from-a-killing-vector) pairs the field with the [velocity](classical-mechanics.md#velocity) of a separate [geodesic](riemannian-geometry.md#geodesic); it does not require the [velocity](classical-mechanics.md#velocity) to equal the [Killing vector field](killing-vector-field.md).

### Helical orbit of a Euclidean Killing vector

↑ **Parent:** [Euclidean Killing vector field](#euclidean-killing-vector-field)

An infinitesimal rotation in one coordinate plane plus a constant translation has [integral curves of a vector field](multivariable-calculus.md#integral-curve-of-a-vector-field) that rotate about a shifted centre in that plane and move uniformly in the remaining directions. Nonzero transverse drift gives helices; zero drift gives circles, with zero radius allowing straight or stationary curves.

## Killing equation

↑ **Parent:** [Killing vector field](killing-vector-field.md)

The [Killing equation](#killing-equation) tests whether a candidate [vector field](multivariable-calculus.md#vector-field) generates a local [isometry](riemannian-geometry.md#isometry), without needing to solve for its [flow of a vector field](multivariable-calculus.md#flow-of-a-vector-field). For the [Levi-Civita connection](general-relativity.md#levi-civita-connection) of a [metric tensor](general-relativity.md#metric-tensor) $g$, it is

$$
\nabla_{(\mu}K_{\nu)}=\tfrac12(\nabla_\mu K_\nu+\nabla_\nu K_\mu)=0,
\qquad K_\nu=g_{\nu\rho}K^\rho.
$$

Parentheses mean averaging over the two index orders. The equation says the symmetric part of the [covariant derivative](general-relativity.md#covariant-derivative) vanishes, not that the entire [covariant derivative](general-relativity.md#covariant-derivative) vanishes. The [Lie derivative](differential-form.md#lie-derivative-of-a-differential-form) of the [metric tensor](general-relativity.md#metric-tensor) gives the coordinate form

$$
(\mathcal L_Kg)_{\mu\nu}
=K^\rho\partial_\rho g_{\mu\nu}
+g_{\rho\nu}\partial_\mu K^\rho+g_{\mu\rho}\partial_\nu K^\rho
=\nabla_\mu K_\nu+\nabla_\nu K_\mu.
$$

The last two terms account for how [tangent vectors](tangent-vector.md) move with the field; checking only $K^\rho\partial_\rho g_{\mu\nu}$ misses this. See [Carroll, section 5, equations (5.33) and (5.41)-(5.42)](https://arxiv.org/pdf/gr-qc/9712019#page=147).

For the [Euclidean Killing vector field](#euclidean-killing-vector-field) $K=-y\partial_x+x\partial_y$, the [Euclidean metric](riemannian-metric.md#euclidean-metric) in [Cartesian coordinates](linear-algebra.md#cartesian-coordinate-system) makes [covariant derivatives](general-relativity.md#covariant-derivative) ordinary [partial derivatives](multivariable-calculus.md#partial-derivative). Its diagonal equations give $\partial_xK_x=\partial_yK_y=0$, and its mixed equation gives $\partial_xK_y+\partial_yK_x=1-1=0$. Thus a varying [vector field](multivariable-calculus.md#vector-field) can preserve a constant [metric tensor](general-relativity.md#metric-tensor). In contrast, $K=x\partial_x+y\partial_y$ gives $(\mathcal L_Kg)_{xx}=2$ and fails the [Killing equation](#killing-equation), despite the constant metric components.

If $K=\partial_z$ is a [coordinate basis](tangent-vector.md#coordinate-basis) vector, its components are constant and the coordinate form reduces to $\partial_zg_{\mu\nu}=0$. Hence independence of the metric components from $z$ supplies a [Killing vector field](killing-vector-field.md). This shortcut applies to that coordinate generator, not to an arbitrary varying [vector field](multivariable-calculus.md#vector-field).

### Killing derivative contraction identity

↑ **Parent:** [Killing equation](#killing-equation)

For a [Killing vector field](killing-vector-field.md), set $F_{ab}=\nabla_aK_b$ and $a^s=K^t\nabla_tK^s$. The [Killing equation](#killing-equation) makes $F$ antisymmetric, and expansion of normalized three-index antisymmetrization gives the displayed identity. On a [Killing horizon](general-relativity.md#killing-horizon), [hypersurface orthogonality](differential-geometry.md#hypersurface-orthogonality) removes its first right-hand term and relates $F^{ab}F_{ab}$ to [surface gravity](general-relativity.md#surface-gravity).

### Second covariant derivative of a Killing vector

↑ **Parent:** [Killing equation](#killing-equation)

For a [Killing vector field](killing-vector-field.md) and the curvature convention $[\nabla_\mu,\nabla_\nu]V^\alpha=R^\alpha{}_{\beta\mu\nu}V^\beta$,

$$
\nabla_\nu\nabla_\mu K^\alpha=R^\alpha{}_{\mu\nu\beta}K^\beta,
\qquad
\nabla_\mu\nabla^\mu K^\alpha=-R^\alpha{}_{\beta}K^\beta.
$$

The identity follows by combining the [Ricci identity](riemann-curvature-tensor.md#curvature-commutator-on-a-covariant-tensor), [Killing equation](#killing-equation), and [first Bianchi identity](riemann-curvature-tensor.md#first-bianchi-identity).

#### Curvature-sign convention in Killing derivative identities

↑ **Parent:** [Second covariant derivative of a Killing vector](#second-covariant-derivative-of-a-killing-vector)

Let $C^a{}_{bcd}=\partial_d\Gamma^a_{bc}-\partial_c\Gamma^a_{bd}-\Gamma^a_{ec}\Gamma^e_{bd}+\Gamma^a_{ed}\Gamma^e_{bc}$, with all other index positions obtained by the [metric tensor](general-relativity.md#metric-tensor). This convention is the negative of the convention $[\nabla_c,\nabla_d]V^a=R^a{}_{bcd}V^b$. The [Ricci identity](riemann-curvature-tensor.md#curvature-commutator-on-a-covariant-tensor) is $k_{a;bc}-k_{a;cb}=C_a{}^d{}_{bc}k_d$, with $k_{a;bc}=\nabla_c\nabla_b k_a$. For a [Killing vector](killing-vector-field.md), the [Killing equation](#killing-equation) makes this second derivative antisymmetric in $a,b$. Applying the commutator three times gives $2k_{a;bc}=(C_a{}^d{}_{bc}+C_c{}^d{}_{ba}-C_b{}^d{}_{ac})k_d=-2C_{abc}{}^d k_d$, where the last step uses the [first Bianchi identity](riemann-curvature-tensor.md#first-bianchi-identity). Switching the sign of the [Riemann curvature tensor](riemann-curvature-tensor.md) switches the sign in this identity; moving a raised index by ordinary metric contraction does not switch it.

#### Killing vector preserves scalar curvature

↑ **Parent:** [Second covariant derivative of a Killing vector](#second-covariant-derivative-of-a-killing-vector)

Every [Killing vector field](killing-vector-field.md) $K$ preserves the [scalar curvature](second-fundamental-form.md#scalar-curvature): $\mathcal L_KR=K^\alpha\nabla_\alpha R=0$. One index proof rewrites this derivative as a doubly contracted curvature commutator acting on the antisymmetric tensor $\nabla_{[\mu}K_{\lambda]}$; both terms vanish by symmetry of the [Ricci tensor](riemann-curvature-tensor.md#ricci-tensor).

## Geodesic conserved quantity from a Killing vector

↑ **Parent:** [Killing vector field](killing-vector-field.md)

Each [Killing vector field](killing-vector-field.md) supplies a [conserved quantity](hamiltonian-mechanics.md#conserved-quantity) for freely moving [test particles](classical-mechanics.md#test-particle): it turns a geometric [symmetry](physics.md#symmetry-physics) into a first integral of the [geodesic equation](riemannian-geometry.md#geodesic-equation). Let $\gamma(\lambda)$ be a [geodesic](riemannian-geometry.md#geodesic) with [affine parameter](riemannian-geometry.md#affine-parameter) $\lambda$, [tangent vector](tangent-vector.md) $U^\mu=dx^\mu/d\lambda$, and $\nabla_UU=0$. Wherever a [Killing vector field](killing-vector-field.md) $K$ is defined along the [geodesic](riemannian-geometry.md#geodesic),

$$
C_K=g(K,U)=K_\mu U^\mu,\qquad \frac{dC_K}{d\lambda}=0.
$$

The statement applies to [Riemannian manifolds](riemannian-geometry.md#riemannian-manifold) and to [timelike geodesics](general-relativity.md#timelike-geodesic), [null geodesics](special-relativity.md#null-geodesic) and [spacelike geodesics](riemannian-geometry.md#spacelike-geodesic) in a [Lorentzian manifold](topological-manifold.md#lorentzian-manifold). It requires an [affine parameter](riemannian-geometry.md#affine-parameter); for a massive [test particle](classical-mechanics.md#test-particle), [proper time](special-relativity.md#proper-time) is one choice. See [Tong, section 4.3.2, equation (4.32)](https://davidtong.org/pdfs/teaching/general-relativity/gr.pdf#page=171).

For a worked example in the [Euclidean plane](geometry-and-topology.md#euclidean-plane), take $\gamma(t)=(1+t,2-t)$ with [affine parameter](riemannian-geometry.md#affine-parameter) $t$ and [velocity](classical-mechanics.md#velocity) $U=(1,-1)$. The [Euclidean Killing vector fields](#euclidean-killing-vector-field) for [translation](geometry-and-topology.md#translation-geometry) and [rotation](riemannian-geometry.md#rotation-mathematics) give

$$
C_{\mathrm{tr}}=v_x=1,\qquad
C_{\mathrm{rot}}=xv_y-yv_x=-(1+t)-(2-t)=-3.
$$

The rotational field along the [geodesic](riemannian-geometry.md#geodesic) is $K_{\mathrm{rot}}(\gamma(t))=(t-2,1+t)$: it changes from $(-2,1)$ at $t=0$ to $(-1,2)$ at $t=1$, yet its pairing with $U$ stays $-3$. With toy [mass](classical-mechanics.md#mass) $m=1$ and $t$ interpreted as time, the first constant is the $x$ component of [linear momentum](momentum.md), and the second is the signed $z$ component of [angular momentum](momentum.md#angular-momentum) about the origin. Their numerical values use toy units. The [geodesic](riemannian-geometry.md#geodesic) is straight; the [rotation](riemannian-geometry.md#rotation-mathematics) flow orbits are [circles](topology.md#circle).

<a id="image-one-straight-euclidean-geodesic-the-rotational-killing-field-varies-while-translation-momentum-and-angular-momentum-stay-constant-for-toy-unit-mass"></a>
![](killing-geodesic-conserved-quantity.png)

**[Figure 2](#image-one-straight-euclidean-geodesic-the-rotational-killing-field-varies-while-translation-momentum-and-angular-momentum-stay-constant-for-toy-unit-mass). One straight Euclidean geodesic: the rotational Killing field varies while translation momentum and angular momentum stay constant for toy unit mass**.

This [conservation law](mathematical-physics.md#conservation-law) follows from [metric compatibility](vector-bundle.md#metric-compatibility) and the [Killing equation](#killing-equation):

$$
\frac{d}{d\lambda}(K_\mu U^\mu)
=U^\mu U^\nu\nabla_\mu K_\nu+K_\nu(\nabla_UU)^\nu
=U^\mu U^\nu\nabla_{(\mu}K_{\nu)}=0.
$$

The [geodesic equation](riemannian-geometry.md#geodesic-equation) kills the acceleration term, and the symmetric product $U^\mu U^\nu$ selects the vanishing symmetric derivative. This [tensor contraction](multilinear-algebra.md#tensor-contraction) is the whole proof outline; see [Carroll, equation (5.43)](https://arxiv.org/pdf/gr-qc/9712019#page=147).

In a [stationary spacetime](general-relativity.md#stationary-spacetime), a chosen time-translation [Killing vector field](killing-vector-field.md) $K$ gives [Killing energy](#killing-energy). With [metric signature](topological-manifold.md#metric-signature) $(-+++)$, $c=1$, and a massive [test particle](classical-mechanics.md#test-particle)'s [four-momentum](special-relativity.md#four-momentum) $p^\mu=mU^\mu$, the physical normalization is

$$
E=-p_\mu K^\mu,\qquad L_z=p_\mu\Phi^\mu.
$$

Here $\Phi$ generates the axial [rotational symmetry](linear-algebra.md#rotational-symmetry) when one exists. In coordinates with $K=\partial_t$ and $\Phi=\partial_\phi$, these are $E=-p_t$ and $L_z=p_\phi$. Both are [conserved quantities](hamiltonian-mechanics.md#conserved-quantity) along the [geodesic](riemannian-geometry.md#geodesic), even if the metric has a time-angle cross term. A future timelike $K$ makes $E$ positive for a future massive particle; the scale of $E$ depends on the normalization of $K$. Not every [spacetime](special-relativity.md#spacetime) has a global timelike [Killing vector field](killing-vector-field.md), and a stationary field can become spacelike in an [ergoregion of a stationary spacetime](general-relativity.md#ergoregion-of-a-stationary-spacetime). Conservation on the field's domain does not imply a universal global positive [energy](energy.md); see [Tong, sections 4.3.1-4.3.2 on the timelike-domain qualification and conserved charges](https://davidtong.org/pdfs/teaching/general-relativity/gr.pdf#page=170).

### Killing energy

↑ **Parent:** [Geodesic conserved quantity from a Killing vector](#geodesic-conserved-quantity-from-a-killing-vector)

For a geodesic tangent $u$ and a stationary [Killing vector field](killing-vector-field.md) $K$, the [Killing energy](#killing-energy) is $E=-g(K,u)$. It is conserved along the [geodesic](riemannian-geometry.md#geodesic). When $K$ is future timelike and $u$ is future causal, $E>0$ for a nonzero tangent; it need not be positive where $K$ becomes spacelike.

#### Killing energy with positive time signature

↑ **Parent:** [Killing energy](#killing-energy)

With [metric signature](topological-manifold.md#metric-signature) $(+---)$ and a future timelike stationary [Killing vector](killing-vector-field.md) $K$, positive [energy](energy.md) is $E=g(P,K)$ for future physical momentum $P$. A common $(-+++)$ convention instead uses $-g(P,K)$. The normalization of $K$ fixes the observer or asymptotic time scale.

### Charged-particle conserved quantity from a Killing symmetry

↑ **Parent:** [Geodesic conserved quantity from a Killing vector](#geodesic-conserved-quantity-from-a-killing-vector)

Suppose $V$ is a [Killing vector field](killing-vector-field.md), $F$ is an [electromagnetic field tensor](relativistic-electromagnetism.md#electromagnetic-field-tensor) satisfying $dF=0$ and $\mathcal L_VF=0$, and a particle of nonzero mass $m$ obeys the [Lorentz force](relativistic-electromagnetism.md#lorentz-force) equation $\nabla_uu=(q/m)F^a{}_bu^b$. [Cartan's magic formula](differential-form.md#cartan-s-magic-formula) gives $d(\iota_VF)=0$, so the [local potential of a closed differential one-form](differential-form.md#local-potential-of-a-closed-differential-one-form) proof gives $d\Phi=\iota_VF$ locally. The [Killing equation](#killing-equation) eliminates $u^au^b\nabla_aV_b$, and the force term gives $d(V\cdot u)/d\tau=(q/m)d\Phi/d\tau$. Therefore $mV\cdot u-q\Phi$ is locally conserved. The sign assumes contraction in the first argument of $F$. A global potential additionally requires the closed one-form to have zero periods; invariance alone is insufficient without the homogeneous [Maxwell equations](maxwell-equations.md).

## Stress-energy current from a Killing vector

↑ **Parent:** [Killing vector field](killing-vector-field.md)

If $T^{ab}$ is symmetric and covariantly conserved and $K$ is a [Killing vector field](killing-vector-field.md), then $J^a=T^a{}_bK^b$ is conserved. Its flux through a spacelike hypersurface is the energy or momentum charge generated by the isometry.

## Komar charge

↑ **Parent:** [Killing vector field](killing-vector-field.md)

A Komar integral constructs a conserved gravitational charge from the exterior derivative of the one-form dual to a Killing vector. In four dimensions, a stationary mass is conventionally normalized as

$$
M_K=-\frac1{8\pi}\int_S\star dk.
$$

### Komar current from trace-reversed stress-energy

↑ **Parent:** [Komar charge](#komar-charge)

A [Killing vector field](killing-vector-field.md) gives an antisymmetric tensor $\nabla^\mu\xi^\nu$ whose divergence is this current, up to overall surface-orientation convention. The four-dimensional [Einstein field equations](einstein-field-equations.md) express it as $8\pi G(T^\mu{}_\nu-\tfrac12T\delta^\mu{}_\nu)\xi^\nu$ at zero cosmological constant. The [contracted Bianchi identity](riemann-curvature-tensor.md#contracted-bianchi-identity) and Killing invariance of [scalar curvature](second-fundamental-form.md#scalar-curvature) prove its divergence is zero. Stress conservation alone does not cancel the trace derivative without Killing invariance of the trace.

### Komar angular momentum

↑ **Parent:** [Komar charge](#komar-charge)

[Komar angular momentum](#komar-angular-momentum) is the [Komar charge](#komar-charge) associated with an axial [Killing vector field](killing-vector-field.md) in four-dimensional [general relativity](general-relativity.md). In geometrized units its normalization is $(16\pi)^{-1}\int_S\star dm$, where $m$ is the metric-dual [differential one-form](differential-form.md#one-form). With zero [cosmological constant](cosmology.md#cosmological-constant), vacuum [Einstein field equations](einstein-field-equations.md) make $d\star dm=0$, so homologous surrounding surfaces in the vacuum region give the same charge.

#### Angular momentum conservation in an axisymmetric vacuum region

↑ **Parent:** [Komar angular momentum](#komar-angular-momentum)

For an axial [Killing vector](killing-vector-field.md) $\xi$ and zero [cosmological constant](cosmology.md#cosmological-constant), set $F^{ab}=\nabla^b\xi^a$. The [Killing equation](#killing-equation) and [Ricci identity](riemann-curvature-tensor.md#curvature-commutator-on-a-covariant-tensor) give $\nabla_bF^{ab}=-R^a{}_b\xi^b$. In a vacuum region this vanishes, so [Stokes theorem](multivariable-calculus.md#stokes-theorem) makes the [Komar angular momentum](#komar-angular-momentum) equal on homologous enclosing surfaces. The region may contain [gravitational waves](gravitational-wave.md) with nonzero Weyl curvature: Ricci flatness, rather than complete flatness, is what removes the flux. This proves absence of axial angular-momentum transport by exactly axisymmetric gravitational radiation, without assuming that a radiating spacetime is stationary.

#### Komar angular momentum with inner boundaries

↑ **Parent:** [Komar angular momentum](#komar-angular-momentum)

With zero [cosmological constant](cosmology.md#cosmological-constant) and the component [Hodge star operator](differential-form.md#hodge-star-operator) convention $(\star j)_{abc}=\epsilon_{abcd}j^d$, the [Einstein field equations](einstein-field-equations.md) and [Killing equation](#killing-equation) give $d\star dm=-16\pi\star(T_{ab}m^b-\tfrac12Tm_a)$. If $m$ is tangent to a spacelike [hypersurface](smooth-manifold.md#hypersurface), the trace term pulls back to zero. For $\partial\Sigma=S_\infty-\bigcup_iS_i$, [Stokes theorem](multivariable-calculus.md#stokes-theorem) yields

$$
J_\infty-\sum_iJ_i=-\int_\Sigma\star(T_{ab}m^b\,dx^a).
$$

The inner [Komar charges](#komar-charge) cannot be dropped for a vacuum [Kerr black hole](black-hole.md#kerr-black-hole), whose [angular momentum](momentum.md#angular-momentum) is nonzero although its [stress-energy tensor](stress-energy-tensor.md) vanishes. A matter-only volume formula requires a regular filling with no inner boundaries.

### Komar mass

↑ **Parent:** [Komar charge](#komar-charge)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Komar_mass)

Komar mass is the [Komar charge](#komar-charge) associated with a stationary timelike Killing vector, using the normalization appropriate to gravitational mass.

#### Komar mass normalization in higher dimensions

↑ **Parent:** [Komar mass](#komar-mass)

For future static-slice normal $u$ and outward radial normal $n$, take $d\Sigma_{ab}=(n_au_b-n_bu_a)dA$, with both antisymmetric components summed. For the [Schwarzschild-Tangherlini metric](black-hole.md#schwarzschild-tangherlini-metric) the flux is $-\Omega_{D-2}r^{D-2}f'=-(D-3)\Omega_{D-2}\mu$. The displayed dimension-dependent coefficient then reproduces the [ADM mass](general-relativity.md#arnowitt-deser-misner-mass). Reversing orientation reverses the flux; including a factor of one-half in the binormal convention also changes its numerical value. A four-dimensional normalization cannot be carried unchanged into other dimensions.

#### Static spherical Komar mass in reciprocal radial gauge

↑ **Parent:** [Komar mass](#komar-mass)

For $ds^2=-f(r)dt^2+dr^2/f(r)+R(r)^2d\Omega^2$ and $K=\partial_t$ normalized at infinity, the [Komar mass](#komar-mass) on a round sphere is $R^2f'/(2G)$. The future unit normal to a static slice is $f^{-1/2}K$, and the outward unit radial normal is $f^{1/2}\partial_r$; their contraction with $\nabla_aK_b$ gives $f'/2$, whose integral over the sphere yields the formula. The asymptotic mass is its limit at infinity. In the presence of matter, the finite-radius integral need not be constant.

### Background-subtracted Komar energy

↑ **Parent:** [Komar charge](#komar-charge)

For a spacetime with a non-flat reference background, replacing $k$ by $k-\bar k$ removes the background contribution and can make the Komar surface integral finite.

## ↑ Ancestors (4)

1. [General relativity](general-relativity.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (135)

- [Axisymmetric radiation carries no axial angular momentum](gravitational-wave.md#axisymmetric-radiation-carries-no-axial-angular-momentum)
- [Bifurcate Killing horizon](general-relativity.md#bifurcate-killing-horizon)
- [Black-hole rigidity theorem](black-hole.md#black-hole-rigidity-theorem)
- [Bochner identity for Killing vector fields](#bochner-identity-for-killing-vector-fields)
- [Charged-particle conserved quantity from a Killing symmetry](#charged-particle-conserved-quantity-from-a-killing-symmetry)
- [Coordinate invariance of the Schwarzschild photon radial potential](schwarzschild-spacetime.md#coordinate-invariance-of-the-schwarzschild-photon-radial-potential)
- [Dimension bound for Killing vector fields](#dimension-bound-for-killing-vector-fields)
- [Eisenhart-Duval lift](classical-mechanics.md#eisenhart-duval-lift)
- [Ergoregion of a stationary spacetime](general-relativity.md#ergoregion-of-a-stationary-spacetime)
- [Euclidean Killing vector field](#euclidean-killing-vector-field)
- [Geodesic conserved quantity from a Killing vector](#geodesic-conserved-quantity-from-a-killing-vector)
- [Hydrostatic equilibrium along a Killing vector](stress-energy-tensor.md#hydrostatic-equilibrium-along-a-killing-vector)
- [Ingoing Kerr coordinates](black-hole.md#ingoing-kerr-coordinates)
- [Isometry dimension of a compact flat manifold](second-fundamental-form.md#isometry-dimension-of-a-compact-flat-manifold)
- [Kaluza-Klein decomposition along a Killing field](#kaluza-klein-decomposition-along-a-killing-field)
- [Kerr horizon angular velocity](black-hole.md#kerr-horizon-angular-velocity)
- [Kerr stationary-limit surface is generically timelike](black-hole.md#kerr-stationary-limit-surface-is-generically-timelike)
- [Killing derivative contraction identity](#killing-derivative-contraction-identity)
- [Killing energy](#killing-energy)
- [Killing equation](#killing-equation)
- [Killing fields on incomplete manifolds need not generate global isometries](#killing-fields-on-incomplete-manifolds-need-not-generate-global-isometries)
- [Killing-flow four-acceleration](#killing-flow-four-acceleration)
- [Killing frame for a right-invariant Heisenberg metric](lie-algebra.md#killing-frame-for-a-right-invariant-heisenberg-metric)
- [Killing horizon](general-relativity.md#killing-horizon)
- [Killing tensor](riemannian-geometry.md#killing-tensor)
- [Killing vector field](killing-vector-field.md)
- [Killing vector preserves scalar curvature](#killing-vector-preserves-scalar-curvature)
- [Komar angular momentum](#komar-angular-momentum)
- [Komar current from trace-reversed stress-energy](#komar-current-from-trace-reversed-stress-energy)
- [Lie derivative of an affine connection](general-relativity.md#lie-derivative-of-an-affine-connection)
- [Nonstationary spacetime](general-relativity.md#nonstationary-spacetime)
- [Normalized Killing one-form](differential-geometry.md#normalized-killing-one-form)
- [Papapetrou electromagnetic field](#papapetrou-electromagnetic-field)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-72.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-72.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-73.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-73.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-56.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-19.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-55.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-62.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-62.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-63.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-64.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2.md#35a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-63.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-63.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-63.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-66.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-66.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-66.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-56.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-56.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-56.md#1/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-56.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-56.md#2/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-56.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-58.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-60.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#36b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-52.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#1/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#1/a/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#2/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#4/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#4/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#4/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-58.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-58.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-58.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-58.md#section-i/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-58.md#section-i/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-51.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-52.md#3/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-52.md#3/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-52.md#3/b/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-52.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1.md#35d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1.md#35d/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-52.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-52.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-54.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-54.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-54.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-54.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-56.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-311.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-309.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-309.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-311.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-311.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-311.md#3/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-309.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-311.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-311.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-309.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-311.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-311.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-309.md#4/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-311.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-309.md#2/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-311.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-311.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-311.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-309.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-311.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-311.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-309.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-309.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-311.md#3/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-313.md#3/d/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2012/paper-1.md#4/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2021.md#section-a/1/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2021.md#section-b/4/b/solution)
- [Planar warped spacetime](general-relativity.md#planar-warped-spacetime)
- [Radiation fluid has no regular free surface](stress-energy-tensor.md#radiation-fluid-has-no-regular-free-surface)
- [Rank-two Killing tensor](riemannian-geometry.md#rank-two-killing-tensor)
- [Reissner-Nordstrom horizon surface gravity](black-hole.md#reissner-nordstrom-horizon-surface-gravity)
- [Right-invariant Riemannian metric](lie-theory.md#right-invariant-riemannian-metric)
- [Schwarzschild surface gravity](general-relativity.md#schwarzschild-surface-gravity)
- [Second covariant derivative of a Killing vector](#second-covariant-derivative-of-a-killing-vector)
- [Signed surface gravity of a de Sitter horizon](general-relativity.md#signed-surface-gravity-of-a-de-sitter-horizon)
- [Stationary radiation density](stress-energy-tensor.md#stationary-radiation-density)
- [Stress-energy current from a Killing vector](#stress-energy-current-from-a-killing-vector)
- [Surface gravity](general-relativity.md#surface-gravity)
- [Timelike geodesics of a quadratic-time conformal metric](general-relativity.md#timelike-geodesics-of-a-quadratic-time-conformal-metric)
- [Timelike vector field](general-relativity.md#timelike-vector-field)
- [Tolman–Ehrenfest relation](thermal-equilibrium.md#tolman-ehrenfest-relation)
