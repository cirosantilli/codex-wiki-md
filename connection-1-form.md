# Connection 1-form

↑ **Parent:** [Orthonormal coframe in spacetime](general-relativity.md#orthonormal-coframe-in-spacetime)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Connection_1-form)

Connection one-forms are defined by $\nabla e_b=\omega^a{}_b\otimes e_a$. For the Levi-Civita connection they obey Cartan's torsion-free equation $d\theta^a+\omega^a{}_b\wedge\theta^b=0$ and metric compatibility $\omega_{ab}=-\omega_{ba}$.

**Table of contents**

- [Lorentzian connection-form antisymmetry](#lorentzian-connection-form-antisymmetry)
- [Spin connection](#spin-connection)
  - [Spin connection of a conformally flat metric](#spin-connection-of-a-conformally-flat-metric)
  - [Tetrad postulate](#tetrad-postulate)
  - [Spinor covariant derivative](#spinor-covariant-derivative)
    - [Twistor spinor](#twistor-spinor)
      - [Conformal rescaling of a parallel spinor to a twistor spinor](#conformal-rescaling-of-a-parallel-spinor-to-a-twistor-spinor)
    - [Two-component spinor calculus](#two-component-spinor-calculus)
      - [Two-component spinor](#two-component-spinor)
      - [Weyl curvature spinor](#weyl-curvature-spinor)
      - [Chiral spinor curvature operator](#chiral-spinor-curvature-operator)
        - [Chiral Riemann curvature spinor decomposition](#chiral-riemann-curvature-spinor-decomposition)
        - [Contracted chiral curvature identity](#contracted-chiral-curvature-identity)
    - [Parallel spinor](#parallel-spinor)
      - [Polar-frame parallel spinor](#polar-frame-parallel-spinor)
    - [Spinor curvature identity](#spinor-curvature-identity)
      - [Killing-spinor integrability with rescaled gamma matrices](#killing-spinor-integrability-with-rescaled-gamma-matrices)
        - [Maximal Killing spinors force constant negative curvature](#maximal-killing-spinors-force-constant-negative-curvature)
      - [Einstein tensor contraction of spin curvature](#einstein-tensor-contraction-of-spin-curvature)
- [Cartan's first structure equation](#cartan-s-first-structure-equation)
- [Cartan's second structure equation](#cartan-s-second-structure-equation)
- [Curvature 2-form](#curvature-2-form)
  - [Cartan curvature forms for a static spherical metric](#cartan-curvature-forms-for-a-static-spherical-metric)
  - [Diagonal curvature operator](#diagonal-curvature-operator)
    - [Diagonal curvature operator implies diagonal Ricci tensor](#diagonal-curvature-operator-implies-diagonal-ricci-tensor)

## Lorentzian connection-form antisymmetry

↑ **Parent:** [Connection 1-form](connection-1-form.md)

In an [orthonormal coframe in spacetime](general-relativity.md#orthonormal-coframe-in-spacetime), antisymmetry applies after lowering the first index with the Lorentzian frame metric. Thus mixed time–space [connection 1-forms](connection-1-form.md) are equal under index interchange, while mixed spatial forms are opposite. The same rule holds for [curvature 2-forms](#curvature-2-form). Confusing lowered antisymmetry with ordinary mixed-index antisymmetry changes the curvature signs.

## Spin connection

↑ **Parent:** [Connection 1-form](connection-1-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spin_connection)

In an [orthonormal frame](general-relativity.md#orthonormal-frame-in-spacetime), the spin connection is the Lorentz connection acting on spinors. With $\gamma^{AB}=\tfrac12[\gamma^A,\gamma^B]$, its [covariant derivative](general-relativity.md#covariant-derivative) is $\nabla_\mu\psi=\partial_\mu\psi+\tfrac14\omega_{\mu AB}\gamma^{AB}\psi$. The metric connection determines $\omega$ when torsion conditions are specified. A [zweibein](general-relativity.md#zweibein) gives its two-dimensional form; omitting it on a curved worldsheet generally destroys covariance.

### Spin connection of a conformally flat metric

↑ **Parent:** [Spin connection](#spin-connection)

For $g_{ab}=\Omega^2\eta_{ab}$, use the [vierbein](general-relativity.md#orthonormal-coframe-in-spacetime) $e^\mu{}_a=\Omega\delta^\mu{}_a$ and constant flat [gamma matrices](algebra.md#gamma-matrices). The [tetrad postulate](#tetrad-postulate) and $\Gamma^c{}_{ab}=\delta^c_a\partial_b\log\Omega+\delta^c_b\partial_a\log\Omega-\eta_{ab}\eta^{cd}\partial_d\log\Omega$ give the displayed lowered [spin connection](#spin-connection). With $L=\widehat\gamma^c\partial_c\log\Omega$, its spinor action is $\nabla_a=\partial_a+[\widehat\gamma_a,L]/4$. The Lorentz index lowering matters in indefinite signature.

### Tetrad postulate

↑ **Parent:** [Spin connection](#spin-connection)

The [tetrad postulate](#tetrad-postulate) expresses compatibility of the spacetime and Lorentz-frame connections on a [vierbein](general-relativity.md#orthonormal-coframe-in-spacetime). For the inverse coframe $e_\nu{}^b$, solving gives $\omega_a{}^\mu{}_{\nu}=e_\nu{}^b(\Gamma^c{}_{ab}e^\mu{}_c-\partial_a e^\mu{}_b)$. [Metric compatibility](fiber-bundle.md#metric-compatibility) makes the lowered connection antisymmetric in its Lorentz indices. Lifting this connection through the [Spinor representation of the Lorentz group](relativistic-quantum-field.md#spinor-representation-of-the-lorentz-group) defines the [spinor covariant derivative](#spinor-covariant-derivative).

### Spinor covariant derivative

↑ **Parent:** [Spin connection](#spin-connection)

Lift the [Levi-Civita connection](general-relativity.md#levi-civita-connection) to the [spinor bundle](riemannian-geometry.md#spinor-bundle) using the spin representation of the Lorentz algebra. Under a [local Lorentz transformation](special-relativity.md#local-lorentz-transformation), its matrix $\Omega_\mu=\tfrac14\omega_{\mu AB}\gamma^{AB}$ obeys $\Omega'_\mu=S\Omega_\mu S^{-1}-(\partial_\mu S)S^{-1}$, so $\nabla'_\mu\psi'=S\nabla_\mu\psi$. The [Clifford algebra](algebra.md#clifford-algebra) identity $[\gamma^C,\gamma^{AB}]=2(\eta^{CA}\gamma^B-\eta^{CB}\gamma^A)$ fixes the coefficient. The tetrad postulate then gives $\partial_\mu\gamma^\nu+\Gamma^\nu_{\mu\rho}\gamma^\rho+[\Omega_\mu,\gamma^\nu]=0$, establishing compatibility with curved Clifford multiplication.

#### Twistor spinor

↑ **Parent:** [Spinor covariant derivative](#spinor-covariant-derivative)

A [twistor spinor](#twistor-spinor) has vanishing gamma-trace-free part of its [spinor covariant derivative](#spinor-covariant-derivative). In $n$ dimensions the displayed equation uses [gamma matrices](algebra.md#gamma-matrices) satisfying $\{\gamma_a,\gamma_b\}=2g_{ab}$. It is weaker than being a [parallel spinor](#parallel-spinor). In four dimensions it implies $[\gamma_a\nabla_b+\gamma_b\nabla_a-g_{ab}\gamma^c\nabla_c/2]\epsilon=0$.

##### Conformal rescaling of a parallel spinor to a twistor spinor

↑ **Parent:** [Twistor spinor](#twistor-spinor)

In the conformal frame for $g=\Omega^2\eta$, identify the spinor fibres using the chosen [vierbein](general-relativity.md#orthonormal-coframe-in-spacetime). If $\epsilon_0$ is a flat constant [spinor field](riemannian-geometry.md#spinor-field), the [spin connection of a conformally flat metric](#spin-connection-of-a-conformally-flat-metric) gives $\nabla_a\epsilon=\widehat\gamma_a\widehat\gamma^c(\partial_c\log\Omega)\epsilon/2$. Contracting with curved $\gamma^a=\Omega^{-1}\widehat\gamma^a$ yields $\gamma^a\nabla_a\epsilon=n\Omega^{-1}\widehat\gamma^c(\partial_c\log\Omega)\epsilon/2$. Thus $\nabla_a\epsilon=\gamma_a\gamma^b\nabla_b\epsilon/n$: the rescaled parallel spinor is a [twistor spinor](#twistor-spinor).

#### Two-component spinor calculus

↑ **Parent:** [Spinor covariant derivative](#spinor-covariant-derivative)

The complexified tangent space of a four-dimensional [Lorentzian manifold](topology.md#lorentzian-manifold) factors locally into an unprimed and a primed two-dimensional [spinor representation](semisimple-lie-algebra.md#spin-representation). Their alternating forms $\epsilon_{AB}$ and $\epsilon_{A'B'}$ encode the [metric tensor](general-relativity.md#metric-tensor) and raise or lower spinor indices. A convention must specify the order of contraction with these alternating forms. An antisymmetric spacetime tensor decomposes into symmetric unprimed and primed spinors, $F_{AA'BB'}=\phi_{AB}\epsilon_{A'B'}+\widetilde\phi_{A'B'}\epsilon_{AB}$. This splits the six-dimensional space of [differential two-forms](differential-form.md#2-form) into the two three-dimensional eigenspaces of the complexified [Hodge star operator](differential-form.md#hodge-star-operator).

##### Two-component spinor

↑ **Parent:** [Two-component spinor calculus](#two-component-spinor-calculus)

A two-component [two-component spinor](#two-component-spinor) is an element of a two-dimensional complex spin space with invariant antisymmetric form $\epsilon_{AB}$. In complexified four-dimensional geometry there are independent unprimed and primed spin spaces, and vectors are represented by $x^{AA'}$. Raising an index uses the antisymmetric form, so $\pi^{A'}\pi_{A'}=0$. This identity makes the incidence-plane directions $\pi^{A'}\partial_{AA'}$ totally null.

##### Weyl curvature spinor

↑ **Parent:** [Two-component spinor calculus](#two-component-spinor-calculus)

The totally symmetric unprimed four-index spinor represents one chiral part of the [Weyl tensor](general-relativity.md#weyl-tensor). The other part is represented by a primed spinor, conjugate to the unprimed one on a Lorentzian real slice. The trace-free symmetry separates conformal curvature from the [Ricci tensor](general-relativity.md#ricci-tensor) and scalar-curvature terms.

##### Chiral spinor curvature operator

↑ **Parent:** [Two-component spinor calculus](#two-component-spinor-calculus)

The [spinor covariant derivative](#spinor-covariant-derivative) commutator is a [differential two-form](differential-form.md#2-form) in its derivative indices, so the [two-component spinor calculus](#two-component-spinor-calculus) decomposition defines symmetric curvature operators $\Delta_{AB}$ and $\Delta_{A'B'}$. With $\epsilon^{AB}\epsilon_{AB}=2$, the unprimed projection is $\Delta_{AB}=\epsilon^{A'B'}[\nabla_{AA'},\nabla_{BB'}]/2$, and the primed projection is analogous. For a [torsion-free connection](fiber-bundle.md#torsion-free-connection) these are algebraic curvature derivations: they annihilate scalar functions and obey the [Leibniz rule](calculus.md#leibniz-rule) on tensor products.

###### Chiral Riemann curvature spinor decomposition

↑ **Parent:** [Chiral spinor curvature operator](#chiral-spinor-curvature-operator)

Metric compatibility makes the curvature action on a two-component spinor symplectic, so its lowered curvature spinor is symmetric in each pair. The pair-exchange symmetry of the [Riemann curvature tensor](general-relativity.md#riemann-curvature-tensor) makes $X_{ABCD}=X_{CDAB}$. This six-component tensor decomposes into the five-component totally symmetric [Weyl curvature spinor](#weyl-curvature-spinor) $\Psi_{ABCD}=X_{(ABCD)}$ and one scalar term. In the displayed normalization, with alternating forms satisfying $\epsilon^{AB}\epsilon_{AB}=2$, its scalar is $\Lambda=X_{ABCD}\epsilon^{AC}\epsilon^{BD}/3$. This coefficient follows by contracting the displayed scalar term; different normalizations of that term give different scalar conventions.

###### Contracted chiral curvature identity

↑ **Parent:** [Chiral spinor curvature operator](#chiral-spinor-curvature-operator)

For the [Levi-Civita connection](general-relativity.md#levi-civita-connection), the action of the curvature commutator on a [bivector](linear-algebra.md#bivector) $w^{ab}$ obeys $[\nabla_a,\nabla_b]w^{ab}=0$: both resulting curvature contractions pair the symmetric [Ricci tensor](general-relativity.md#ricci-tensor) with an antisymmetric tensor. For a bivector of one chirality, $w^{AA'BB'}=\phi^{AB}\epsilon^{A'B'}$, this is $2\Delta_{AB}\phi^{AB}=0$. In particular it holds for $\phi^{AB}=\alpha^A\alpha^B$; polarization gives $\Delta_{AB}(\alpha^{(A}\beta^{B)})=0$. The polarization step avoids incorrectly calling $\alpha_A\beta_B\epsilon_{A'B'}$ a simple bivector for independent spinors.

#### Parallel spinor

↑ **Parent:** [Spinor covariant derivative](#spinor-covariant-derivative)

A parallel [spinor field](riemannian-geometry.md#spinor-field) is annihilated by the [spinor covariant derivative](#spinor-covariant-derivative). Its value at one point determines it on a connected domain by [parallel transport](fiber-bundle.md#parallel-transport). The [spinor curvature identity](#spinor-curvature-identity) implies $R_{\mu\nu AB}\gamma^{AB}\epsilon=0$, but this local condition alone need not settle global existence: the [spin structure](riemannian-geometry.md#spin-structure) and [holonomy](fiber-bundle.md#holonomy) also matter. Lorentzian parallel spinors need not force the whole [Ricci tensor](general-relativity.md#ricci-tensor) to vanish, unlike the positive-definite case.

##### Polar-frame parallel spinor

↑ **Parent:** [Parallel spinor](#parallel-spinor)

In flat three-dimensional spacetime with polar spatial [orthonormal coframe](general-relativity.md#orthonormal-coframe-in-spacetime) $(dT,d\rho,\rho d\phi)$, the [spin connection](#spin-connection) has $\omega_{12}=-d\phi$. Thus every [parallel spinor](#parallel-spinor) has the displayed components. Since $(\gamma^1\gamma^2)^2=-1$, these components change sign under $\phi\mapsto\phi+2\pi$. This is the lift of a full rotation to the [spin structure](riemannian-geometry.md#spin-structure) extending over the disk; the polar frame itself does not extend over the origin. In a Cartesian frame the same [parallel spinors](#parallel-spinor) have constant components.

#### Spinor curvature identity

↑ **Parent:** [Spinor covariant derivative](#spinor-covariant-derivative)

The [spinor covariant derivative](#spinor-covariant-derivative) has curvature $d\Omega+\Omega\wedge\Omega=\tfrac14R_{AB}\gamma^{AB}$, since the spin representation preserves the Lorentz algebra bracket. In a coordinate basis with the [torsion-free connection](fiber-bundle.md#torsion-free-connection), antisymmetric second covariant derivatives therefore give the displayed commutator. With unit-weight antisymmetrization, $\nabla_{[\mu}\nabla_{\nu]}\psi=\tfrac18R_{\mu\nu AB}\gamma^{AB}\psi=\tfrac1{16}R_{\mu\nu AB}[\gamma^A,\gamma^B]\psi$. A noncoordinate frame requires its frame-commutator correction when using the operator commutator; the full second covariant derivative includes that correction automatically.

##### Killing-spinor integrability with rescaled gamma matrices

↑ **Parent:** [Spinor curvature identity](#spinor-curvature-identity)

For $\{\gamma_a,\gamma_b\}=2s g_{ab}$, the compatible [spinor covariant derivative](#spinor-covariant-derivative) has curvature $R_{abcd}\gamma^{cd}/(4s)$. The torsion-free connection preserves [Clifford multiplication](algebra.md#clifford-multiplication), so the mixed derivative terms cancel for $D_a=\nabla_a+c\gamma_a$. Its integrability is therefore $(R_{abcd}\gamma^{cd}+8s c^2\gamma_{ab})\epsilon=0$. Changing antisymmetrization weight cannot change the relative coefficient. The common normalization uses $s=1$; $s=2$ gives the coefficient $16c^2$.

###### Maximal Killing spinors force constant negative curvature

↑ **Parent:** [Killing-spinor integrability with rescaled gamma matrices](#killing-spinor-integrability-with-rescaled-gamma-matrices)

Four independent complex Dirac solutions in four dimensions span each [spinor](algebra.md#spinor) fibre, because a connection-parallel solution is determined by its value at one point. Their integrability operator must therefore vanish on the whole fibre. Independence of the six Clifford bivectors then gives the displayed constant-curvature tensor and $R_{ab}=-12s c^2g_{ab}$. When $c>0$, the [Ricci tensor](general-relativity.md#ricci-tensor) is automatically nondegenerate.

##### Einstein tensor contraction of spin curvature

↑ **Parent:** [Spinor curvature identity](#spinor-curvature-identity)

For the torsion-free [spin connection](#spin-connection) with $[\nabla_\nu,\nabla_\rho]=R_{\nu\rho ab}\gamma^{ab}/4$, Clifford expansion and the [first Bianchi identity](general-relativity.md#first-bianchi-identity) give $\gamma^{\mu\nu\rho}R_{\nu\rho ab}\gamma^{ab}=4R^\mu{}_\lambda\gamma^\lambda-2R\gamma^\mu$. Thus the antisymmetric double derivative equals $G^\mu{}_\lambda\gamma^\lambda/2$. This is the shared algebra behind quadratic-order [minimal four-dimensional supergravity](supersymmetry.md#minimal-four-dimensional-supergravity) invariance and the [Nester two-form](general-relativity.md#nester-two-form) divergence.

<h2 id="cartan-s-first-structure-equation">Cartan's first structure equation</h2>

↑ **Parent:** [Connection 1-form](connection-1-form.md)

Cartan's first structure equation is

$$
T^a=d\theta^a+\omega^a{}_b\wedge\theta^b.
$$

For the torsion-free [Levi-Civita connection](general-relativity.md#levi-civita-connection), $T^a=0$.

<h2 id="cartan-s-second-structure-equation">Cartan's second structure equation</h2>

↑ **Parent:** [Connection 1-form](connection-1-form.md)

Cartan's second structure equation defines the curvature forms by

$$
\mathcal R^a{}_b=d\omega^a{}_b+\omega^a{}_c\wedge\omega^c{}_b.
$$

## Curvature 2-form

↑ **Parent:** [Connection 1-form](connection-1-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Curvature_2-form)

The curvature two-forms are

$$
\mathcal R^a{}_b=d\omega^a{}_b+\omega^a{}_c\wedge\omega^c{}_b
=\frac12R^a{}_{bcd}\theta^c\wedge\theta^d.
$$

### Cartan curvature forms for a static spherical metric

↑ **Parent:** [Curvature 2-form](#curvature-2-form)

In the exterior orthonormal coframe $E^0=\sqrt Vdt$, $E^1=dr/\sqrt V$, $E^2=rd\theta$, $E^3=r\sin\theta d\phi$, use $\Omega^a{}_b=\tfrac12R^a{}_{bcd}E^c\wedge E^d$. The independent mixed-index [curvature 2-forms](#curvature-2-form) are $\Omega^0{}_1=-V''E^0\wedge E^1/2$, $\Omega^0{}_A=-V'E^0\wedge E^A/(2r)$, $\Omega^1{}_A=-V'E^1\wedge E^A/(2r)$ for $A=2,3$, and $\Omega^2{}_3=(1-V)E^2\wedge E^3/r^2$. The orthonormal [Ricci tensor](general-relativity.md#ricci-tensor) is diagonal with entries $V''/2+V'/r$, $-V''/2-V'/r$, and twice $(1-V-rV')/r^2$. The [Einstein field equations](general-relativity.md#einstein-field-equations) with negative [cosmological constant](cosmology.md#cosmological-constant) then give $V=1-2M/r+r^2/l^2$.

// Target: general-relativity.bigb

### Diagonal curvature operator

↑ **Parent:** [Curvature 2-form](#curvature-2-form)

The curvature operator is diagonal in an orthonormal coframe $\{e^a\}$ when every [curvature 2-form](#curvature-2-form) satisfies $\mathcal R^{ab}=K_{ab}e^a\wedge e^b$. Its matrix on the corresponding basis of [2-forms](differential-form.md#2-form) is then diagonal.

#### Diagonal curvature operator implies diagonal Ricci tensor

↑ **Parent:** [Diagonal curvature operator](#diagonal-curvature-operator)

If $\mathcal R^{ab}$ is proportional to $e^a\wedge e^b$ for every pair, then a curvature component can be nonzero only when its two index pairs describe the same coordinate two-plane. The contraction $R_{bd}=R^a{}_{bad}$ therefore vanishes for $b\ne d$, so the [Ricci tensor](general-relativity.md#ricci-tensor) is diagonal in the same frame.

## ↑ Ancestors (6)

1. [Orthonormal coframe in spacetime](general-relativity.md#orthonormal-coframe-in-spacetime)
2. [Orthonormal frame in spacetime](general-relativity.md#orthonormal-frame-in-spacetime)
3. [General relativity](general-relativity.md)
4. [Branches of physics](physics.md#branches-of-physics)
5. [Physics](physics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (22)

- [Cartan curvature of a planar warped spacetime](general-relativity.md#cartan-curvature-of-a-planar-warped-spacetime)
- [Curvature of a conformally Euclidean metric](general-relativity.md#curvature-of-a-conformally-euclidean-metric)
- [Curvature of a diagonal plane wave in Rosen coordinates](general-relativity.md#curvature-of-a-diagonal-plane-wave-in-rosen-coordinates)
- [First-order three-dimensional gravity](general-relativity.md#first-order-three-dimensional-gravity)
- [Flat linearized metric perturbations are locally pure gauge](general-relativity.md#flat-linearized-metric-perturbations-are-locally-pure-gauge)
- [Lorentzian connection-form antisymmetry](#lorentzian-connection-form-antisymmetry)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-63.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-58.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-58.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-14.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-55.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-55.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-55.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-49.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-309.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-309.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-309.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-309.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-309.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-309.md#3/c/solution)
