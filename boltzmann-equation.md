# Boltzmann equation

↑ **Parent:** [Statistical physics](statistical-physics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boltzmann_equation)

The Boltzmann equation evolves a phase-space distribution by balancing free streaming, external forces, and collisions.

**Table of contents**

- [Renormalized Boltzmann solution](#renormalized-boltzmann-solution)
- [Hydrodynamic limit of the Boltzmann equation](#hydrodynamic-limit-of-the-boltzmann-equation)
- [Spatially homogeneous Boltzmann equation](#spatially-homogeneous-boltzmann-equation)
- [Nonlinear Boltzmann collision operator](#nonlinear-boltzmann-collision-operator)
  - [Dissipation form of the linearized Boltzmann operator](#dissipation-form-of-the-linearized-boltzmann-operator)
  - [Grad angular cutoff](#grad-angular-cutoff)
  - [Weak Boltzmann collision identity](#weak-boltzmann-collision-identity)
- [Local Maxwellian](#local-maxwellian)
  - [Expanding Gaussian solution of the Boltzmann equation](#expanding-gaussian-solution-of-the-boltzmann-equation)
- [Boltzmann H functional](#boltzmann-h-functional)
  - [Boltzmann entropy dissipation](#boltzmann-entropy-dissipation)
  - [H-theorem](#h-theorem)
- [Maxwell molecule collision operator](#maxwell-molecule-collision-operator)
  - [Collision invariant](#collision-invariant)
  - [Bobylev identity](#bobylev-identity)
    - [Fourier distance of order two](#fourier-distance-of-order-two)
      - [Fourier nonexpansion for Maxwell molecules](#fourier-nonexpansion-for-maxwell-molecules)
  - [Angular exchange for elastic collisions](#angular-exchange-for-elastic-collisions)
- [Linear Boltzmann equation](#linear-boltzmann-equation)
  - [Order preservation for the linear Boltzmann equation](#order-preservation-for-the-linear-boltzmann-equation)
  - [Normalized velocity-reset collision operator](#normalized-velocity-reset-collision-operator)
    - [Weighted Hilbert structure of velocity-reset relaxation](#weighted-hilbert-structure-of-velocity-reset-relaxation)
      - [Exact spectral gap of normalized velocity relaxation](#exact-spectral-gap-of-normalized-velocity-relaxation)
    - [Integrable Volterra solution for normalized velocity relaxation](#integrable-volterra-solution-for-normalized-velocity-relaxation)
    - [Normalized velocity-reset projection](#normalized-velocity-reset-projection)
  - [Volterra series for the linear Boltzmann equation](#volterra-series-for-the-linear-boltzmann-equation)
  - [Boltzmann Volterra operator](#boltzmann-volterra-operator)
  - [Damped free-transport evolution](#damped-free-transport-evolution)
  - [Linear Boltzmann collision operator](#linear-boltzmann-collision-operator)
    - [Rank-one gain on bounded continuous functions](#rank-one-gain-on-bounded-continuous-functions)
- [Relativistic kinetic theory](#relativistic-kinetic-theory)
  - [One-particle distribution function](#one-particle-distribution-function)
    - [Photon energy density](#photon-energy-density)
  - [Kinetic stress-energy tensor](#kinetic-stress-energy-tensor)
- [Boltzmann hierarchy](#boltzmann-hierarchy)

## Renormalized Boltzmann solution

↑ **Parent:** [Boltzmann equation](boltzmann-equation.md)

A weak solution framework in which a suitable nonlinear transform $\beta(f)$ satisfies a transport equation with transformed collision source $\beta'(f)Q(f,f)$, interpreted with the required integrability and possible framework-dependent defect terms. Renormalization addresses distributions whose raw collision term is not integrable enough to support the ordinary weak formulation. This is different from a classical smooth solution and does not by itself imply smooth global well-posedness.

## Hydrodynamic limit of the Boltzmann equation

↑ **Parent:** [Boltzmann equation](boltzmann-equation.md)

In a scaling $\partial_tf+v\cdot\nabla_xf=\varepsilon^{-1}Q(f,f)$ with small [Knudsen number](kinetic-theory.md#knudsen-number), the leading collision balance formally forces a [local Maxwellian](#local-maxwellian). The conserved moments then give the [Euler equations](euler-equations-for-an-inviscid-fluid.md) with a monatomic ideal-gas closure. The next nonequilibrium correction produces viscous and heat-conduction terms. These substitutions are formal: rigorous limits need uniform estimates, initial and boundary conditions, and sufficient convergence.

## Spatially homogeneous Boltzmann equation

↑ **Parent:** [Boltzmann equation](boltzmann-equation.md)

When the velocity distribution is independent of position and there are no forces, the [free transport equation](transport-equation.md#free-transport-equation) contributes zero and only collisions evolve $f$. For a bounded cutoff kernel, $\|Q(f,g)\|_1\leq C\|f\|_1\|g\|_1$ gives local existence and uniqueness by the [Banach fixed-point theorem](analysis.md#contraction-mapping-theorem). Positivity and mass conservation bound the norm and permit global continuation in this particular model. Stronger kernels require moment or weighted estimates.

## Nonlinear Boltzmann collision operator

↑ **Parent:** [Boltzmann equation](boltzmann-equation.md)

For equal-mass [elastic collisions](classical-mechanics.md#elastic-collision), one reflection parametrization is $v'=v-((v-v_*)\cdot n)n$ and $v_*'=v_*+((v-v_*)\cdot n)n$. The fixed-$n$ transformation preserves pairwise [momentum](momentum.md), [kinetic energy](energy.md#kinetic-energy) and velocity-pair measure. A nonnegative kernel invariant under particle interchange and collision reversal yields a gain-loss operator. Its [weak Boltzmann collision identity](#weak-boltzmann-collision-identity) proves conservation and its entropy identity proves the [Boltzmann H theorem](#h-theorem). Unlike the [Maxwell molecule collision operator](#maxwell-molecule-collision-operator), this general kernel may depend on relative speed.

### Dissipation form of the linearized Boltzmann operator

↑ **Parent:** [Nonlinear Boltzmann collision operator](#nonlinear-boltzmann-collision-operator)

Write $f=M(1+h)$ around a fixed Maxwellian and expand the [nonlinear Boltzmann collision operator](#nonlinear-boltzmann-collision-operator) to first order. The [weak Boltzmann collision identity](#weak-boltzmann-collision-identity) gives the nonnegative dissipation form in $L^2(M\,dv)$, and polarization proves symmetry on an appropriate common domain. Its zero modes are the [collision invariants](#collision-invariant) when the scattering kernel is nondegenerate. A [spectral gap](linear-operator-theory.md#spectral-gap), and self-adjointness of an unbounded realization, require additional domain and kernel hypotheses.

### Grad angular cutoff

↑ **Parent:** [Nonlinear Boltzmann collision operator](#nonlinear-boltzmann-collision-operator)

The angular collision rate is integrable at each nonzero relative velocity, with any needed speed-growth bounds stated separately. This makes the separate gain and loss integrals available under suitable velocity integrability. Non-cutoff kernels can have infinite angular collision rate and require cancellation rather than the same naive gain-loss split.

### Weak Boltzmann collision identity

↑ **Parent:** [Nonlinear Boltzmann collision operator](#nonlinear-boltzmann-collision-operator)

Here $\Delta\psi=\psi(v')+\psi(v_*')-\psi(v)-\psi(v_*)$ is the pairwise collision change, not a [Laplace operator](partial-differential-equation.md#laplace-operator). Average over the two particle labels and use collision reversal to obtain the formula. Every [collision invariant](#collision-invariant) has $\Delta\psi=0$, giving mass, [momentum](momentum.md) and [kinetic energy](energy.md#kinetic-energy) conservation. A second symmetrization replaces $ff_*\Delta\psi/2$ by $(f'f_*'-ff_*)(-\Delta\psi)/4$.

## Local Maxwellian

↑ **Parent:** [Boltzmann equation](boltzmann-equation.md)

A Gaussian velocity profile at each position, with coefficients encoding local density, mean velocity and temperature. Its logarithm is a [linear combination](vector-space.md#linear-combination) of [collision invariants](#collision-invariant), so its collision term vanishes pointwise in position. Transport need not vanish: the coefficients must also satisfy their transport equations for a [local Maxwellian](#local-maxwellian) to solve the full [Boltzmann equation](boltzmann-equation.md).

### Expanding Gaussian solution of the Boltzmann equation

↑ **Parent:** [Local Maxwellian](#local-maxwellian)

This spatially nonconstant [local Maxwellian](#local-maxwellian) is constant along free [characteristic curves](transport-equation.md#characteristic-curve). Its collision term vanishes by the [collision invariants](#collision-invariant), so it solves the full [Boltzmann equation](boltzmann-equation.md). It is positive, rapidly decaying and integrable in [phase space](hamiltonian-mechanics.md#phase-space). Completing its velocity square gives local mean $\alpha tx/(\beta+\alpha t^2)$ and local variance proportional to $(\beta+\alpha t^2)^{-1}$, while its spatial profile broadens with time.

## Boltzmann H functional

↑ **Parent:** [Boltzmann equation](boltzmann-equation.md)

The [integral](integral.md) uses $0\log0=0$ when it is defined. For the [Boltzmann equation](boltzmann-equation.md), the [Boltzmann H theorem](#h-theorem) makes it nonincreasing under suitable regularity and integrability. This functional is distinct from the microstate-counting [Boltzmann entropy](entropy.md#boltzmann-s-entropy-formula); the physical kinetic [entropy](entropy.md) has the opposite sign.

### Boltzmann entropy dissipation

↑ **Parent:** [Boltzmann H functional](#boltzmann-h-functional)

Put $A=f'f_*'$ and $B_0=ff_*$. The [weak Boltzmann collision identity](#weak-boltzmann-collision-identity) applied to $\log f$ gives $H'(t)=-\int D(f)\,dx$ when transport boundary fluxes vanish. Monotonicity of the logarithm makes every integrand nonnegative. For positive sufficiently regular distributions and nondegenerate angular scattering, zero dissipation forces $\log f$ to be a [collision invariant](#collision-invariant), hence $f$ to be a [local Maxwellian](#local-maxwellian). This equality statement alone does not establish convergence rates.

### H-theorem

↑ **Parent:** [Boltzmann H functional](#boltzmann-h-functional)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/H-theorem)

For the normalized isotropic [Maxwell molecule collision operator](#maxwell-molecule-collision-operator), put $a=f'f_*'$ and $b=ff_*$. The [integral](integral.md) is over position, both velocities and collision direction. The symmetrized weak identity yields the displayed [derivative](calculus.md#derivative) of the [Boltzmann H functional](#boltzmann-h-functional). It is nonpositive because $(a-b)\log(a/b)\geq0$ for positive $a,b$. Spatial transport contributes only a boundary flux, which must vanish for the total-space inequality.

## Maxwell molecule collision operator

↑ **Parent:** [Boltzmann equation](boltzmann-equation.md)

For the normalized isotropic cutoff model, collisions redistribute the direction of relative velocity uniformly while keeping its length. With center $C=(v+v_*)/2$ and relative speed $r=|v-v_*|$, outgoing velocities are $C\pm r\sigma/2$. [Momentum](momentum.md) and [kinetic energy](energy.md#kinetic-energy) are preserved, and the collision rate has no relative-speed factor. The displayed operator uses unit total angular rate. General Maxwell molecule kernels can have nonconstant angular dependence.

### Collision invariant

↑ **Parent:** [Maxwell molecule collision operator](#maxwell-molecule-collision-operator)

A [collision invariant](#collision-invariant) has an unchanged pairwise sum in every allowed [elastic collision](classical-mechanics.md#elastic-collision). The functions $1$, each velocity coordinate, and $|v|^2$ encode mass, [momentum](momentum.md) and energy. Symmetrized weak collision identities then give zero moments of the collision operator against these functions. Under standard regularity assumptions, the invariants form their five-dimensional linear span in three velocity dimensions.

### Bobylev identity

↑ **Parent:** [Maxwell molecule collision operator](#maxwell-molecule-collision-operator)

For the [Maxwell molecule collision operator](#maxwell-molecule-collision-operator) and the [Fourier transform](fourier-transform.md) with exponent $-i\xi\cdot v$, put $\xi^\pm=(\xi\pm|\xi|\sigma)/2$. The [angular exchange for elastic collisions](#angular-exchange-for-elastic-collisions), rotation invariance of spherical surface area and factorization of the two velocity [integrals](integral.md) give the displayed formula. This identity converts the collision [integral](integral.md) into a spherical average of products at two related frequencies.

#### Fourier distance of order two

↑ **Parent:** [Bobylev identity](#bobylev-identity)

For finite nonnegative measures with equal mass and first moment and finite second moments, the constant and linear terms of their [Fourier transforms](fourier-transform.md) cancel. Taylor's remainder bounds their difference by a constant times $|\xi|^2$, making this distance finite. Fourier uniqueness gives definiteness. The origin is excluded from the supremum; the quotient need not have a direction-independent limit there.

##### Fourier nonexpansion for Maxwell molecules

↑ **Parent:** [Fourier distance of order two](#fourier-distance-of-order-two)

Unit-mass solutions of the isotropic [Maxwell molecule collision operator](#maxwell-molecule-collision-operator) with matching first moments obey this comparison. The [Bobylev identity](#bobylev-identity), the Fourier bound by one, and $|\xi^+|^2+|\xi^-|^2=|\xi|^2$ give a scalar damped differential inequality. Its [integral](integral.md) form and the [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) yield nonexpansion in the [Fourier distance of order two](#fourier-distance-of-order-two). This does not alone establish strict contraction or equilibrium convergence.

### Angular exchange for elastic collisions

↑ **Parent:** [Maxwell molecule collision operator](#maxwell-molecule-collision-operator)

Write incoming relative velocity as $r\omega$ and outgoing relative velocity as $r\sigma$. For isotropic scattering, the product measure $dC\,r^2dr\,d\omega\,d\sigma$ is invariant under exchanging the two angular variables. This gives the pre/post-collision weak identities. Keeping $\sigma$ fixed and sending only the velocities to the outgoing pair is not invertible: that map discards the incoming angular direction.

## Linear Boltzmann equation

↑ **Parent:** [Boltzmann equation](boltzmann-equation.md)

A linear kinetic transport equation with velocity-integral gain $K_t$ and nonnegative loss coefficient $a$. Its characteristic integral formulation combines the [damped free-transport evolution](#damped-free-transport-evolution) with the [Boltzmann Volterra operator](#boltzmann-volterra-operator). A uniform square-integrable velocity kernel yields bounded gain on $L^2_{x,v}$ and a globally convergent [Volterra series for the linear Boltzmann equation](#volterra-series-for-the-linear-boltzmann-equation) on every finite time interval.

### Order preservation for the linear Boltzmann equation

↑ **Parent:** [Linear Boltzmann equation](#linear-boltzmann-equation)

Nonnegative gain kernels and positive damping preserve pointwise order. The [Volterra series for the linear Boltzmann equation](#volterra-series-for-the-linear-boltzmann-equation) has nonnegative terms when its initial datum is nonnegative. Applying this to the difference of two solutions proves comparison, with uniqueness identifying that difference with the positive series. This order property is distinct from positivity of a quadratic form on a [Hilbert space](hilbert-space.md).

### Normalized velocity-reset collision operator

↑ **Parent:** [Linear Boltzmann equation](#linear-boltzmann-equation)

Let $M\geq0$ have velocity [integral](integral.md) one, and $\rho(g)(x)=\int g(x,v)dv$. On phase-space $L^1$, the normalized relaxation collision operator is $B=P-I$, where $Pg=\rho(g)M$. It obeys $\|B\|\leq2$ because $\|Pg\|_1\leq\|g\|_1$. It preserves mass at each spatial position. The corresponding [linear Boltzmann equation](#linear-boltzmann-equation) combines this bounded collision operator with the [free-transport semigroup](transport-equation.md#free-transport-semigroup).

#### Weighted Hilbert structure of velocity-reset relaxation

↑ **Parent:** [Normalized velocity-reset collision operator](#normalized-velocity-reset-collision-operator)

For $M>0$ with [integral](integral.md) one, the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) makes the mass functional bounded on the weighted [Hilbert space](hilbert-space.md). The vector $M$ has [norm](normed-vector-space.md#norm) one, so the velocity-reset projection is the [orthogonal projection](hilbert-space.md#orthogonal-projection) onto its span. Consequently $L=\Pi-I$ is bounded and [self-adjoint](linear-operator-theory.md#self-adjoint-operator). This Hilbert geometry differs from the norm-one positive reset projection on phase-space $L^1$.

##### Exact spectral gap of normalized velocity relaxation

↑ **Parent:** [Weighted Hilbert structure of velocity-reset relaxation](#weighted-hilbert-structure-of-velocity-reset-relaxation)

For the [normalized velocity-reset collision operator](#normalized-velocity-reset-collision-operator) on the weighted [Hilbert space](hilbert-space.md), $L=\Pi-I$ vanishes on the equilibrium direction and equals $-I$ on its [orthogonal complement](hilbert-space.md#orthogonal-complement). The [spectral gap](linear-operator-theory.md#spectral-gap) is exactly one. Conservation of the projected component and the displayed energy identity give exact exponential decay of the remaining component; the full solution need not decay to zero.

#### Integrable Volterra solution for normalized velocity relaxation

↑ **Parent:** [Normalized velocity-reset collision operator](#normalized-velocity-reset-collision-operator)

For $E=L^1_{x,v}$, let $(\tau f)(t)=\int_0^tU_{t-s}(P-I)f(s)ds$. The [factorial bound for a Volterra iterate](analysis.md#factorial-bound-for-a-volterra-iterate) is $\|\tau^nf(t)\|_1\leq(2t)^n\sup_{s\leq t}\|f(s)\|_1/n!$. Thus the [Neumann series](banach-algebra.md#neumann-series) converges in $C([0,T];E)$ for every finite $T$ and solves $f=U_\cdot f_0+\tau f$. The same estimate applied to a difference proves uniqueness among locally time-bounded [integral](integral.md) solutions. The whole collision term remains inside this undamped [integral](integral.md), rather than absorbing loss into the free propagator.

#### Normalized velocity-reset projection

↑ **Parent:** [Normalized velocity-reset collision operator](#normalized-velocity-reset-collision-operator)

For a nonnegative normalized velocity density $M$, $Pg(x,v)=M(v)\int g(x,w)dw$ is a positive [norm](normed-vector-space.md#norm)-one projection on phase-space $L^1$. Normalization gives $P^2=P$. Its range consists of fields $a(x)M(v)$. This Banach-space projection need not be an [orthogonal projection](hilbert-space.md#orthogonal-projection) in unweighted $L^2$; no such assertion is needed for the $L^1$ collision estimates.

### Volterra series for the linear Boltzmann equation

↑ **Parent:** [Linear Boltzmann equation](#linear-boltzmann-equation)

The [factorial bound for a Volterra iterate](analysis.md#factorial-bound-for-a-volterra-iterate) gives convergence in the space of bounded strongly measurable $L^2$-valued functions on $[0,T]$. The sum solves $(I-\tau)f=F$, where $F=U_a(t,0)f_0$, and satisfies $\sup_{t\leq T}\|f(t)\|_2\leq e^{CT}\|f_0\|_2$. Applying the same iterate bound to a difference $g=\tau g$ proves uniqueness on every finite interval.

### Boltzmann Volterra operator

↑ **Parent:** [Linear Boltzmann equation](#linear-boltzmann-equation)

Combine the [damped free-transport evolution](#damped-free-transport-evolution) and the [linear Boltzmann collision operator](#linear-boltzmann-collision-operator) in a time-ordered [Bochner integral](measure-theory.md#bochner-integral). Its norm obeys $\|\tau f(t)\|_2\leq C\int_0^t\|f(s)\|_2ds$. This reduces the characteristic integral equation to $(I-\tau)f=U_a(t,0)f_0$.

### Damped free-transport evolution

↑ **Parent:** [Linear Boltzmann equation](#linear-boltzmann-equation)

For nonnegative measurable $a$, define $(U_a(t,s)g)(x,v)=e^{-\int_s^t a(r,x-v(t-r),v)dr}g(x-v(t-s),v)$. The shear preserves [Lebesgue measure](measure-theory.md#lebesgue-measure) and the multiplier lies in $[0,1]$, so this is a contraction on [Lp spaces](measure-theory.md#lp-space). Extended nonnegative integrals use $e^{-\infty}=0$. Characteristic local integrability gives the usual continuous trace at the starting time.

### Linear Boltzmann collision operator

↑ **Parent:** [Linear Boltzmann equation](#linear-boltzmann-equation)

The gain term integrates over the incoming velocity. If $C^2=\int\sup_{t,x}|k(t,x,v,v_*)|^2\,dv\,dv_*<\infty$, the [Hilbert-Schmidt kernel bound](compact-operator.md#hilbert-schmidt-kernel-bound) at each $x$ gives $\|K_tg\|_{L^2_{x,v}}\leq C\|g\|_{L^2_{x,v}}$, uniformly in time. The existence proof uses boundedness; kernel positivity is not needed for that estimate.

#### Rank-one gain on bounded continuous functions

↑ **Parent:** [Linear Boltzmann collision operator](#linear-boltzmann-collision-operator)

A bounded continuous factor $k_1$ and an integrable factor $k_2$ give a bounded velocity-integral gain on [bounded continuous functions](calculus.md#bounded-continuous-functions), with bound $\|Kf\|_\infty\leq\|k_1\|_\infty\|k_2\|_1\|f\|_\infty$. The [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) proves joint continuity of the velocity [integral](integral.md). Combined with damped transport, the [factorial bound for a Volterra iterate](analysis.md#factorial-bound-for-a-volterra-iterate) proves existence on arbitrary finite time slabs.

## Relativistic kinetic theory

↑ **Parent:** [Boltzmann equation](boltzmann-equation.md)

Relativistic kinetic theory describes particles by a scalar [phase-space distribution function](statistical-physics.md#phase-space-distribution-function) on the future mass shell. Its [Boltzmann equation](boltzmann-equation.md) uses geodesic streaming and a collision operator. Integrating its momentum moments supplies a [kinetic stress-energy tensor](#kinetic-stress-energy-tensor) and particle-number currents. An [orthonormal tetrad](general-relativity.md#orthonormal-frame-in-spacetime) makes the local momentum integrals identical in form to those of [special relativity](special-relativity.md).

### One-particle distribution function

↑ **Parent:** [Relativistic kinetic theory](#relativistic-kinetic-theory)

A scalar function on the future mass shell describing the expected particle count in a [phase-space distribution](statistical-physics.md#phase-space-distribution-function) cell. In a local [orthonormal tetrad](general-relativity.md#orthonormal-frame-in-spacetime), the number crossing a spacelike surface element is $f\,p^\mu d\Sigma_\mu\,d^3p/E$. On a constant-time slice it becomes $f\,d^3x\,d^3p$. Including degeneracy and phase-space normalization in $f$ gives the [stress-energy tensor](stress-energy-tensor.md) $T^{\mu\nu}=\int(d^3p/E)fp^\mu p^\nu$. Other conventions may put the degeneracy or $(2\pi)^{-3}$ explicitly in the measure.

#### Photon energy density

↑ **Parent:** [One-particle distribution function](#one-particle-distribution-function)

The temporal-temporal component of the photon [stress-energy tensor](stress-energy-tensor.md) in a local [orthonormal tetrad](general-relativity.md#orthonormal-frame-in-spacetime). For an isotropic [one-particle distribution function](#one-particle-distribution-function) expressed using comoving energy $\epsilon=aE$, it is $\bar\rho_\gamma=4\pi a^{-4}\int d\epsilon\,\epsilon^3\bar f(\epsilon)$. A thermal [photon temperature perturbation](cosmic-microwave-background-anisotropy.md#photon-temperature-perturbation) gives a first-order directional energy perturbation four times its fractional temperature change. Boundary conditions on the distribution justify this factor through [integration by parts](calculus.md#integration-by-parts).

### Kinetic stress-energy tensor

↑ **Parent:** [Relativistic kinetic theory](#relativistic-kinetic-theory)

The invariant future mass-shell measure is $d^3p/E$, up to fixed normalization factors absorbed in $f$. Its relation to the [Lorentz-invariant phase-space measure](quantum-scattering.md#lorentz-invariant-phase-space-measure) follows by integrating $2\theta(p^0)\delta(p_\mu p^\mu+m^2)\,d^4p$ over $p^0$ in a local [orthonormal tetrad](general-relativity.md#orthonormal-frame-in-spacetime). A particle carries [four-momentum](special-relativity.md#four-momentum) $p^\mu$ and crosses a local spatial surface with velocity $p^i/p^0$. Integrating the associated [momentum flux](mathematical-physics.md#momentum-flux) gives the displayed [stress-energy tensor](stress-energy-tensor.md). For [photons](quantum-mechanics.md#photon), $p^{\hat a}=E(1,\mathbf e)$ and $|\mathbf e|=1$.

## Boltzmann hierarchy

↑ **Parent:** [Boltzmann equation](boltzmann-equation.md)

Expanding an angular distribution in multipoles converts the Boltzmann equation into a hierarchy in which free streaming couples neighboring multipoles and collisions damp or source selected moments.

## ↑ Ancestors (4)

1. [Statistical physics](statistical-physics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (16)

- [Boltzmann-Grad limit](kinetic-theory.md#boltzmann-grad-limit)
- [Boltzmann H functional](#boltzmann-h-functional)
- [Expanding Gaussian solution of the Boltzmann equation](#expanding-gaussian-solution-of-the-boltzmann-equation)
- [Franck-Hertz repeated-loss collection model](energy-eigenvalue.md#franck-hertz-repeated-loss-collection-model)
- [Kinetic theory](kinetic-theory.md)
- [Knudsen number](kinetic-theory.md#knudsen-number)
- [Local Maxwellian](#local-maxwellian)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3.md#12c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-312.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-312.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-312.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-312.md#4/a/solution)
- [Solution](past-exam-of-the-particle-astrophysics-course-of-the-university-of-cambridge/2012/paper-1.md#2/solution)
- [Photon number current](statistical-physics.md#photon-number-current)
- [Relativistic kinetic theory](#relativistic-kinetic-theory)
