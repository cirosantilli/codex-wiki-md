# Geodesic congruence

↑ **Parent:** [General relativity](general-relativity.md)

A geodesic congruence is a family of nonintersecting geodesics filling an open spacetime region. Its derivative tensor describes the relative motion of neighboring geodesics.

Requiring each member to be a [geodesic](riemannian-geometry.md#geodesic) specializes a [congruence of curves in general relativity](general-relativity.md#congruence-general-relativity).

**Table of contents**

- [Timelike geodesic vector field](#timelike-geodesic-vector-field)
  - [Spatial projector of a timelike congruence](#spatial-projector-of-a-timelike-congruence)
  - [Deformation tensor of a timelike geodesic congruence](#deformation-tensor-of-a-timelike-geodesic-congruence)
    - [Kinematic decomposition of a timelike geodesic congruence](#kinematic-decomposition-of-a-timelike-geodesic-congruence)
    - [Riccati equation for a timelike geodesic congruence](#riccati-equation-for-a-timelike-geodesic-congruence)
  - [Expansion scalar](#expansion-scalar)
  - [Shear tensor of a timelike congruence](#shear-tensor-of-a-timelike-congruence)
  - [Vorticity tensor of a timelike congruence](#vorticity-tensor-of-a-timelike-congruence)
  - [Focal point of a hypersurface](#focal-point-of-a-hypersurface)
- [Timelike geodesic completeness](#timelike-geodesic-completeness)
  - [Timelike geodesic incompleteness](#timelike-geodesic-incompleteness)
- [Null geodesic congruence](#null-geodesic-congruence)
  - [Optical matrix of a null congruence](#optical-matrix-of-a-null-congruence)
    - [Sachs optical equations](#sachs-optical-equations)
  - [Parallel null partner for ingoing Schwarzschild rays](#parallel-null-partner-for-ingoing-schwarzschild-rays)
  - [Affine rescaling of a null normal](#affine-rescaling-of-a-null-normal)
  - [Parallel auxiliary null vector](#parallel-auxiliary-null-vector)
  - [Null-gradient affine-geodesic identity](#null-gradient-affine-geodesic-identity)
  - [Screen-space projector](#screen-space-projector)
    - [Optical tensor](#optical-tensor)
      - [Null expansion](#null-expansion)
        - [Spherical null expansion in ingoing coordinates](#spherical-null-expansion-in-ingoing-coordinates)
        - [Spherical null expansions in double-null coordinates](#spherical-null-expansions-in-double-null-coordinates)
          - [Double-null focusing identity](#double-null-focusing-identity)
            - [Persistence of spherical trapping](#persistence-of-spherical-trapping)
      - [Null shear](#null-shear)
        - [Null-shear propagation equation](#null-shear-propagation-equation)
      - [Null twist](#null-twist)
        - [Null twist vanishes exactly for hypersurface-orthogonal geodesics](#null-twist-vanishes-exactly-for-hypersurface-orthogonal-geodesics)
        - [Null-twist propagation equation](#null-twist-propagation-equation)
  - [Null Raychaudhuri equation](#null-raychaudhuri-equation)
    - [Area-square-root optical focusing equation](#area-square-root-optical-focusing-equation)
      - [Flat-space anisotropic beam shear focusing](#flat-space-anisotropic-beam-shear-focusing)
    - [Null focusing theorem](#null-focusing-theorem)
      - [Conjugate point to a spacelike surface](#conjugate-point-to-a-spacelike-surface)

## Timelike geodesic vector field

↑ **Parent:** [Geodesic congruence](geodesic-congruence.md)

A timelike geodesic vector field is a smooth unit timelike field $u^a$ whose integral curves obey $u^b\nabla_bu^a=0$. Its [expansion scalar](#expansion-scalar), [shear tensor of a timelike congruence](#shear-tensor-of-a-timelike-congruence), and [vorticity tensor of a timelike congruence](#vorticity-tensor-of-a-timelike-congruence) evolve according to the timelike [Raychaudhuri equation](cosmology.md#friedmann-acceleration-equation).

### Spatial projector of a timelike congruence

↑ **Parent:** [Timelike geodesic vector field](#timelike-geodesic-vector-field)

For a unit timelike vector field $u^au_a=-1$, the tensor $h_{ab}=g_{ab}+u_au_b$ projects onto the three-dimensional subspace orthogonal to $u^a$. In particular, $h_{ab}u^a=h_{ab}u^b=0$ and $g^{ab}h_{ab}=3$ in four spacetime dimensions.

### Deformation tensor of a timelike geodesic congruence

↑ **Parent:** [Timelike geodesic vector field](#timelike-geodesic-vector-field)

For a unit geodesic vector field $u^a$, differentiation of $u^au_a=-1$ and the geodesic equation show that $B_{ab}u^a=B_{ab}u^b=0$. The tensor therefore acts entirely in the local rest space.

#### Kinematic decomposition of a timelike geodesic congruence

↑ **Parent:** [Deformation tensor of a timelike geodesic congruence](#deformation-tensor-of-a-timelike-geodesic-congruence)

In four spacetime dimensions, the deformation tensor decomposes as

$$
B_{ab}=\frac13\theta h_{ab}+\sigma_{ab}+\omega_{ab},
$$

where $\theta=B^{ab}h_{ab}$ is the [expansion scalar](#expansion-scalar), $\sigma_{ab}=B_{(ab)}-\theta h_{ab}/3$ is the symmetric trace-free [shear tensor of a timelike congruence](#shear-tensor-of-a-timelike-congruence), and $\omega_{ab}=B_{[ab]}$ is the [vorticity tensor of a timelike congruence](#vorticity-tensor-of-a-timelike-congruence).

#### Riccati equation for a timelike geodesic congruence

↑ **Parent:** [Deformation tensor of a timelike geodesic congruence](#deformation-tensor-of-a-timelike-geodesic-congruence)

With the curvature convention $[\nabla_\mu,\nabla_\beta]X_\alpha=-R^\rho{}_{\alpha\mu\beta}X_\rho$, the deformation tensor along a unit timelike geodesic field satisfies

$$
X^\mu\nabla_\mu B_{\alpha\beta}
=-B^\mu{}_{\beta}B_{\alpha\mu}
+R_{\mu\beta\alpha}{}^\nu X^\mu X_\nu.
$$

Taking its spatial trace and inserting the [kinematic decomposition of a timelike geodesic congruence](#kinematic-decomposition-of-a-timelike-geodesic-congruence) leads to the timelike [Raychaudhuri equation](cosmology.md#friedmann-acceleration-equation).

### Expansion scalar

↑ **Parent:** [Timelike geodesic vector field](#timelike-geodesic-vector-field)

The expansion scalar of a unit timelike congruence with tangent $u^a$ is $\theta=\nabla_au^a$. It gives the fractional rate of change of an infinitesimal comoving spatial volume.

### Shear tensor of a timelike congruence

↑ **Parent:** [Timelike geodesic vector field](#timelike-geodesic-vector-field)

The shear tensor is the symmetric trace-free spatial part of $\nabla_bu_a$. It changes the shape of an infinitesimal comoving volume without changing that volume to first order.

### Vorticity tensor of a timelike congruence

↑ **Parent:** [Timelike geodesic vector field](#timelike-geodesic-vector-field)

The vorticity tensor is the antisymmetric spatial part of $\nabla_bu_a$. It vanishes exactly when the timelike congruence is locally hypersurface orthogonal.

### Focal point of a hypersurface

↑ **Parent:** [Timelike geodesic vector field](#timelike-geodesic-vector-field)

A focal point of a hypersurface along an orthogonal geodesic is a point where a nonzero normal [Jacobi field](general-relativity.md#jacobi-field) arising from variations of the initial point vanishes. Beyond the first focal point, that geodesic no longer locally maximizes proper time from a spacelike initial hypersurface.

## Timelike geodesic completeness

↑ **Parent:** [Geodesic congruence](geodesic-congruence.md)

A spacetime is timelike-geodesically complete when every inextendible affinely parametrized timelike geodesic has proper time extending without a finite endpoint in both directions.

### Timelike geodesic incompleteness

↑ **Parent:** [Timelike geodesic completeness](#timelike-geodesic-completeness)

Timelike geodesic incompleteness means that at least one inextendible timelike geodesic reaches an endpoint after finite proper time. Singularity theorems commonly establish this conclusion without asserting that curvature diverges.

## Null geodesic congruence

↑ **Parent:** [Geodesic congruence](geodesic-congruence.md)

A null geodesic congruence has an affinely parametrized null tangent $k^a$ satisfying $k^ak_a=0$ and $k^b\nabla_bk^a=0$.

### Optical matrix of a null congruence

↑ **Parent:** [Null geodesic congruence](#null-geodesic-congruence)

For affine null tangent $U$, choose an auxiliary null vector $N$ with $U\cdot N=-1$ and parallel transport it along the rays. The screen-space projector is $P_{ab}=g_{ab}+U_aN_b+N_aU_b$. The [optical matrix of a null congruence](#optical-matrix-of-a-null-congruence) describes evolution of screen-projected deviation vectors. Its trace is the null expansion, its symmetric trace-free part is the null shear, and its antisymmetric part is the null twist. In four dimensions $\widehat B=\theta P/2+\widehat\sigma+\widehat\omega$.

#### Sachs optical equations

↑ **Parent:** [Optical matrix of a null congruence](#optical-matrix-of-a-null-congruence)

For a parallel-transported screen and affine null geodesic tangent $U$, the optical matrix satisfies

$$
U^c\nabla_c\widehat B_{ab}=-\widehat B_{ac}\widehat B^c{}_b-P_a{}^eP_b{}^fR_{cedf}U^cU^d.
$$

Its trace gives the null Raychaudhuri equation. In a two-dimensional screen, symmetric trace-free matrices have scalar squares and anticommute with antisymmetric matrices. The trace-free symmetric and antisymmetric parts consequently yield the null shear and twist transport equations without additional quadratic trace-free terms.

### Parallel null partner for ingoing Schwarzschild rays

↑ **Parent:** [Null geodesic congruence](#null-geodesic-congruence)

In the [Ingoing Eddington-Finkelstein coordinates](general-relativity.md#ingoing-eddington-finkelstein-coordinates) metric $ds^2=-f(r)dv^2+2dv\,dr+r^2d\Omega^2$, where $f=1-2M/r$, the tangent $U=-E\partial_r$ is affine when $E>0$ is constant along each ray. The displayed radial partner obeys $N^2=0$ and $U\cdot N=-1$. Since $\Gamma^v{}_{rv}=\Gamma^a{}_{rr}=0$ and $\Gamma^r{}_{rv}=-f'/2$, its derivative $\partial_rN^r=f'/(2E)$ cancels the connection term, giving $\nabla_UN=0$. Its screen is the angular two-plane, with [optical tensor](#optical-tensor) $\widehat B_{AB}=-Er\gamma_{AB}$, [null expansion](#null-expansion) $-2E/r$, and zero [null shear](#null-shear) and [null twist](#null-twist).

### Affine rescaling of a null normal

↑ **Parent:** [Null geodesic congruence](#null-geodesic-congruence)

If a [null vector](special-relativity.md#null-vector) tangent satisfies $\nabla_KK=\kappa K$, then $U=hK$ is affine when $K(\log h)=-\kappa$. Choose $h=1$ on the initial transverse surface. The [screen-space projector](#screen-space-projector) kills derivative terms proportional to $K$, so the initial [optical tensor](#optical-tensor) and its [null expansion](#null-expansion) agree with those of $K$. In ingoing spherical coordinates, $K=\partial_v+(f/2)\partial_r$ has $\kappa=f'/2$.

### Parallel auxiliary null vector

↑ **Parent:** [Null geodesic congruence](#null-geodesic-congruence)

For an affine [null geodesic congruence](#null-geodesic-congruence) with future tangent $U$, choose a future unit [timelike vector](general-relativity.md#timelike-vector) $T$ on a transverse section, put $E=-U\cdot T$, and set $N=T/E-U/(2E^2)$ there. It has $N^2=0$ and $U\cdot N=-1$. [Parallel transport](fiber-bundle.md#parallel-transport) along each generator preserves these contractions by metric compatibility and $\nabla_UU=0$. The construction is local up to caustics and supplies the auxiliary normal for a [screen-space projector](#screen-space-projector).

### Null-gradient affine-geodesic identity

↑ **Parent:** [Null geodesic congruence](#null-geodesic-congruence)

If $k_a=\nabla_aS$ is a null gradient, symmetry of the Hessian gives $k^a\nabla_ak_b=k^a\nabla_bk_a=\tfrac12\nabla_b(k^2)=0$. Its integral curves are therefore affinely parametrized [null geodesics](special-relativity.md#null-geodesic), rather than merely null curves with a nonaffinity term.

### Screen-space projector

↑ **Parent:** [Null geodesic congruence](#null-geodesic-congruence)

Given null vectors $k$ and $n$ with $k\mathbin\cdot n=-1$, the screen-space projector is

$$
P^a{}_b=\delta^a_b+k^an_b+n^ak_b.
$$

It annihilates $k$ and $n$ and, in $D$ spacetime dimensions, projects onto the $(D-2)$-dimensional spacelike space transverse to them.

#### Optical tensor

↑ **Parent:** [Screen-space projector](#screen-space-projector)

For $B_{ab}=\nabla_bk_a$, the optical tensor is the screen projection $\widehat B_{ab}=P_a{}^cP_b{}^dB_{cd}$. Its trace, symmetric trace-free part, and antisymmetric part are the expansion, shear, and twist of the null congruence.

##### Null expansion

↑ **Parent:** [Optical tensor](#optical-tensor)

The null expansion is $\theta=P^{ab}\widehat B_{ab}$. It is the logarithmic derivative of an infinitesimal transverse area: $\theta=A^{-1}dA/d\lambda$.

###### Spherical null expansion in ingoing coordinates

↑ **Parent:** [Null expansion](#null-expansion)

For a four-dimensional spherical metric $ds^2=-f\,dv^2+2\,dv\,dr+r^2d\Omega^2$, a radial [null vector](special-relativity.md#null-vector) normal $K$ to a round sphere has [null expansion](#null-expansion) $\theta_K=\tfrac12q^{AB}\mathcal L_Kq_{AB}=2K(r)/r$, where $q_{AB}=r^2\gamma_{AB}$. The angular metric changes only by a common scale, so radial congruences have zero [null shear](#null-shear); hypersurface orthogonality also gives zero [null twist](#null-twist). The convention here is the trace, not the screen-averaged expansion.

###### Spherical null expansions in double-null coordinates

↑ **Parent:** [Null expansion](#null-expansion)

For a four-dimensional spherically symmetric metric $ds^2=-2f\,dU\,dV+r^2d\Omega^2$, the affine null gradients are $f^{-1}\partial_V$ and $f^{-1}\partial_U$. Their [null expansions](#null-expansion) are $2r_{,V}/(fr)$ and $2r_{,U}/(fr)$. Their [null shear](#null-shear) and [null twist](#null-twist) vanish because the transverse metric changes only by a common scale and the covectors are exact gradients.

###### Double-null focusing identity

↑ **Parent:** [Spherical null expansions in double-null coordinates](#spherical-null-expansions-in-double-null-coordinates)

The [Null Raychaudhuri equation](#null-raychaudhuri-equation) and [Einstein field equations](general-relativity.md#einstein-field-equations) give $\partial_U(f^{-1}r_{,U})=-rR_{UU}/(2f)=-4\pi rT_{UU}/f$, with an exchanged-coordinate identity in $V$. Under the [null energy condition](general-relativity.md#null-energy-condition), each rescaled radial derivative is nonincreasing along its corresponding future null direction.

###### Persistence of spherical trapping

↑ **Parent:** [Double-null focusing identity](#double-null-focusing-identity)

In a regular double-null region satisfying the [null energy condition](general-relativity.md#null-energy-condition), an initially negative $r_{,U}$ on a [Cauchy hypersurface](general-relativity.md#cauchy-surface) remains negative in its [future domain of dependence](general-relativity.md#future-domain-of-dependence). If both spherical [null expansions](#null-expansion) are negative at one sphere, the exchanged-coordinate focusing inequality preserves the other sign along its future outgoing null direction. Every later sphere that still exists there remains a [trapped surface](general-relativity.md#trapped-surface).

##### Null shear

↑ **Parent:** [Optical tensor](#optical-tensor)

The null shear is the symmetric trace-free part $\widehat\sigma_{ab}=\widehat B_{(ab)}-\theta P_{ab}/(D-2)$. It changes the shape of a transverse beam while preserving its area to first order.

###### Null-shear propagation equation

↑ **Parent:** [Null shear](#null-shear)

For an affine null congruence in four spacetime dimensions with a parallel-transported screen, the displayed equation follows by taking the symmetric trace-free part of the Sachs optical equations. The Ricci contribution to the optical tidal tensor is $P_{ab}R_{cd}U^cU^d/2$, so it changes the expansion but contributes no screen-trace-free source. The projected Weyl tensor supplies the tidal source of shear.

##### Null twist

↑ **Parent:** [Optical tensor](#optical-tensor)

The null twist is $\widehat\omega_{ab}=\widehat B_{[ab]}$. It vanishes for null generators orthogonal to a hypersurface by the [Frobenius theorem](differential-geometry.md#frobenius-theorem).

###### Null twist vanishes exactly for hypersurface-orthogonal geodesics

↑ **Parent:** [Null twist](#null-twist)

For an affine [null geodesic congruence](#null-geodesic-congruence), $B_{ab}=\nabla_bU_a$ annihilates $U$ in both slots. Relative to a null partner, its antisymmetric part is its screen projection plus a term of the form $U_{[a}q_{b]}$. Hence zero [null twist](#null-twist) implies $U\wedge dU=0$, and [Frobenius theorem](differential-geometry.md#frobenius-theorem) makes $U_a$ locally proportional to a hypersurface gradient. Conversely, if $U_a=h\nabla_aS$, its antisymmetric derivative has a factor of $U$, so the screen projection vanishes. Geodesicity is essential to the converse from vanishing screen twist to the full Frobenius condition.

###### Null-twist propagation equation

↑ **Parent:** [Null twist](#null-twist)

For an affinely parametrized four-dimensional [null geodesic congruence](#null-geodesic-congruence), the screen-projected evolution of the [null twist](#null-twist) is

$$
k^c\nabla_c\widehat\omega_{ab}
=-\theta\widehat\omega_{ab}
+2\widehat\sigma_{c[a}\widehat\omega_{b]}{}^c.
$$

Consequently zero twist remains zero along every generator on which the optical description remains regular.

### Null Raychaudhuri equation

↑ **Parent:** [Null geodesic congruence](#null-geodesic-congruence)

For an affinely parametrized null congruence in $D$ spacetime dimensions,

$$
\frac{d\theta}{d\lambda}
=-\frac1{D-2}\theta^2
-\widehat\sigma_{ab}\widehat\sigma^{ab}
+\widehat\omega_{ab}\widehat\omega^{ab}
-R_{ab}k^ak^b.
$$

#### Area-square-root optical focusing equation

↑ **Parent:** [Null Raychaudhuri equation](#null-raychaudhuri-equation)

For an affinely parametrized twist-free [null geodesic congruence](#null-geodesic-congruence), let $A$ be local transported screen area and $\sigma^2=\widehat\sigma_{AB}\widehat\sigma^{AB}/2$. The [Null Raychaudhuri equation](#null-raychaudhuri-equation) gives $\theta'=-\theta^2/2-2\sigma^2-R_{ab}k^ak^b$ and $A'/A=\theta$. Combining these gives the displayed equation. Positive shear focuses the beam and has a negative sign. For nonuniform expansion this is a local area identity, not the same differential equation for the entire integrated horizon area.

##### Flat-space anisotropic beam shear focusing

↑ **Parent:** [Area-square-root optical focusing equation](#area-square-root-optical-focusing-equation)

In flat spacetime take a twist-free beam's two screen Jacobi factors to be $1+\lambda$ and $1-\lambda$. They solve the zero-curvature [geodesic deviation](general-relativity.md#geodesic-deviation) equation. Their product is the displayed area, and subtracting the trace from their optical matrix gives the displayed nonnegative shear. Direct differentiation yields $(A^{1/2})''=-(1-\lambda^2)^{-3/2}=-\sigma^2A^{1/2}$, an explicit check of the focusing sign.

#### Null focusing theorem

↑ **Parent:** [Null Raychaudhuri equation](#null-raychaudhuri-equation)

For a hypersurface-orthogonal null congruence under the [null energy condition](general-relativity.md#null-energy-condition) in $D$ spacetime dimensions, an initially negative expansion $\theta_0$ diverges to $-\infty$ within affine distance at most $(D-2)/|\theta_0|$.

##### Conjugate point to a spacelike surface

↑ **Parent:** [Null focusing theorem](#null-focusing-theorem)

A [conjugate point to a spacelike surface](#conjugate-point-to-a-spacelike-surface) occurs where normal [geodesics](riemannian-geometry.md#geodesic) develop a focal degeneracy: the transverse [Jacobi field](general-relativity.md#jacobi-field) map from initial points on the surface ceases to be invertible. Collapse of the transverse area makes the [null expansion](#null-expansion) diverge. Beyond a first such point, the normal [null geodesic](special-relativity.md#null-geodesic) cannot continue as a generator of the [achronal boundary](general-relativity.md#achronal-boundary) of the surface's future.

## ↑ Ancestors (4)

1. [General relativity](general-relativity.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Congruence (general relativity)](general-relativity.md#congruence-general-relativity)
- [Free-fall proper time in Schwarzschild spacetime](general-relativity.md#free-fall-proper-time-in-schwarzschild-spacetime)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-52.md#3/solution)
