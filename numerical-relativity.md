# Numerical relativity

↑ **Parent:** [General relativity](general-relativity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Numerical_relativity)

Numerical relativity solves Einstein's equations as an initial-value problem, usually after decomposing spacetime into spatial hypersurfaces and evolution in time.

**Table of contents**

- [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)
  - [Normal scalar-field momentum](#normal-scalar-field-momentum)
    - [Scalar-field stress projections](#scalar-field-stress-projections)
  - [Unimodular spatial metric](#unimodular-spatial-metric)
  - [Metric determinant in a 3+1 decomposition](#metric-determinant-in-a-3-plus-1-decomposition)
  - [Hamiltonian formulation of general relativity](#hamiltonian-formulation-of-general-relativity)
    - [Vanishing canonical Hamiltonian of a closed universe](#vanishing-canonical-hamiltonian-of-a-closed-universe)
    - [Momentum constraint](#momentum-constraint)
      - [Scalar momentum constraint with positive extrinsic curvature](#scalar-momentum-constraint-with-positive-extrinsic-curvature)
    - [Canonical momentum of the spatial metric](#canonical-momentum-of-the-spatial-metric)
  - [Spatial projection tensor](#spatial-projection-tensor)
    - [Spatial projector derivative identity](#spatial-projector-derivative-identity)
    - [Spatial metric sign for a unit timelike normal](#spatial-metric-sign-for-a-unit-timelike-normal)
    - [Spatial covariant derivative](#spatial-covariant-derivative)
      - [Metric compatibility of the spatial covariant derivative](#metric-compatibility-of-the-spatial-covariant-derivative)
    - [Normal acceleration](#normal-acceleration)
  - [Lapse function](#lapse-function)
  - [Shift vector](#shift-vector)
  - [Extrinsic curvature of a spatial hypersurface](#extrinsic-curvature-of-a-spatial-hypersurface)
    - [Positive-expansion convention for extrinsic curvature](#positive-expansion-convention-for-extrinsic-curvature)
    - [Spatial volume evolution identity](#spatial-volume-evolution-identity)
    - [Extrinsic curvature with a negative shift](#extrinsic-curvature-with-a-negative-shift)
      - [Trace of extrinsic curvature with a negative shift](#trace-of-extrinsic-curvature-with-a-negative-shift)
    - [Gauss–Codazzi equations for a spatial hypersurface](#gauss-codazzi-equations-for-a-spatial-hypersurface)
      - [Contracted Codazzi equation with positive expansion](#contracted-codazzi-equation-with-positive-expansion)
      - [Vacuum Weyl tensors from hypersurface data](#vacuum-weyl-tensors-from-hypersurface-data)
    - [Hypersurface orthogonality implies symmetric extrinsic curvature](#hypersurface-orthogonality-implies-symmetric-extrinsic-curvature)
    - [Scalar Gauss equation](#scalar-gauss-equation)
      - [Hamiltonian constraint](#hamiltonian-constraint)
        - [Time-symmetric conformally flat vacuum initial data](#time-symmetric-conformally-flat-vacuum-initial-data)
        - [Linearized cosmological Hamiltonian constraint](#linearized-cosmological-hamiltonian-constraint)
  - [Z4 formulation](#z4-formulation)
  - [3+1 Noether-current conservation law](#3-plus-1-noether-current-conservation-law)
  - [3+1 decomposition of the stress-energy tensor](#3-plus-1-decomposition-of-the-stress-energy-tensor)
    - [Scalar-field matter projections](#scalar-field-matter-projections)
    - [Momentum equation in a 3+1 decomposition](#momentum-equation-in-a-3-plus-1-decomposition)
  - [Geodesic slicing](#geodesic-slicing)
  - [Baumgarte–Shapiro–Shibata–Nakamura formulation](#baumgarte-shapiro-shibata-nakamura-formulation)
    - [Finite-time blow-up of mean curvature in geodesic slicing](#finite-time-blow-up-of-mean-curvature-in-geodesic-slicing)
- [Harmonic coordinate](#harmonic-coordinate)
  - [Harmonic reduction of the vacuum Einstein equations](#harmonic-reduction-of-the-vacuum-einstein-equations)
  - [Harmonic slicing](#harmonic-slicing)
    - [Harmonic lapse evolution](#harmonic-lapse-evolution)
    - [Bona--Masso slicing condition](#bona-masso-slicing-condition)
      - [Stationary Schwarzschild Bona--Masso slicing function](#stationary-schwarzschild-bona-masso-slicing-function)
  - [Hyperbolic reduction of Einstein's equations](#hyperbolic-reduction-of-einstein-s-equations)
- [ADM formalism](#adm-formalism)

<h2 id="3-plus-1-decomposition-of-spacetime">3+1 decomposition of spacetime</h2>

↑ **Parent:** [Numerical relativity](numerical-relativity.md)

A 3+1 decomposition writes $ds^2=-\alpha^2dt^2+\gamma_{ij}(dx^i+\beta^idt)(dx^j+\beta^jdt)$ in terms of lapse, shift, and spatial metric.

A spacetime foliation separates a spatial metric, lapse and shift. The [ADM formalism](#adm-formalism) uses this decomposition to express Einstein evolution and constraint equations in Hamiltonian form.

### Normal scalar-field momentum

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)

For a [minimally coupled scalar field](quantum-field-theory.md#minimally-coupled-scalar-field) with spatial [induced metric](riemannian-geometry.md#induced-metric) $h_{ij}$, the field's derivative along the future [unit normal](differential-geometry.md#unit-normal) is $\Pi$. If the [shift vector](#shift-vector) enters as $dx^i-N^idt$, then $\Pi=(\dot\phi+N^i\partial_i\phi)/N$. The canonical momentum of the density is $\pi_\phi=\sqrt h\,\Pi$. Confusing this density with the normal derivative loses a volume factor.

#### Scalar-field stress projections

↑ **Parent:** [Normal scalar-field momentum](#normal-scalar-field-momentum)

For a [minimally coupled scalar field](quantum-field-theory.md#minimally-coupled-scalar-field), put $q^2=h^{ij}D_i\phi D_j\phi$ using the [spatial covariant derivative](#spatial-covariant-derivative). Spatial and normal projections of its [stress-energy tensor](general-relativity.md#stress-energy-tensor) give $\rho=\Pi^2/2+q^2/2+V$, $\mathcal J_i=-\Pi D_i\phi$, and $S_{ij}=D_i\phi D_j\phi+h_{ij}(\Pi^2/2-q^2/2-V)$. The trace-free stress is $D_i\phi D_j\phi-h_{ij}q^2/3$, with coefficient one. This makes the scalar [anisotropic stress](general-relativity.md#anisotropic-stress) second order in a spatial gradient expansion.

### Unimodular spatial metric

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)

In fixed spatial coordinates set $a_{\mathrm{loc}}=(\det h)^{1/6}$ and $\gamma_{ij}=a_{\mathrm{loc}}^{-2}h_{ij}$, so $\det\gamma=1$. This volume-shape decomposition is useful for separating isotropic expansion and anisotropic shape. The determinant-defined scale depends on the coordinate volume convention.

<h3 id="metric-determinant-in-a-3-plus-1-decomposition">Metric determinant in a 3+1 decomposition</h3>

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)

For a positive [lapse function](#lapse-function) $\alpha$, [shift vector](#shift-vector) $\beta^i$ and spatial [induced metric](riemannian-geometry.md#induced-metric) $\gamma_{ij}$, the block metric has $g_{00}=-\alpha^2+\gamma_{ij}\beta^i\beta^j$ and $g_{0i}=\gamma_{ij}\beta^j$. Its block determinant is $g=-\alpha^2\det\gamma$. Therefore the [metric volume tensor](differential-form.md#metric-volume-tensor) contracted with the future [unit normal](differential-geometry.md#unit-normal) restricts to the spatial volume tensor: $n^\mu\epsilon_{\mu ijk}=\sqrt{\det\gamma}\,[ijk]$.

### Hamiltonian formulation of general relativity

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)

Using the [lapse function](#lapse-function) $N$, [shift vector](#shift-vector) $N^i$ and spatial metric $h_{ij}$, the [Legendre transform in mechanics](classical-mechanics.md#legendre-transform-in-mechanics) of the [Einstein-Hilbert action](general-relativity.md#einstein-hilbert-action) gives, in units $16\pi G=1$,

$$
H_{\rm bulk}=\int d^3x\sqrt h\,(N\mathcal H+N^i\mathcal H_i),\qquad\mathcal H=\frac{\pi^{ij}\pi_{ij}-\pi^2/2}{h}-{}^{(3)}R,\qquad\mathcal H_i=-2D_j\left(\frac{\pi^j{}_i}{\sqrt h}\right).
$$

Here $\pi=h_{ij}\pi^{ij}$ and $\pi^{ij}$ is the [canonical momentum of the spatial metric](#canonical-momentum-of-the-spatial-metric). Varying lapse and shift imposes the [Hamiltonian constraint](#hamiltonian-constraint) and [momentum constraint](#momentum-constraint). An asymptotic time translation requires an [Arnowitt-Deser-Misner energy](general-relativity.md#arnowitt-deser-misner-energy) boundary term. The bulk constraints generate gauge evolution; the nonzero asymptotic energy comes from the boundary.

#### Vanishing canonical Hamiltonian of a closed universe

↑ **Parent:** [Hamiltonian formulation of general relativity](#hamiltonian-formulation-of-general-relativity)

On a compact spatial [Cauchy hypersurface](general-relativity.md#cauchy-surface) without boundary, the gravitational [Hamiltonian](classical-mechanics.md#hamiltonian) consists entirely of constraints and vanishes on solutions. There is no asymptotic time-translation boundary charge to add. This is the canonical statement that a closed universe has zero total energy; it does not assert that local matter energy density or local curvature vanishes.

#### Momentum constraint

↑ **Parent:** [Hamiltonian formulation of general relativity](#hamiltonian-formulation-of-general-relativity)

The momentum constraint is the equation obtained by varying the [shift vector](#shift-vector) in the [Hamiltonian formulation of general relativity](#hamiltonian-formulation-of-general-relativity). It expresses the tangential-normal projection of the [Einstein field equations](general-relativity.md#einstein-field-equations) and generates spatial coordinate transformations. Writing $p^{ij}=\pi^{ij}/\sqrt h$ avoids ambiguities about covariant derivatives of [tensor densities](general-relativity.md#tensor-density).

##### Scalar momentum constraint with positive extrinsic curvature

↑ **Parent:** [Momentum constraint](#momentum-constraint)

For scalar metric potentials $ds^2=a^2[-(1+2A)d\tau^2+2B_{,i}d\tau dx^i+((1-2\psi)\delta_{ij}+2E_{,ij})dx^idx^j]$ and positive [extrinsic curvature](differential-geometry.md#extrinsic-curvature), $\delta K^i{}_j=a^{-1}[-(\psi'+\mathcal HA)\delta^i{}_j+\partial^i\partial_j(E'-B)]$. The scalar shear terms cancel between its divergence and trace gradient. With $j_i=-P^\mu{}_iT_{\mu\nu}n^\nu$, the [momentum constraint](#momentum-constraint) becomes $2\partial_i(\psi'+\mathcal HA)/a=-8\pi G j_i$. Reversing the convention for $K$ reverses the geometric left side.

#### Canonical momentum of the spatial metric

↑ **Parent:** [Hamiltonian formulation of general relativity](#hamiltonian-formulation-of-general-relativity)

With the convention $K_{ij}=(\dot h_{ij}-D_iN_j-D_jN_i)/(2N)$ for [extrinsic curvature](differential-geometry.md#extrinsic-curvature), differentiation of the gravitational Lagrangian gives $\pi^{ij}=\sqrt h(K^{ij}-Kh^{ij})$ in units $16\pi G=1$. It is a weight-one [tensor density](general-relativity.md#tensor-density). In three spatial dimensions, $\pi=-2\sqrt hK$, so

$$
K^{ij}=h^{-1/2}(\pi^{ij}-\tfrac12\pi h^{ij}).
$$

The [lapse function](#lapse-function) and [shift vector](#shift-vector) have no time derivatives in this action and consequently have vanishing conjugate momenta. Changing the sign convention for extrinsic curvature changes the corresponding momentum relation; it must not be silently combined with this formula.

### Spatial projection tensor

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)

For a unit timelike normal $n^\mu n_\mu=-1$, the spatial projection tensor annihilates $n^\mu$ and projects every spacetime tensor onto a spatial hypersurface.

#### Spatial projector derivative identity

↑ **Parent:** [Spatial projection tensor](#spatial-projection-tensor)

Differentiating the [spatial projection tensor](#spatial-projection-tensor) and projecting its derivative and covariant indices leaves $-n^\lambda K_{\sigma\rho}$, where $K$ is the [extrinsic curvature of a spatial hypersurface](#extrinsic-curvature-of-a-spatial-hypersurface). Contracting $\lambda$ with $\rho$ gives zero because $K$ is transverse. This distinction separates the informative tensor identity, with a free normal index, from its vanishing trace. [Hypersurface orthogonality implies symmetric extrinsic curvature](#hypersurface-orthogonality-implies-symmetric-extrinsic-curvature).

#### Spatial metric sign for a unit timelike normal

↑ **Parent:** [Spatial projection tensor](#spatial-projection-tensor)

With signature $+---$ and $n^\mu n_\mu=1$, the [spatial projection tensor](#spatial-projection-tensor) is $P^\mu{}_\nu=\delta^\mu{}_\nu-n^\mu n_\nu$. Projecting the spacetime [metric tensor](general-relativity.md#metric-tensor) gives $q_{\mu\nu}=g_{\mu\nu}-n_\mu n_\nu$, which is negative definite on spatial vectors. The positive spatial [induced metric](riemannian-geometry.md#induced-metric) is $h_{\mu\nu}=-q_{\mu\nu}$. A plus sign in $g_{\mu\nu}+n_\mu n_\nu$ belongs to a different normal/signature convention and is not transverse in this one. Fully projected [covariant derivatives](general-relativity.md#covariant-derivative) of either spatial metric vanish by [metric compatibility](fiber-bundle.md#metric-compatibility).

#### Spatial covariant derivative

↑ **Parent:** [Spatial projection tensor](#spatial-projection-tensor)

The spatial covariant derivative projects the spacetime [covariant derivative](general-relativity.md#covariant-derivative) and every free tensor index onto a spatial hypersurface. It is the [Levi-Civita connection](general-relativity.md#levi-civita-connection) of the induced spatial metric.

##### Metric compatibility of the spatial covariant derivative

↑ **Parent:** [Spatial covariant derivative](#spatial-covariant-derivative)

For a unit timelike normal $n$, the [induced metric](riemannian-geometry.md#induced-metric) is $h_{\mu\nu}=g_{\mu\nu}+n_\mu n_\nu$. The [spatial covariant derivative](#spatial-covariant-derivative) projects the derivative and all free indices with the [spatial projection tensor](#spatial-projection-tensor) $P^\mu{}_\nu=\delta^\mu{}_\nu+n^\mu n_\nu$. [Metric compatibility](fiber-bundle.md#metric-compatibility) gives $\nabla_\lambda h_{\mu\nu}=(\nabla_\lambda n_\mu)n_\nu+n_\mu\nabla_\lambda n_\nu$; projecting kills the normal factor in each term. Thus the [spatial covariant derivative](#spatial-covariant-derivative) is compatible with the [induced metric](riemannian-geometry.md#induced-metric).

#### Normal acceleration

↑ **Parent:** [Spatial projection tensor](#spatial-projection-tensor)

The normal acceleration measures failure of the hypersurface unit normals to be geodesics. It is spatial, $n^\mu a_\mu=0$, and in a 3+1 decomposition satisfies $a_i=D_i\log\alpha$.

### Lapse function

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lapse_function)

The lapse function measures proper-time separation between neighboring spatial hypersurfaces along their unit normal.

### Shift vector

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shift_vector)

The shift vector describes how spatial coordinates move tangentially between neighboring hypersurfaces.

### Extrinsic curvature of a spatial hypersurface

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)

With future unit normal $n^\mu$, the convention $K_{\mu\nu}=-\perp^\rho{}_\mu\nabla_\rho n_\nu$ measures how the hypersurface is embedded in spacetime.

#### Positive-expansion convention for extrinsic curvature

↑ **Parent:** [Extrinsic curvature of a spatial hypersurface](#extrinsic-curvature-of-a-spatial-hypersurface)

With a future unit timelike normal in signature $(-,+,+,+)$, this convention makes the [extrinsic curvature](differential-geometry.md#extrinsic-curvature) trace equal to the normal congruence's expansion, $K=\nabla_\mu n^\mu$. An expanding flat [Friedmann-Lemaître-Robertson-Walker metric](cosmology.md#friedmann-lemaitre-robertson-walker-metric) has $K_{ij}=a'\delta_{ij}$ and $K=3a'/a^2$. This is the opposite sign to the negative-expansion convention used in many [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime) formulas. Projection identities and momentum constraints must use the same convention throughout.

#### Spatial volume evolution identity

↑ **Parent:** [Extrinsic curvature of a spatial hypersurface](#extrinsic-curvature-of-a-spatial-hypersurface)

In a [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime) with $K_{ij}=-(\partial_t\gamma_{ij}-\mathcal L_\beta\gamma_{ij})/(2\alpha)$, contract the metric evolution with $\gamma^{ij}$ and use the [Jacobi determinant derivative formula](linear-algebra.md#jacobi-determinant-derivative-formula). Here $\gamma=\det\gamma_{ij}$, $K=\gamma^{ij}K_{ij}$, $\alpha$ is the [lapse function](#lapse-function), and $\beta$ is the [shift vector](#shift-vector). The identity separates spatial transport and coordinate compression from the geometric volume change caused by [extrinsic curvature](differential-geometry.md#extrinsic-curvature).

#### Extrinsic curvature with a negative shift

↑ **Parent:** [Extrinsic curvature of a spatial hypersurface](#extrinsic-curvature-of-a-spatial-hypersurface)

For $ds^2=-N^2dt^2+h_{ij}(dx^i-N^idt)(dx^j-N^jdt)$ and the future unit normal, the convention $K_{ij}=-n_{i;j}$ gives $K_{ij}=-(\dot h_{ij}+D_iN_j+D_jN_i)/(2N)$. Lower the [shift vector](#shift-vector) with $h$. The sign of the shift terms changes when the opposite threading convention is used.

##### Trace of extrinsic curvature with a negative shift

↑ **Parent:** [Extrinsic curvature with a negative shift](#extrinsic-curvature-with-a-negative-shift)

For the threading convention $dx^i-N^i dt$ and $K_{ij}=-(\dot\gamma_{ij}+D_iN_j+D_jN_i)/(2N)$, contract with $\gamma^{ij}$. [Metric compatibility](fiber-bundle.md#metric-compatibility) gives $\gamma^{ij}D_iN_j=D_iN^i$, and the [Jacobi determinant derivative formula](linear-algebra.md#jacobi-determinant-derivative-formula) gives $\gamma^{ij}\dot\gamma_{ij}=\partial_t\log\det\gamma$. With zero shift, $-K/3=(3N)^{-1}\partial_t\log\sqrt\gamma$ is the [local volume Hubble parameter](cosmology.md#local-volume-hubble-parameter). Reversing the shift convention reverses both the normal's spatial component and the shift terms; the two conventions must not be mixed.

<h4 id="gauss-codazzi-equations-for-a-spatial-hypersurface">Gauss–Codazzi equations for a spatial hypersurface</h4>

↑ **Parent:** [Extrinsic curvature of a spatial hypersurface](#extrinsic-curvature-of-a-spatial-hypersurface)

With signature $(-,+,+,+)$, future [unit normal](differential-geometry.md#unit-normal) $n$ and $K_{ab}=-P^c{}_aP^d{}_b\nabla_cn_d$, the [Gauss–Codazzi equations](second-fundamental-form.md#gauss-codazzi-equations) become $(\perp R)_{abcd}=\mathcal R_{abcd}+K_{ac}K_{db}-K_{ad}K_{cb}$ and $(\perp R)_{abcd}n^d=-D_aK_{bc}+D_bK_{ac}$, where in the second expression only the first three indices are projected. The intrinsic curvature and [spatial covariant derivative](#spatial-covariant-derivative) use the spatial [induced metric](riemannian-geometry.md#induced-metric). The normal is timelike, so the normal-sign convention differs from a spacelike normal in a positive-definite ambient metric.

##### Contracted Codazzi equation with positive expansion

↑ **Parent:** [Gauss–Codazzi equations for a spatial hypersurface](#gauss-codazzi-equations-for-a-spatial-hypersurface)

For the [positive-expansion convention for extrinsic curvature](#positive-expansion-convention-for-extrinsic-curvature), write $\nabla_\mu n_\nu=K_{\mu\nu}-n_\mu a_\nu$ with [normal acceleration](#normal-acceleration) $a_\nu=n^\rho\nabla_\rho n_\nu$. The Ricci commutator applied to $n$ gives the difference of its two second-derivative contractions. Projecting tangentially, the acceleration term in that commutator cancels exactly the acceleration term converting a spacetime divergence of $K$ into its fully projected [spatial covariant derivative](#spatial-covariant-derivative). Einstein's equations then identify the displayed equation as the [momentum constraint](#momentum-constraint).

##### Vacuum Weyl tensors from hypersurface data

↑ **Parent:** [Gauss–Codazzi equations for a spatial hypersurface](#gauss-codazzi-equations-for-a-spatial-hypersurface)

For a Ricci-flat spacetime with the stated [Gauss–Codazzi equations for a spatial hypersurface](#gauss-codazzi-equations-for-a-spatial-hypersurface) and induced orientation $\tilde\epsilon_{abc}=n^d\epsilon_{dabc}$, the [electric part of the Weyl tensor](general-relativity.md#electric-part-of-the-weyl-tensor) and [magnetic part of the Weyl tensor](general-relativity.md#magnetic-part-of-the-weyl-tensor) satisfy

$$
E_{ab}=\mathcal R_{ab}+KK_{ab}-K_a{}^cK_{cb},\qquad B_{ab}=\tilde\epsilon_a{}^{cd}D_cK_{db}.
$$

The electric relation comes from the vanishing spatial projection of the [Ricci tensor](general-relativity.md#ricci-tensor). The magnetic relation combines the normal curvature projection with the sign $\epsilon_{acde}n^c=-\tilde\epsilon_{ade}$.

#### Hypersurface orthogonality implies symmetric extrinsic curvature

↑ **Parent:** [Extrinsic curvature of a spatial hypersurface](#extrinsic-curvature-of-a-spatial-hypersurface)

Unit normalization gives $n^\nu\nabla_\mu n_\nu=0$. Hence $K_{\mu\nu}=-P^\alpha{}_\mu P^\beta{}_\nu\nabla_\alpha n_\beta=-P^\alpha{}_\mu\nabla_\alpha n_\nu$. Set $F_{\mu\nu}=\nabla_\mu n_\nu-\nabla_\nu n_\mu$. [Frobenius theorem](differential-geometry.md#frobenius-theorem) for a hypersurface normal gives $n_\alpha F_{\beta\gamma}+n_\beta F_{\gamma\alpha}+n_\gamma F_{\alpha\beta}=0$. Contracting with $n^\alpha P^\beta{}_\mu P^\gamma{}_\nu$ leaves $-P^\beta{}_\mu P^\gamma{}_\nu F_{\beta\gamma}=0$, precisely the vanishing antisymmetric part of the [extrinsic curvature of a spatial hypersurface](#extrinsic-curvature-of-a-spatial-hypersurface).

#### Scalar Gauss equation

↑ **Parent:** [Extrinsic curvature of a spatial hypersurface](#extrinsic-curvature-of-a-spatial-hypersurface)

For the convention $K_{\mu\nu}=-\perp^\rho{}_\mu\nabla_\rho n_\nu$, contraction of the [Gauss equation](second-fundamental-form.md#gauss-equation) gives

$$
{}^{(4)}R+2R_{\mu\nu}n^\mu n^\nu
={}^{(3)}R+K^2-K_{\mu\nu}K^{\mu\nu}.
$$

##### Hamiltonian constraint

↑ **Parent:** [Scalar Gauss equation](#scalar-gauss-equation)

The Hamiltonian constraint is the normal-normal projection of the [Einstein field equations](general-relativity.md#einstein-field-equations) onto a spatial hypersurface. With the extrinsic-curvature convention used here,

$$
{}^{(3)}R+K^2-K_{ij}K^{ij}=16\pi\rho.
$$

###### Time-symmetric conformally flat vacuum initial data

↑ **Parent:** [Hamiltonian constraint](#hamiltonian-constraint)

For a spatial initial slice with vanishing [extrinsic curvature](differential-geometry.md#extrinsic-curvature), the vacuum [momentum constraint](#momentum-constraint) is automatic and the [Hamiltonian constraint](#hamiltonian-constraint) requires zero [Ricci scalar](general-relativity.md#ricci-scalar). In three spatial dimensions, the indicated [conformally flat metric](general-relativity.md#conformally-flat-metric) has $\mathcal R=-8\psi^{-5}\Delta\psi$, with a nonzero [conformal factor](general-relativity.md#conformal-factor). Thus a [harmonic function](partial-differential-equation.md#harmonic-function) supplies the data on its domain. A positive example is $\psi=1+a/r$ on a punctured or exterior region. There is no nonconstant globally smooth example on all of Euclidean three-space tending to one at infinity, by the [maximum principle for harmonic functions](partial-differential-equation.md#maximum-principle-for-harmonic-functions). Time symmetry of an initial slice does not imply that its entire evolved spacetime is static.

###### Linearized cosmological Hamiltonian constraint

↑ **Parent:** [Hamiltonian constraint](#hamiltonian-constraint)

For a spatially flat [Friedmann-Lemaître-Robertson-Walker metric](cosmology.md#friedmann-lemaitre-robertson-walker-metric), negative [extrinsic curvature](differential-geometry.md#extrinsic-curvature), and $K=-3H+\kappa$, the [Hamiltonian constraint](#hamiltonian-constraint) gives the displayed scalar perturbation equation. Indeed $K^2=9H^2-6H\kappa$ and $K^i{}_jK^j{}_i=3H^2-2H\kappa$ to first order. The spatial [Ricci scalar](general-relativity.md#ricci-scalar) is $4\Delta\Phi$; subtract the background equation $6H^2=16\pi G\bar\rho$ and divide by four.

### Z4 formulation

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)

The Z4 formulation introduces a spacetime vector $Z_\mu$ into Einstein's equations so that the Hamiltonian and momentum constraints become part of a dynamical system. Its normal projection is commonly written $\Theta=-n^\mu Z_\mu$.

<h3 id="3-plus-1-noether-current-conservation-law">3+1 Noether-current conservation law</h3>

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)

For $J^\mu=Qn^\mu+Q^\mu$ with spatial $Q^\mu$, current conservation gives $n^\mu\nabla_\mu Q=KQ-D_\mu Q^\mu-Q^\mu D_\mu\log\alpha$ under the stated extrinsic-curvature convention.

<h3 id="3-plus-1-decomposition-of-the-stress-energy-tensor">3+1 decomposition of the stress-energy tensor</h3>

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)

Relative to a future unit normal $n^\mu$, the stress-energy tensor decomposes as

$$
T_{\mu\nu}=\rho n_\mu n_\nu+j_\mu n_\nu+n_\mu j_\nu+S_{\mu\nu},
$$

where $j_\mu$ and both indices of $S_{\mu\nu}$ are spatial.

#### Scalar-field matter projections

↑ **Parent:** [3+1 decomposition of the stress-energy tensor](#3-plus-1-decomposition-of-the-stress-energy-tensor)

For signature $(+---)$ and future normal $n$, write $\Pi=n^\mu\partial_\mu\phi$ and use the positive induced metric $\gamma_{ij}$ for $s^2=\gamma^{ij}D_i\phi D_j\phi$. The [Klein-Gordon scalar stress-energy tensor](general-relativity.md#klein-gordon-scalar-stress-energy-tensor) has normal-frame density $\rho=(\Pi^2+s^2)/2+V$, momentum $J_i=-\Pi D_i\phi$ and spatial stress $S_{ij}=D_i\phi D_j\phi+\gamma_{ij}[(\Pi^2-s^2)/2-V]$. The spatial index convention and normal orientation must be specified.

<h4 id="momentum-equation-in-a-3-plus-1-decomposition">Momentum equation in a 3+1 decomposition</h4>

↑ **Parent:** [3+1 decomposition of the stress-energy tensor](#3-plus-1-decomposition-of-the-stress-energy-tensor)

With $K_{\mu\nu}=-\perp^\rho{}_\mu\nabla_\rho n_\nu$ and $a_\mu=n^\rho\nabla_\rho n_\mu$, spatial projection of $\nabla_\mu T^{\mu\nu}=0$ gives

$$
\mathcal L_nj_\alpha=-D_\mu S^\mu{}_\alpha-S^\mu{}_\alpha a_\mu+Kj_\alpha-\rho a_\alpha.
$$

### Geodesic slicing

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geodesic_slicing)

Geodesic slicing chooses unit lapse and zero shift, so the hypersurface normals are affinely parametrized timelike geodesics. It is simple but commonly develops coordinate singularities in finite time.

<h3 id="baumgarte-shapiro-shibata-nakamura-formulation">Baumgarte–Shapiro–Shibata–Nakamura formulation</h3>

↑ **Parent:** [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Baumgarte–Shapiro–Shibata–Nakamura_formulation)

The Baumgarte–Shapiro–Shibata–Nakamura formulation rewrites the Einstein evolution equations using a conformal spatial metric, conformal traceless extrinsic curvature, the trace $K$, and conformal connection functions.

#### Finite-time blow-up of mean curvature in geodesic slicing

↑ **Parent:** [Baumgarte–Shapiro–Shibata–Nakamura formulation](#baumgarte-shapiro-shibata-nakamura-formulation)

In vacuum geodesic slicing, discarding nonnegative shear leaves $\partial_tK=K^2/3$. Positive initial $K_0$ therefore gives $K=K_0/[1-K_0(t-t_0)/3]$ and blows up at $t=t_0+3/K_0$.

## Harmonic coordinate

↑ **Parent:** [Numerical relativity](numerical-relativity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Harmonic_coordinate)

A harmonic coordinate satisfies $\Delta_gx^\lambda=0$ for a [Riemannian metric](differential-geometry.md#riemannian-metric), or $\Box_gx^\lambda=0$ for a [Lorentzian metric](general-relativity.md#lorentzian-metric). Equivalently $g^{\mu\nu}\Gamma^\lambda_{\mu\nu}=0$ or $\partial_\mu(\sqrt{|\det g|}\,g^{\lambda\mu})=0$. This common coordinate condition applies in both [Riemannian geometry](riemannian-geometry.md) and [general relativity](general-relativity.md).

### Harmonic reduction of the vacuum Einstein equations

↑ **Parent:** [Harmonic coordinate](#harmonic-coordinate)

With the [Riemann curvature tensor](general-relativity.md#riemann-curvature-tensor) convention $R^\mu{}_{\nu\rho\sigma}=\partial_\rho\Gamma^\mu{}_{\nu\sigma}-\partial_\sigma\Gamma^\mu{}_{\nu\rho}+\cdots$, [harmonic coordinates](#harmonic-coordinate) remove the mixed second derivatives from the [Ricci tensor](general-relativity.md#ricci-tensor). The remainder $Q_{ab}$ contains at most first derivatives of the [metric tensor](general-relativity.md#metric-tensor). The vacuum [Einstein field equations](general-relativity.md#einstein-field-equations) become a system of [quasilinear partial differential equations](partial-differential-equation.md#quasilinear-partial-differential-equation) with a Lorentzian [wave equation](wave-equation.md) principal part. Harmonic coordinate constraints must be maintained when using the reduced system.

### Harmonic slicing

↑ **Parent:** [Harmonic coordinate](#harmonic-coordinate)

Harmonic slicing imposes the harmonic-coordinate condition only on time. In 3+1 form it obeys $(\partial_t-\beta^i\partial_i)\alpha=-\alpha^2K$.

#### Harmonic lapse evolution

↑ **Parent:** [Harmonic slicing](#harmonic-slicing)

For a positive [lapse function](#lapse-function) $\alpha$, [shift vector](#shift-vector) $\beta^i$, and the convention $K_{ij}=-(\partial_t\gamma_{ij}-\mathcal L_\beta\gamma_{ij})/(2\alpha)$ for [extrinsic curvature of a spatial hypersurface](#extrinsic-curvature-of-a-spatial-hypersurface), the time-coordinate [harmonic slicing](#harmonic-slicing) condition yields the displayed advective lapse equation. Combining $\partial_t(\sqrt\gamma/\alpha)=\partial_i(\sqrt\gamma\beta^i/\alpha)$ with the [spatial volume evolution identity](#spatial-volume-evolution-identity) proves it without setting the [shift vector](#shift-vector) to zero.

<h4 id="bona-masso-slicing-condition">Bona--Masso slicing condition</h4>

↑ **Parent:** [Harmonic slicing](#harmonic-slicing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bona--Masso_slicing_condition)

The Bona--Masso family is $(\partial_t-\beta^i\partial_i)\alpha=-\alpha^2f(\alpha)K$. Harmonic slicing is the choice $f=1$.

<h5 id="stationary-schwarzschild-bona-masso-slicing-function">Stationary Schwarzschild Bona--Masso slicing function</h5>

↑ **Parent:** [Bona--Masso slicing condition](#bona-masso-slicing-condition)

For the stationary conformally flat Schwarzschild slicing with areal radius $R=r+M$, lapse $\alpha=r/(r+M)$, and radial shift $\beta^r=Mr/(r+M)^2$, the Bona--Masso condition selects

$$
f(\alpha)=\frac{1-\alpha}{\alpha}.
$$

<h3 id="hyperbolic-reduction-of-einstein-s-equations">Hyperbolic reduction of Einstein's equations</h3>

↑ **Parent:** [Harmonic coordinate](#harmonic-coordinate)

In harmonic gauge, the vacuum Einstein equations have principal part $-g^{\mu\nu}\partial_\mu\partial_\nu g_{\alpha\beta}/2$, forming a quasilinear wave system supplemented by constraints.

## ADM formalism

↑ **Parent:** [Numerical relativity](numerical-relativity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/ADM_formalism)

The Arnowitt-Deser-Misner formalism expresses [general relativity](general-relativity.md) as constrained Hamiltonian evolution of a spatial metric and its conjugate momentum after a [3+1 decomposition of spacetime](#3-plus-1-decomposition-of-spacetime). Lapse and shift enforce the Hamiltonian and momentum constraints. For an asymptotically flat spacetime its boundary Hamiltonian gives the [Arnowitt-Deser-Misner energy](general-relativity.md#arnowitt-deser-misner-energy).

## ↑ Ancestors (4)

1. [General relativity](general-relativity.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)
