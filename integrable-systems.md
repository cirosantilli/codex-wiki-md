# Integrable systems

↑ **Parent:** [Branches of physics](physics.md#branches-of-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integrable_systems)

Integrable systems admit unusually rich exact structure such as Lax pairs, conserved quantities, and symmetry reductions.

**Table of contents**

- [Infinite-dimensional Hamiltonian integrability](#infinite-dimensional-hamiltonian-integrability)
- [Bäcklund transformation](#backlund-transformation)
- [Classical integrability](#classical-integrability)
- [Hirota's bilinear method](#hirota-s-bilinear-method)
- [Hirota tau function](#hirota-tau-function)
- [Periodic Toda lattice](#periodic-toda-lattice)
- [Sinh-Gordon equation](#sinh-gordon-equation)
- [Sine-Gordon equation](#sine-gordon-equation)
  - [Scaling symmetry of the sine-Gordon equation](#scaling-symmetry-of-the-sine-gordon-equation)
  - [One-soliton solution of the sine-Gordon equation in light-cone coordinates](#one-soliton-solution-of-the-sine-gordon-equation-in-light-cone-coordinates)
  - [Sine-Gordon breather](#sine-gordon-breather)
- [Painlevé III equation](#painleve-iii-equation)
- [Focusing nonlinear Schrodinger equation](#focusing-nonlinear-schrodinger-equation)
  - [Bright standing soliton of the focusing nonlinear Schrodinger equation](#bright-standing-soliton-of-the-focusing-nonlinear-schrodinger-equation)
- [Hamiltonian form of the cubic nonlinear Schrodinger equations](#hamiltonian-form-of-the-cubic-nonlinear-schrodinger-equations)
- [Defocusing nonlinear Schrödinger equation](#defocusing-nonlinear-schrodinger-equation)
  - [Linearizable Robin scattering for defocusing NLS](#linearizable-robin-scattering-for-defocusing-nls)
    - [Finite-horizon Robin spectral elimination](#finite-horizon-robin-spectral-elimination)
    - [Robin spectral determinant for defocusing NLS](#robin-spectral-determinant-for-defocusing-nls)
  - [Half-line NLS spectral functions](#half-line-nls-spectral-functions)
    - [Half-line NLS global relation](#half-line-nls-global-relation)
  - [No rapidly decaying standing wave for the defocusing cubic nonlinear Schrodinger equation](#no-rapidly-decaying-standing-wave-for-the-defocusing-cubic-nonlinear-schrodinger-equation)
  - [Dark soliton](#dark-soliton)
- [Korteweg-De Vries equation](#korteweg-de-vries-equation)
  - [First Hamiltonian structure of the KdV equation](#first-hamiltonian-structure-of-the-kdv-equation)
  - [Cylindrical KdV equation](#cylindrical-kdv-equation)
  - [Modified Korteweg-De Vries equation](#modified-korteweg-de-vries-equation)
    - [Half-line mKdV spectral global relation](#half-line-mkdv-spectral-global-relation)
    - [Miura transformation](#miura-transformation)
  - [KdV Schrodinger spectral problem](#kdv-schrodinger-spectral-problem)
    - [Jost solution](#jost-solution)
    - [KdV scattering data](#kdv-scattering-data)
      - [Time evolution of KdV scattering data](#time-evolution-of-kdv-scattering-data)
      - [Born approximation for a one-dimensional reflection coefficient](#born-approximation-for-a-one-dimensional-reflection-coefficient)
    - [Isospectrality of the KdV discrete spectrum](#isospectrality-of-the-kdv-discrete-spectrum)
      - [Evolution of a KdV discrete norming constant](#evolution-of-a-kdv-discrete-norming-constant)
  - [Soliton](#soliton)
    - [Multisoliton solution](#multisoliton-solution)
- [Inverse scattering transform](#inverse-scattering-transform)
  - [Scattering data](#scattering-data)
  - [Cauchy-kernel dressing for the KdV equation](#cauchy-kernel-dressing-for-the-kdv-equation)
    - [Finite-rank KdV dressing determinant](#finite-rank-kdv-dressing-determinant)
  - [Discrete scattering data](#discrete-scattering-data)
  - [Marchenko equation](#marchenko-equation)
    - [Rank-one Gelfand-Levitan-Marchenko kernel](#rank-one-gelfand-levitan-marchenko-kernel)
- [Poisson-commuting separated energies](#poisson-commuting-separated-energies)
- [Separable forced harmonic oscillators](#separable-forced-harmonic-oscillators)
- [Action variable of a shifted harmonic oscillator](#action-variable-of-a-shifted-harmonic-oscillator)
  - [Phase-plane area formula for an action variable](#phase-plane-area-formula-for-an-action-variable)
- [Compatibility condition for an overdetermined linear system](#compatibility-condition-for-an-overdetermined-linear-system)
- [Integrable partial differential equation](#integrable-partial-differential-equation)
  - [Harry Dym equation](#harry-dym-equation)
  - [Boussinesq equation](#boussinesq-equation)
- [Lax pair](#lax-pair)
  - [Volterra analyticity sectors for reverse-dispersion mKdV](#volterra-analyticity-sectors-for-reverse-dispersion-mkdv)
  - [Quadratic spectral Lax pair for zero-parameter Painlevé II](#quadratic-spectral-lax-pair-for-zero-parameter-painleve-ii)
  - [Volterra analyticity sectors for a half-line NLS Lax pair](#volterra-analyticity-sectors-for-a-half-line-nls-lax-pair)
  - [Lax pair for the Bogomolny equations](#lax-pair-for-the-bogomolny-equations)
  - [Lax equation preserves the spectrum](#lax-equation-preserves-the-spectrum)
  - [Monodromy matrix](#monodromy-matrix)
  - [Spectral parameter](#spectral-parameter)
  - [Lax pair for the anti-self-dual Yang-Mills equations](#lax-pair-for-the-anti-self-dual-yang-mills-equations)
    - [Euclidean complex-coordinate anti-self-dual Lax pair](#euclidean-complex-coordinate-anti-self-dual-lax-pair)
  - [Airy equation](#airy-equation)
    - [Cubic dispersion symmetry with negative transport](#cubic-dispersion-symmetry-with-negative-transport)
    - [Gauge reduction of a third-order half-line equation](#gauge-reduction-of-a-third-order-half-line-equation)
    - [Backward-sign Airy half-line global relation](#backward-sign-airy-half-line-global-relation)
      - [Two boundary traces for reverse-dispersion Airy flow](#two-boundary-traces-for-reverse-dispersion-airy-flow)
    - [Mixed-boundary Airy energy principle](#mixed-boundary-airy-energy-principle)
    - [Linear dispersive Stokes equation](#linear-dispersive-stokes-equation)
      - [Spatial root splitting for the dispersive Stokes resolvent](#spatial-root-splitting-for-the-dispersive-stokes-resolvent)
        - [Stokes resolvent kernel with advection](#stokes-resolvent-kernel-with-advection)
          - [Half-line Stokes solution with a boundary derivative](#half-line-stokes-solution-with-a-boundary-derivative)
    - [Airy resolvent kernel](#airy-resolvent-kernel)
      - [Airy half-line solution with prescribed boundary derivative](#airy-half-line-solution-with-prescribed-boundary-derivative)
  - [AKNS Lax pair for the nonlinear Schrodinger equation](#akns-lax-pair-for-the-nonlinear-schrodinger-equation)
  - [Isospectral Lax equation](#isospectral-lax-equation)
    - [Third-order Boussinesq Lax pair](#third-order-boussinesq-lax-pair)
    - [Trace invariants of a Lax equation](#trace-invariants-of-a-lax-equation)
    - [Finite Volterra lattice](#finite-volterra-lattice)
      - [Zero-diagonal Jacobi Lax pair for the finite Volterra lattice](#zero-diagonal-jacobi-lax-pair-for-the-finite-volterra-lattice)
    - [Periodic KdV transfer matrix](#periodic-kdv-transfer-matrix)
  - [Zero-curvature condition](#zero-curvature-condition)
  - [Global relation for the half-line free Schrodinger equation](#global-relation-for-the-half-line-free-schrodinger-equation)
- [Tzitzeica equation](#tzitzeica-equation)
  - [Scaling-invariant reduction of the Tzitzeica equation](#scaling-invariant-reduction-of-the-tzitzeica-equation)

## Infinite-dimensional Hamiltonian integrability

↑ **Parent:** [Integrable systems](integrable-systems.md)

For a field evolving by a [Hamiltonian](classical-mechanics.md#hamiltonian) [partial differential equation](partial-differential-equation.md), infinite-dimensional integrability combines sufficiently rich commuting conservation laws with a mechanism such as the [inverse scattering transform](#inverse-scattering-transform) or a spectral coordinate system that linearizes evolution. [Lax equations](#isospectral-lax-equation) supply spectral invariants; [Lenard-Magri recursions](symplectic-geometry.md#lenard-magri-recursion) supply commuting [Hamiltonians](classical-mechanics.md#hamiltonian) when their solvability conditions hold. Infinite many [conserved quantities](classical-mechanics.md#conserved-quantity) alone do not prove completeness or an infinite-dimensional action-angle theorem: the [function](function.md) space, [boundary conditions](differential-equation.md#boundary-condition) and analytic independence all matter.

<h2 id="backlund-transformation">Bäcklund transformation</h2>

↑ **Parent:** [Integrable systems](integrable-systems.md)

A parameter-dependent system of differential relations maps a solution of one differential equation to a solution of another, or to a new solution of the same equation. Compatibility of the relations supplies the equations of motion. Integration constants select a particular transformed field. The [Sine-Gordon Bäcklund transformation](scalar-field-theory.md#sine-gordon-backlund-transformation) is an example of an auto-transformation and also generates [conserved currents](quantum-field-theory.md#conserved-current).

## Classical integrability

↑ **Parent:** [Integrable systems](integrable-systems.md)

For a finite-dimensional [Hamiltonian system](classical-mechanics.md#hamiltonian-system), integrability is normally expressed by enough independent first integrals in mutual [Poisson bracket](classical-mechanics.md#poisson-bracket) involution. In classical field theories, an infinite hierarchy of compatible [conserved quantities](classical-mechanics.md#conserved-quantity) is the corresponding structure. For [Sine-Gordon theory](scalar-field-theory.md#sine-gordon-theory), [Bäcklund transformations](#backlund-transformation) generate local [conservation laws](physics.md#conservation-law) and explicit soliton solutions. Conservation of arbitrary quantities alone should not be confused with proof of their [Hamiltonian](classical-mechanics.md#hamiltonian) involution.

<h2 id="hirota-s-bilinear-method">Hirota's bilinear method</h2>

↑ **Parent:** [Integrable systems](integrable-systems.md)

An exact-solution method that transforms a nonlinear [partial differential equation](partial-differential-equation.md) into equations bilinear in auxiliary [Hirota tau functions](#hirota-tau-function). Finite exponential expansions of the [Hirota tau functions](#hirota-tau-function) produce [soliton](#soliton) families. The auxiliary exponential coefficients need not all be positive.

## Hirota tau function

↑ **Parent:** [Integrable systems](integrable-systems.md)

An auxiliary function used in [Hirota's bilinear method](#hirota-s-bilinear-method) to encode a solution of an [integrable partial differential equation](#integrable-partial-differential-equation). Products and ratios of tau functions replace nonlinear field variables; their differential equations become bilinear. In a [Sine-Gordon multisoliton tau representation](scalar-field-theory.md#sine-gordon-multisoliton-tau-representation), two real tau functions encode the field as a continuous $4\arg(f+ig)$.

## Periodic Toda lattice

↑ **Parent:** [Integrable systems](integrable-systems.md)

The periodic Hamiltonian chain $H=\tfrac12\sum p_i^2+\sum e^{q_i-q_{i+1}}$, with cyclic indices, is a [Liouville integrable](classical-mechanics.md#integrable-hamiltonian-system) system. Exponentials of neighbouring coordinate differences lead to a [Lax pair](#lax-pair) and conserved characteristic coefficients.

## Sinh-Gordon equation

↑ **Parent:** [Integrable systems](integrable-systems.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sinh-Gordon_equation)

The sinh-Gordon equation is an integrable nonlinear wave equation. Under the one-dimensional reduction $u=u(x)$ with $z=x+iy$, it becomes

$$
u_{xx}=2\sinh(2u).
$$

Writing $\phi=2u$ gives $\phi''=4\sinh\phi$ and the first integral

$$
\frac12(\phi')^2-4\cosh\phi=\text{constant}.
$$

## Sine-Gordon equation

↑ **Parent:** [Integrable systems](integrable-systems.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sine-Gordon_equation)

In light-cone coordinates, the sine-Gordon equation can be written $u_{XT}=\sin u$. Its [inverse scattering transform](#inverse-scattering-transform), [solitons](#soliton), breathers, and scaling symmetries make it an [integrable system](integrable-systems.md).

### Scaling symmetry of the sine-Gordon equation

↑ **Parent:** [Sine-Gordon equation](#sine-gordon-equation)

The transformations

$$
(X,T,u)\longmapsto(e^sX,e^{-s}T,u)
$$

form a one-parameter [Lie point symmetry](partial-differential-equation.md#lie-point-symmetry) of $u_{XT}=\sin u$. The product $z=XT$ is a [similarity variable](partial-differential-equation.md#similarity-variable), and a [group-invariant solution](partial-differential-equation.md#group-invariant-solution) $u=F(z)$ satisfies

$$
zF''+F'=\sin F.
$$

### One-soliton solution of the sine-Gordon equation in light-cone coordinates

↑ **Parent:** [Sine-Gordon equation](#sine-gordon-equation)

For every $l>0$,

$$
u(X,T)=4\arctan\exp\left(-2lX-\frac{T}{2l}\right)
$$

solves $u_{XT}=\sin u$. The scaling $(X,T)\mapsto(e^sX,e^{-s}T)$ transforms $l$ by multiplication with $e^{-s}$.

### Sine-Gordon breather

↑ **Parent:** [Sine-Gordon equation](#sine-gordon-equation)

A sine-Gordon breather is a spatially localized solution that is periodic in time and can be interpreted through a complex-conjugate pair of discrete scattering eigenvalues.

This is a [breather](classical-field-theory-soliton.md#breather) of the [Sine-Gordon equation](#sine-gordon-equation); the general breather concept also occurs in other nonlinear systems.

<h2 id="painleve-iii-equation">Painlevé III equation</h2>

↑ **Parent:** [Integrable systems](integrable-systems.md)

The third Painlevé equation is the nonlinear second-order [ordinary differential equation](differential-equation.md#ordinary-differential-equation)

$$
w''=\frac{(w')^2}{w}-\frac{w'}z
+\frac{\alpha w^2+\beta}{z}
+\gamma w^3+\frac\delta w.
$$

The substitution $w=e^{iF}$ in the [scaling reduction of the sine-Gordon equation](#scaling-symmetry-of-the-sine-gordon-equation) gives the parameter choice $(\alpha,\beta,\gamma,\delta)=(1/2,-1/2,0,0)$.

## Focusing nonlinear Schrodinger equation

↑ **Parent:** [Integrable systems](integrable-systems.md)

The focusing cubic [nonlinear Schrödinger equation](partial-differential-equation.md#nonlinear-schrodinger-equation) has the normalization

$$
i\psi_t+\psi_{xx}+2|\psi|^2\psi=0,
$$

the positive cubic term focuses the field and permits bright solitons on zero background.

### Bright standing soliton of the focusing nonlinear Schrodinger equation

↑ **Parent:** [Focusing nonlinear Schrodinger equation](#focusing-nonlinear-schrodinger-equation)

For every $\kappa>0$ and $x_0\in\mathbb R$,

$$
\psi(x,t)=\kappa e^{i\kappa^2t}
\operatorname{sech}(\kappa(x-x_0))
$$

solves $i\psi_t+\psi_{xx}+2|\psi|^2\psi=0$ and decays rapidly as $|x|\to\infty$.

## Hamiltonian form of the cubic nonlinear Schrodinger equations

↑ **Parent:** [Integrable systems](integrable-systems.md)

The focusing and defocusing equations

$$
i\psi_t+\psi_{xx}\mathbin{\pm}2|\psi|^2\psi=0
$$

have Hamiltonians

$$
H_\pm=\int_{\mathbb R}\left(|\psi_x|^2\mp|\psi|^4\right)dx
$$

under the convention $i\psi_t=\delta H_\pm/\delta\overline\psi$.

<h2 id="defocusing-nonlinear-schrodinger-equation">Defocusing nonlinear Schrödinger equation</h2>

↑ **Parent:** [Integrable systems](integrable-systems.md)

Writing a defocusing nonlinear Schrödinger field as $\psi=\sqrt\rho\,e^{iS}$ turns it into a continuity equation for $\rho$ and a velocity equation for $v=S_x$, including a quantum-pressure term.

In a common normalization, the defocusing case is $i\psi_t+\psi_{xx}-2|\psi|^2\psi=0$. The sign distinguishes it from the focusing [nonlinear Schrödinger equation](partial-differential-equation.md#nonlinear-schrodinger-equation).

### Linearizable Robin scattering for defocusing NLS

↑ **Parent:** [Defocusing nonlinear Schrödinger equation](#defocusing-nonlinear-schrodinger-equation)

For the [Robin boundary condition](differential-equation.md#robin-boundary-condition) $q_x(0,t)=cq(0,t)$ with real $c$, the time [Lax pair](#lax-pair) has a diagonal-conjugation symmetry under $k\mapsto-k$. It implies $A(-k)=A(k)$ and $B(-k)=-h(k)B(k)$. Together with the [half-line NLS global relation](#half-line-nls-global-relation), this eliminates unknown boundary scattering from an equivalent [Riemann-Hilbert problem](differential-equation.md#riemann-hilbert-problem) determined by the initial data and $c$.

#### Finite-horizon Robin spectral elimination

↑ **Parent:** [Linearizable Robin scattering for defocusing NLS](#linearizable-robin-scattering-for-defocusing-nls)

Here $\Gamma=B^\sharp/(ad)$ and $\Delta=\mathcal D/(2k+ic)$. The difference follows algebraically from the [half-line NLS global relation](#half-line-nls-global-relation) and the Robin symmetry. Multiplication by the spatial-temporal jump factor gives $e^{2ikx-4ik^2(T-t)}$, decaying in the second quadrant for $t<T$. A triangular analytic change of the [Riemann-Hilbert problem](differential-equation.md#riemann-hilbert-problem) removes this finite-horizon defect while retaining the reconstruction and transferring all genuine pole information to the known determinant. No unproved large-time decay of the boundary values is needed.

#### Robin spectral determinant for defocusing NLS

↑ **Parent:** [Linearizable Robin scattering for defocusing NLS](#linearizable-robin-scattering-for-defocusing-nls)

The effective boundary coefficient is $\widetilde\Gamma=-(2k-ic)b^\sharp(-k)/(a\mathcal D)$. All its ingredients come from initial scattering and the [Robin boundary condition](differential-equation.md#robin-boundary-condition). Genuine zeros produce pole data; common zeros in numerator and denominator can instead be removable. It is incorrect to assert absence of boundary poles for every real Robin parameter.

### Half-line NLS spectral functions

↑ **Parent:** [Defocusing nonlinear Schrödinger equation](#defocusing-nonlinear-schrodinger-equation)

Initial scattering gives $s$ and boundary-time scattering gives $S$. The defocusing reduction and unit determinants give the displayed matrix forms. The initial functions $a,b$ are analytic in the upper half-plane, while the boundary functions $A,B$ are bounded in the first and third quadrants. Their finite-horizon compatibility is the [half-line NLS global relation](#half-line-nls-global-relation).

#### Half-line NLS global relation

↑ **Parent:** [Half-line NLS spectral functions](#half-line-nls-spectral-functions)

Evaluating the [Lax pair](#lax-pair) connection formula at $(0,T)$ gives $S^{-1}s=e^{2ik^2T\widehat\sigma_3}\mu_3(0,T,k)$. The upper off-diagonal entry is the displayed relation, where $c_T=[\mu_3(0,T)]_{12}$ is analytic in the upper half-plane and is $O(1/k)$. A finite-time relation must retain this final-state term.

### No rapidly decaying standing wave for the defocusing cubic nonlinear Schrodinger equation

↑ **Parent:** [Defocusing nonlinear Schrödinger equation](#defocusing-nonlinear-schrodinger-equation)

For $\psi=e^{-iEt}f(x)$ with real $f$, the defocusing equation $i\psi_t+\psi_{xx}-2|\psi|^2\psi=0$ has first integral

$$
(f')^2=f^4-Ef^2.
$$

A nonzero smooth function tending to zero at both infinities cannot satisfy this identity: a nonzero extremum requires $f^2=E>0$, but then the right side is negative for sufficiently small nonzero $f$.

### Dark soliton

↑ **Parent:** [Defocusing nonlinear Schrödinger equation](#defocusing-nonlinear-schrodinger-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dark_soliton)

For the normalization

$$
-2i\psi_t=\psi_{xx}+(1-|\psi|^2)\psi,
$$

a dark soliton of speed $0\leq U<1/\sqrt2$ is

$$
\psi_0(\xi)=
\sqrt{1-2U^2}\,
\tanh\left(\frac{\sqrt{1-2U^2}}{\sqrt2}\xi\right)
+i\sqrt2U,
\qquad \xi=x-Ut.
$$

## Korteweg-De Vries equation

↑ **Parent:** [Integrable systems](integrable-systems.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Korteweg–De_Vries_equation)

The Korteweg-De Vries equation

$$
u_t-6uu_x+u_{xxx}=0
$$

is an integrable nonlinear dispersive equation. Its sign convention here admits negative solitary waves.

### First Hamiltonian structure of the KdV equation

↑ **Parent:** [Korteweg-De Vries equation](#korteweg-de-vries-equation)

One normalization of the first [Hamiltonian](classical-mechanics.md#hamiltonian) structure uses the constant differential [Poisson operator](symplectic-geometry.md#poisson-operator) $J=-2\partial_x$. For [functionals](calculus-of-variations.md#functional) with [variational derivatives](classical-mechanics.md#variational-derivative) $f,g$, its [Poisson bracket](classical-mechanics.md#poisson-bracket) is $\int fJg\,dx=-2\int fg'\,dx$ under periodic or vanishing-boundary conventions. Thus the field bracket is $\{u(x),u(y)\}=-2\partial_x\delta(x-y)$. The factor and sign change with normalization; the constant first-order operator is the invariant structural feature.

### Cylindrical KdV equation

↑ **Parent:** [Korteweg-De Vries equation](#korteweg-de-vries-equation)

The [cylindrical KdV equation](#cylindrical-kdv-equation) in this normalization is $q_t+q_{xxx}+qq_x+q/(3t)=0$, for $t\ne0$. The additional time-dependent term distinguishes it from the ordinary [KdV equation](#korteweg-de-vries-equation). A scaling-invariant solution has $q=t^{-2/3}F(xt^{-1/3})$. Substitution gives $F^{(3)}+FF'-(\xi F)'/3=0$. [Integration](calculus.md#integral) reduces the similarity problem to $F''+F^2/2-\xi F/3=C$. The [integration](calculus.md#integral) constant depends on supplementary conditions and cannot be set to zero without them. Use real cube roots separately on either sign of $t$.

### Modified Korteweg-De Vries equation

↑ **Parent:** [Korteweg-De Vries equation](#korteweg-de-vries-equation)

This nonlinear dispersive equation replaces the quadratic KdV nonlinearity by a cubic one. In the displayed sign convention, the [Miura transformation](#miura-transformation) maps its solutions to $u_t-6uu_x+u_{xxx}=0$. Its scaling symmetry is $(x,t,v)\mapsto(e^s x,e^{3s}t,e^{-s}v)$.

#### Half-line mKdV spectral global relation

↑ **Parent:** [Modified Korteweg-De Vries equation](#modified-korteweg-de-vries-equation)

For the three corner-normalized [Lax pair](#lax-pair) eigenfunctions, let $s=\mu_3(0,0,k)$ and $S=e^{4ik^3T\widehat\sigma_3}\mu_2(0,T,k)^{-1}$. Their constant connection matrices give the displayed [global relation](differential-equation.md#global-relation-for-a-linear-boundary-value-problem). If their second columns are $(b,a)^T$ and $(B,A)^T$, its upper-right entry is $Ab-Ba=e^{8ik^3T}\mu_{3,12}(0,T,k)$. The right side is analytic in the lower half-plane. In the linear limit this is the [backward-sign Airy half-line global relation](#backward-sign-airy-half-line-global-relation) at Fourier parameter $2k$, coupling all three boundary traces rather than allowing three independent boundary conditions.

#### Miura transformation

↑ **Parent:** [Modified Korteweg-De Vries equation](#modified-korteweg-de-vries-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Miura_transformation)

Direct differentiation gives

$$
u_t-6uu_x+u_{xxx}=(\partial_x+2v)(v_t-6v^2v_x+v_{xxx}).
$$

Consequently this transformation takes solutions of the [modified Korteweg-De Vries equation](#modified-korteweg-de-vries-equation) to solutions of the [Korteweg-De Vries equation](#korteweg-de-vries-equation) in these sign conventions. Both summands in $u$ have the same scaling weight, so the modified-equation scaling induces $(x,t,u)\mapsto(e^sx,e^{3s}t,e^{-2s}u)$.

### KdV Schrodinger spectral problem

↑ **Parent:** [Korteweg-De Vries equation](#korteweg-de-vries-equation)

The inverse-scattering spectral problem associated with this KdV convention is

$$
-\phi_{xx}+u(x,t)\phi=\lambda(t)\phi.
$$

For

$$
Q=\phi_t+u_x\phi-2(u+2\lambda)\phi_x,
$$

differentiation gives the [Wronskian](differential-equation.md#wronskian) identity

$$
\partial_x(\phi_xQ-\phi Q_x)
=\phi^2\bigl[\dot\lambda-(u_t+u_{xxx}-6uu_x)\bigr].
$$

#### Jost solution

↑ **Parent:** [KdV Schrodinger spectral problem](#kdv-schrodinger-spectral-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jost_solution)

A Jost solution of a one-dimensional [Schrödinger equation](physics.md#schrodinger-equation) is specified by plane-wave asymptotics at one spatial infinity. Comparing the left and right Jost solutions defines transmission and reflection coefficients.

#### KdV scattering data

↑ **Parent:** [KdV Schrodinger spectral problem](#kdv-schrodinger-spectral-problem)

For a rapidly decaying KdV potential, the scattering data consist of the continuous [reflection coefficient](partial-differential-equation.md#reflection-coefficient), the negative discrete eigenvalues $-\kappa_n^2$, and a positive norming constant for each bound state.

##### Time evolution of KdV scattering data

↑ **Parent:** [KdV scattering data](#kdv-scattering-data)

For $u_t-6uu_x+u_{xxx}=0$, the discrete eigenvalues are fixed, while

$$
R(k,t)=R(k,0)e^{8ik^3t},
\qquad
c_n(t)=c_n(0)e^{4\kappa_n^3t}
$$

when $c_n$ denotes the bound-state asymptotic amplitude. The squared amplitudes appearing in the Marchenko kernel consequently evolve by $e^{8\kappa_n^3t}$.

##### Born approximation for a one-dimensional reflection coefficient

↑ **Parent:** [KdV scattering data](#kdv-scattering-data)

For a weak potential $u=\epsilon q$, the first [Born approximation](quantum-theory.md#born-approximation) in the KdV Schrödinger convention is

$$
R(k)=\frac{\epsilon}{2ik}\int_{\mathbb R}e^{-2ikx}q(x)\,dx+O(\epsilon^2).
$$

#### Isospectrality of the KdV discrete spectrum

↑ **Parent:** [KdV Schrodinger spectral problem](#kdv-schrodinger-spectral-problem)

For a rapidly decreasing KdV potential and a normalized bound-state eigenfunction, integration of the Wronskian identity over the real line gives $\dot\lambda_n=0$. Thus every discrete eigenvalue $\lambda_n=-\kappa_n^2$ is constant.

##### Evolution of a KdV discrete norming constant

↑ **Parent:** [Isospectrality of the KdV discrete spectrum](#isospectrality-of-the-kdv-discrete-spectrum)

If $\varphi_n(x,t)\sim c_n(t)e^{-\kappa_nx}$ as $x\to+\infty$, the time equation $Q=0$ gives

$$
c_n'(t)=4\kappa_n^3c_n(t),
$$

and hence $c_n(t)=c_n(0)e^{4\kappa_n^3t}$.

### Soliton

↑ **Parent:** [Korteweg-De Vries equation](#korteweg-de-vries-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Soliton)

A soliton is a localized travelling wave whose shape is preserved by the evolution and whose interactions with other solitons are elastic up to phase shifts.

#### Multisoliton solution

↑ **Parent:** [Soliton](#soliton)

An exact nonlinear-wave solution containing several localized [solitons](#soliton). In an integrable scattering solution, these objects approach separated incoming and outgoing profiles, with collision effects encoded by position shifts and internal phases. [Bäcklund transformations](#backlund-transformation) and [Hirota's bilinear method](#hirota-s-bilinear-method) construct examples such as the [Sine-Gordon multisoliton tau representation](scalar-field-theory.md#sine-gordon-multisoliton-tau-representation).

## Inverse scattering transform

↑ **Parent:** [Integrable systems](integrable-systems.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_scattering_transform)

The inverse scattering transform evolves the scattering data of an auxiliary linear operator and reconstructs the potential from the evolved data.

### Scattering data

↑ **Parent:** [Inverse scattering transform](#inverse-scattering-transform)

[Scattering data](#scattering-data) describe connections between normalized solutions of an auxiliary spectral equation, together with any discrete spectral points and their norming data. In an [inverse scattering transform](#inverse-scattering-transform), the nonlinear potential is reconstructed from these data; boundary spectral connection matrices must additionally obey a [global relation](differential-equation.md#global-relation-for-a-linear-boundary-value-problem).

### Cauchy-kernel dressing for the KdV equation

↑ **Parent:** [Inverse scattering transform](#inverse-scattering-transform)

Put $E_k=e^{i(kx+k^3t)}$, $I=\int_L\varphi(l)d\lambda(l)$ and $q=-I_x$. For the dressing operator $\mathcal Fh=h+iE_k\int_Lh(l)/(k+l)d\lambda(l)$, differentiating gives $\mathcal F(M\varphi)=0$ and $\mathcal F(N\varphi)=3ikM\varphi$, where $M=\partial_x^2-ik\partial_x+q$ and $N=\partial_t+\partial_x^3+3q\partial_x$. Uniqueness of the [linear integral equation](analysis.md#linear-integral-equation) therefore supplies a [Lax pair](#lax-pair). Its [commutator](lie-algebra.md#commutator) identity is $[N,M]=-3q_xM+(q_t+q_{xxx}+6qq_x)$, which gives the [KdV equation](#korteweg-de-vries-equation) when the eigenfunction is not identically zero. Differentiation under the integral and the uniqueness assumption are essential hypotheses.

#### Finite-rank KdV dressing determinant

↑ **Parent:** [Cauchy-kernel dressing for the KdV equation](#cauchy-kernel-dressing-for-the-kdv-equation)

Choose distinct $\kappa_j>0$ and weights $c_j>0$ at spectral points $i\kappa_j$. With $E_j=e^{-\kappa_jx+\kappa_j^3t}$ and $A_{ij}=c_jE_i/(\kappa_i+\kappa_j)$, solve $(I+A)\Phi=E$. The reconstructed [multisoliton solution](#multisoliton-solution) is $q=-\partial_x(c^T\Phi)$. Since $\Lambda A+A\Lambda=Ec^T$, cyclicity of the [trace](linear-algebra.md#matrix-trace) gives $c^T\Phi=-2\partial_x\log\det(I+A)$. The [Cauchy matrix](vector-space.md#cauchy-matrix) $1/(\kappa_i+\kappa_j)$ is positive definite, because it is the Gram matrix of $e^{-\kappa_i s}$ on $s>0$; diagonal similarity then proves $\det(I+A)>0$. For one spectral point this yields $q=(\kappa^2/2)\operatorname{sech}^2[\kappa(x-\kappa^2t-x_0)/2]$.

### Discrete scattering data

↑ **Parent:** [Inverse scattering transform](#inverse-scattering-transform)

Discrete scattering data consist of the discrete eigenvalues and norming constants associated with bound states of the auxiliary spectral problem. Their simple time evolution reconstructs solitons and breathers through the inverse problem.

### Marchenko equation

↑ **Parent:** [Inverse scattering transform](#inverse-scattering-transform)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Marchenko_equation)

For one-dimensional inverse scattering, the Gelfand-Levitan-Marchenko equation

$$
K(x,y)+F(x+y)+\int_x^\infty K(x,z)F(z+y)\,dz=0
$$

recovers the transformation kernel $K$ from scattering data encoded by $F$. In the convention used for the Korteweg-De Vries equation above, the potential is

$$
u(x,t)=-2\frac{\partial}{\partial x}K(x,x;t).
$$

#### Rank-one Gelfand-Levitan-Marchenko kernel

↑ **Parent:** [Marchenko equation](#marchenko-equation)

If $F(s)=c e^{-\chi s}$ with $\chi>0$, the Gelfand-Levitan-Marchenko equation has a separable kernel. Writing $K(x,y)=-B(x)e^{-\chi y}$ reduces the integral equation to one algebraic equation for $B(x)$ and reconstructs a single soliton.

## Poisson-commuting separated energies

↑ **Parent:** [Integrable systems](integrable-systems.md)

Hamiltonians that split into terms $F_i(p_i,q_i)$ have $\{F_i,F_j\}=0$ for $i\ne j$, and their differentials are generically independent because they use disjoint coordinate pairs.

## Separable forced harmonic oscillators

↑ **Parent:** [Integrable systems](integrable-systems.md)

A Hamiltonian that is a sum of one-coordinate quadratic potentials plus linear terms becomes a collection of independent harmonic oscillators after translating each equilibrium position.

## Action variable of a shifted harmonic oscillator

↑ **Parent:** [Integrable systems](integrable-systems.md)

For $F=(p^2+W^2q^2+aq)/2$, shifting $Q=q+a/(2W^2)$ gives oscillator energy $E=F+a^2/(8W^2)$ and action $I=E/|W|$.

### Phase-plane area formula for an action variable

↑ **Parent:** [Action variable of a shifted harmonic oscillator](#action-variable-of-a-shifted-harmonic-oscillator)

The action $(2\pi)^{-1}\oint p\,dq$ is the area enclosed by a periodic phase-plane orbit divided by $2\pi$.

## Compatibility condition for an overdetermined linear system

↑ **Parent:** [Integrable systems](integrable-systems.md)

Commuting mixed derivatives impose an equation on the coefficient matrices of an overdetermined auxiliary system.

## Integrable partial differential equation

↑ **Parent:** [Integrable systems](integrable-systems.md)

An integrable partial differential equation has enough exact structure, such as a [Lax pair](#lax-pair), infinitely many [conserved quantities](classical-mechanics.md#conserved-quantity), or an [inverse scattering transform](#inverse-scattering-transform), to reduce its evolution to auxiliary linear or finite-dimensional data.

### Harry Dym equation

↑ **Parent:** [Integrable partial differential equation](#integrable-partial-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Harry_Dym_equation)

The Harry Dym equation is the [integrable partial differential equation](#integrable-partial-differential-equation) $p_t=p^3p_{xxx}$. It admits a [Lax pair](#lax-pair) based on the second-order operator $L=-\partial_xp^2\partial_x$.

### Boussinesq equation

↑ **Parent:** [Integrable partial differential equation](#integrable-partial-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boussinesq_equation)

The Boussinesq equation is a nonlinear dispersive wave equation. One integrable normalization is

$$
q_{tt}=3q_{xxxx}-12(q^2)_{xx}.
$$

## Lax pair

↑ **Parent:** [Integrable systems](integrable-systems.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lax_pair)

A Lax pair encodes a nonlinear equation as compatibility of two linear equations depending on an auxiliary spectral parameter.

### Volterra analyticity sectors for reverse-dispersion mKdV

↑ **Parent:** [Lax pair](#lax-pair)

For the [modified Korteweg-De Vries equation](#modified-korteweg-de-vries-equation) with linear part $q_t-q_{xxx}$, the [Volterra integral equation](analysis.md#volterra-integral-equation) kernel is $e^{i[k(x-x')-4k^3(t-t')]\widehat\sigma_3}$. In column one its off-diagonal modulus is $e^{2\operatorname{Im}k(x-x')-8\operatorname{Im}k^3(t-t')}$; column two has the reciprocal modulus. Define $D_1$ by signs $(+,+)$, $D_2$ by $(+,-)$, $D_3$ by $(-,+)$ and $D_4$ by $(-,-)$. The normalization points $(0,T)$, $(0,0)$ and $(\infty,t)$ give column domains $(D_4,D_1)$, $(D_3,D_2)$ and $(\mathbb C_+,\mathbb C_-)$, respectively. Finite-path eigenfunctions can be entire at fixed coordinates while failing to be bounded outside these spectral sectors.

<h3 id="quadratic-spectral-lax-pair-for-zero-parameter-painleve-ii">Quadratic spectral Lax pair for zero-parameter Painlevé II</h3>

↑ **Parent:** [Lax pair](#lax-pair)

Let $A$ have diagonal entries $\pm(\lambda^2+w+z/2)$ and off-diagonal entries $u\lambda+u'$ and $-2w\lambda/u+2u'w/u^2$. Let $B$ have diagonal entries $\pm\lambda/2$ and off-diagonal entries $u/2,-w/u$. Substitution into the [isomonodromic deformation](complex-analysis.md#isomonodromic-deformation) compatibility identity gives the displayed equations on domains with $u\ne0$. Thus $(w/u^2)'=0$, so $w=Cu^2$ and $u''+Cu^3+zu/2=0$, a rescaled zero-parameter [Painlevé II equation](differential-equation.md#painleve-ii-equation) when $C\ne0$. The leading coefficient $-2w/u$ is required by cancellation of the quadratic spectral terms.

### Volterra analyticity sectors for a half-line NLS Lax pair

↑ **Parent:** [Lax pair](#lax-pair)

For the normalization points $(0,T)$, $(0,0)$ and spatial infinity, the [Volterra integral equation](analysis.md#volterra-integral-equation) kernel is $e^{-i[k(x-x')+2k^2(t-t')]\widehat\sigma_3}$. Its lower entry in column one has factor $e^{2i[k(x-x')+2k^2(t-t')]}$; column two has the opposite factor. With quadrants numbered counterclockwise, the column domains are $(D_2,D_3)$, $(D_1,D_4)$ and $(\mathbb C_-,\mathbb C_+)$, respectively.

### Lax pair for the Bogomolny equations

↑ **Parent:** [Lax pair](#lax-pair)

For $D_i=\partial_i+A_i$ and Higgs multiplication $\Phi$, set

$$
L_0=D_1+iD_2-\lambda(D_3+i\Phi),\qquad L_1=D_3-i\Phi+\lambda(D_1-iD_2).
$$

Write $a=F_{12}-D_3\Phi$, $b=F_{31}-D_2\Phi$, $c=F_{23}-D_1\Phi$, where $D_i\Phi=\partial_i\Phi+[A_i,\Phi]$. Direct expansion gives $[L_0,L_1]=-b+ic-2i\lambda a-\lambda^2(b+ic)$. Its vanishing for every complex $\lambda$ is therefore equivalent to $a=b=c=0$, the [Bogomolny equations](quantum-field-theory.md#bogomolny-equations). It is a parameter-dependent [zero-curvature representation](#zero-curvature-condition).

### Lax equation preserves the spectrum

↑ **Parent:** [Lax pair](#lax-pair)

For symmetric $L$ and antisymmetric $A$ satisfying $\dot L=LA-AL$, solve $\dot Q=-AQ$, $Q(0)=I$. Then $Q$ is orthogonal and $Q^TLQ$ is constant. Hence every eigenvalue and every coefficient of the characteristic polynomial of $L$ is conserved.

### Monodromy matrix

↑ **Parent:** [Lax pair](#lax-pair)

For periodic $U(x,t,\lambda)$ with period $L$, solve $W_x=UW$, $W(0)=I$. The monodromy matrix is $w=W(L)$. If $U,V$ satisfy the [zero-curvature condition](#zero-curvature-condition) and are periodic, then $W_t=VW-WV(0)$, hence $w_t=[V(0),w]$. The [matrix trace](linear-algebra.md#matrix-trace) of each power of $w$ is a [first integral](differential-equation.md#first-integral).

### Spectral parameter

↑ **Parent:** [Lax pair](#lax-pair)

A spectral parameter is an auxiliary complex parameter in a linear system whose compatibility encodes a nonlinear integrable equation. Its analytic dependence organizes conserved quantities and scattering data.

### Lax pair for the anti-self-dual Yang-Mills equations

↑ **Parent:** [Lax pair](#lax-pair)

For covariant derivatives on Euclidean four-space, one anti-self-dual Yang-Mills Lax pair is

$$
L=D_1+iD_2-\zeta(D_3-iD_4),
\qquad
M=D_3+iD_4+\zeta(D_1-iD_2).
$$

The condition $[L,M]=0$ for every $\zeta\in\mathbb{CP}^1$ is equivalent to anti-self-duality of the curvature.

#### Euclidean complex-coordinate anti-self-dual Lax pair

↑ **Parent:** [Lax pair for the anti-self-dual Yang-Mills equations](#lax-pair-for-the-anti-self-dual-yang-mills-equations)

For metric $2(dw\,d\bar w+dz\,d\bar z)$, the [commutator](lie-algebra.md#commutator) is $[L,M]=F_{wz}+\lambda(F_{w\bar w}+F_{z\bar z})+\lambda^2F_{\bar w\bar z}$. Vanishing for every [spectral parameter](#spectral-parameter) $\lambda$ is exactly the [Anti-self-dual Yang-Mills equations](classical-field-theory-soliton.md#anti-self-dual-yang-mills-equations). The derivative parts span a totally null two-plane in the complexified tangent space. Thus an invertible fundamental solution of $L\Psi=M\Psi=0$ exists locally exactly when the three [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) coefficients vanish; compatibility of one possibly zero vector alone is not enough.

// Destination: fiber-bundle.bigb

### Airy equation

↑ **Parent:** [Lax pair](#lax-pair)

The Airy equation is the linear dispersive partial differential equation $q_t+q_{xxx}=0$. Under the spatial [Fourier transform](analysis.md#fourier-transform), each mode evolves by multiplication by $e^{ik^3t}$.

For positive time its fundamental solution is $(3t)^{-1/3}\operatorname{Ai}(x/(3t)^{1/3})$, connecting this evolution equation to the [Airy function](differential-equation.md#airy-function) without identifying the two concepts.

#### Cubic dispersion symmetry with negative transport

↑ **Parent:** [Airy equation](#airy-equation)

For dispersion $w(k)=-i(k^3+k)$, the other roots of $w(\nu)=w(k)$ satisfy $\nu^2+k\nu+k^2+1=0$. In $D_+=\{\operatorname{Im}k>0,\operatorname{Re}w(k)<0\}$ both roots lie in the lower half-plane. Interpolating the unknown linear polynomial $G_2+i\nu G_1$ at them eliminates two boundary traces. The resulting symmetric expression has removable singularities where the roots coalesce.

#### Gauge reduction of a third-order half-line equation

↑ **Parent:** [Airy equation](#airy-equation)

For $Q_T+Q_{XXX}+aQ_{XX}+bQ_X+cQ=0$, an exponential gauge removes the second derivative. With $\kappa^2=a^2/3-b>0$ and $\sigma=-c+ab/3-2a^3/27$, the remaining equation is $q_t+q_{xxx}-q_x=0$. Negative $a$ improves spatial decay of the transformed initial data; positive $a$ can destroy the convergence of its [Half-range Fourier transform](analysis.md#half-range-fourier-transform).

#### Backward-sign Airy half-line global relation

↑ **Parent:** [Airy equation](#airy-equation)

For the [Airy equation](#airy-equation) with opposite dispersive sign, $q_t-q_{xxx}=0$ on $x>0$, let $Q$ be the initial [Half-range Fourier transform](analysis.md#half-range-fourier-transform) and $F_j(k,t)=\int_0^t e^{ik^3s}\partial_x^jq(0,s)\,ds$. Three [integrations by parts](calculus.md#integration-by-parts) give the displayed [global relation](differential-equation.md#global-relation-for-a-linear-boundary-value-problem). The spatial transform is [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) for $\operatorname{Im}k<0$, whereas the [finite-time spectral boundary transforms](differential-equation.md#finite-time-spectral-boundary-transform) are [entire functions](complex-analysis.md#entire-function). The symmetry $k\mapsto\alpha k$, $\alpha^3=1$, preserves their time exponent.

// Target: analysis.bigb

##### Two boundary traces for reverse-dispersion Airy flow

↑ **Parent:** [Backward-sign Airy half-line global relation](#backward-sign-airy-half-line-global-relation)

For $q_t-q_{xxx}=0$ on $x>0$, evaluate the [global relation](differential-equation.md#global-relation-for-a-linear-boundary-value-problem) at $k=-ir/2$, where $\operatorname{Re}p>0$ and the principal cube root $r=p^{1/3}$ has positive real part. The time exponent becomes $-p$, giving the displayed [Laplace transform](analysis.md#laplace-transform) identity. Thus the second-derivative trace is determined once the value and first-derivative traces are prescribed. The homogeneous transformed equation $u'''-pu=0$ has exactly two spatially decaying roots, so two independent admissible conditions are required. One condition leaves a free decaying mode; three independent conditions generally violate the global constraint.

#### Mixed-boundary Airy energy principle

↑ **Parent:** [Airy equation](#airy-equation)

For $L=-d^2/dx^2+x$ on $(0,1)$, with homogeneous conditions $v(0)=0$, $v'(1)=0$, [integration by parts](calculus.md#integration-by-parts) gives $\langle v,Lv\rangle=\int_0^1(v'^2+xv^2)dx>0$ for nonzero $v$. The affine energy $J[u]=\tfrac12\int_0^1(u'^2+xu^2)dx$, minimized over $H^1$ functions with $u(0)=a$, yields $Lu=0$ and the natural [boundary condition](differential-equation.md#boundary-condition) $u'(1)=0$. The inequality $\|v\|_2^2\le\tfrac12\|v'\|_2^2$ on $v(0)=0$ proves that the form is a [coercive bilinear form](linear-algebra.md#coercive-bilinear-form); [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) supplies a unique critical point, and $J[u+v]-J[u]=\tfrac12\int(v'^2+xv^2)$ proves that it is the unique minimum.

#### Linear dispersive Stokes equation

↑ **Parent:** [Airy equation](#airy-equation)

The scalar [linear partial differential equation](partial-differential-equation.md#linear-partial-differential-equation) $u_t+u_x+u_{xxx}=0$ is an [Airy equation](#airy-equation) with a first-order transport term. It is a linearization of the [Korteweg-De Vries equation](#korteweg-de-vries-equation) with an advective term retained. It is distinct from the viscous incompressible-flow [Stokes equation](stokes-flow.md#stokes-equation). On the whole line its spatial [Fourier transform](analysis.md#fourier-transform) evolves by $e^{i(k^3-k)t}$.

##### Spatial root splitting for the dispersive Stokes resolvent

↑ **Parent:** [Linear dispersive Stokes equation](#linear-dispersive-stokes-equation)

For a time [Laplace transform](analysis.md#laplace-transform) parameter with $\operatorname{Re}p>0$, the spatial [characteristic roots](differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation) satisfy $r^3+r+p=0$. Exactly one root $r_-$ has negative [real part](complex-analysis.md#real-part) and two have positive [real part](complex-analysis.md#real-part). Indeed an imaginary root would force $p=-i(k-k^3)$ to be imaginary. The count is therefore constant on the connected right half-plane; for real $p>0$, the cubic has one negative real root and a conjugate pair with positive real parts. Repeated roots would satisfy $3r^2+1=0$, which again puts $p$ on the imaginary axis. Thus $r_-(p)$ is a nonzero [holomorphic function](complex-analysis.md#holomorphic-function) in the right half-plane. Only $e^{r_-x}$ decays at positive spatial infinity.

###### Stokes resolvent kernel with advection

↑ **Parent:** [Spatial root splitting for the dispersive Stokes resolvent](#spatial-root-splitting-for-the-dispersive-stokes-resolvent)

For $\operatorname{Re}p>0$, let $r_-$ and $r_1,r_2$ be the [characteristic roots](differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation) of $r^3+r+p=0$, split by the signs of their [real parts](complex-analysis.md#real-part). Put $d_j=3r_j^2+1$. The real-line [Green function](analysis.md#green-s-function) of $p+\partial_x+\partial_x^3$ is

$$
R_p(s)=\begin{cases}e^{r_-s}/d_-,&s\ge0,\\-\sum_{j=1}^2e^{r_js}/d_j,&s<0.\end{cases}
$$

The [reciprocal-polynomial root identities](isolated-singularity.md#reciprocal-polynomial-root-identities) imply continuity of $R_p,R_p'$ and jump $R_p''(0+)-R_p''(0-)=1$. The [distributional derivative](distribution-theory.md#distributional-derivative) therefore gives $(p+\partial_s+\partial_s^3)R_p=\delta_0$. The transport term changes the roots: the pure [Airy resolvent kernel](#airy-resolvent-kernel) with $r^3+p=0$ cannot be substituted unchanged.

###### Half-line Stokes solution with a boundary derivative

↑ **Parent:** [Stokes resolvent kernel with advection](#stokes-resolvent-kernel-with-advection)

For the [linear dispersive Stokes equation](#linear-dispersive-stokes-equation) on $x>0$, with sufficiently smooth decaying initial data and $\operatorname{Re}p>0$, define $V(x,p)=\int_0^\infty R_p(x-y)u_0(y)\,dy$ and let $G(p)$ be the time [Laplace transform](analysis.md#laplace-transform) of the prescribed derivative $u_x(0,t)$. Spatial decay and the one-dimensional decaying homogeneous space give

$$
U(x,p)=V(x,p)+\frac{e^{r_-x}}{r_-}\bigl[G(p)-V_x(0,p)\bigr].
$$

The [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) follows by differentiating at zero. The initial forcing follows from the [Stokes resolvent kernel with advection](#stokes-resolvent-kernel-with-advection). The [Bromwich inversion formula](analysis.md#bromwich-inversion-formula) gives an [integral representation](calculus.md#integral-representation) with no unknown boundary traces. Truncating or extending the prescribed boundary signal beyond a target time does not affect earlier values, by the [Laplace transform time-shift rule](analysis.md#laplace-transform-time-shift-rule) and causality of this [Green function](analysis.md#green-s-function).

#### Airy resolvent kernel

↑ **Parent:** [Airy equation](#airy-equation)

For $\operatorname{Re}p>0$, put $\lambda=p^{1/3}$ using the [principal cube root](analysis.md#principal-cube-root) and $r_{1,2}=\lambda e^{\pm i\pi/3}$. The decaying [Green function](analysis.md#green-s-function) for $\partial_s^3+p$ on the real line is

$$
R_p(s)=\begin{cases}e^{-\lambda s}/(3\lambda^2),&s\geq0,\\-\sum_{j=1}^2e^{r_js}/(3r_j^2),&s<0.\end{cases}
$$

The identities among the three [characteristic roots](differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation) show that $R_p$ and $R_p'$ are continuous, while $R_p''$ has jump one. Its [distributional derivative](distribution-theory.md#distributional-derivative) therefore satisfies $(\partial_s^3+p)R_p=\delta_0$. This is the kernel of the [resolvent operator](functional-analysis.md#resolvent-of-an-operator) $(p+\partial_s^3)^{-1}$, obtained by the time [Laplace transform](analysis.md#laplace-transform) of the [Airy equation](#airy-equation).

##### Airy half-line solution with prescribed boundary derivative

↑ **Parent:** [Airy resolvent kernel](#airy-resolvent-kernel)

For $u_t+u_{xxx}=0$ on $x>0$, define $V(x,p)=\int_0^\infty R_p(x-y)u_0(y)dy$ and let $G$ be the time [Laplace transform](analysis.md#laplace-transform) of $u_x(0,t)$. The transformed solution with spatial decay is

$$
U(x,p)=V(x,p)+\frac{e^{-p^{1/3}x}}{p^{1/3}}\left[V_x(0,p)-G(p)\right].
$$

Only one [characteristic root](differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation) has negative [real part](complex-analysis.md#real-part), so one scalar boundary derivative fixes the remaining homogeneous mode. The [Bromwich inversion formula](analysis.md#bromwich-inversion-formula) supplies an [integral representation](calculus.md#integral-representation) involving only the initial and boundary data. For general [linear differential equations](differential-equation.md#linear-differential-equation) on a half-line, the number and form of the necessary boundary data depend on the decaying spatial roots; [Fokas and Wang](https://arxiv.org/abs/1409.2083) study the corresponding boundary maps for linear dispersive equations.

### AKNS Lax pair for the nonlinear Schrodinger equation

↑ **Parent:** [Lax pair](#lax-pair)

For complex fields $q,r$, the standard two-by-two AKNS pair has zero-curvature equations

$$
ir_t+r_{xx}+2qr^2=0,
\qquad
iq_t-q_{xx}-2rq^2=0.
$$

The reductions $q=\overline r$ and $q=-\overline r$ give the focusing and defocusing cubic nonlinear Schrödinger equations, respectively.

### Isospectral Lax equation

↑ **Parent:** [Lax pair](#lax-pair)

For $\dot L=[L,A]$, the operator $\partial_t+A$ maps each eigenspace of $L$ into itself, so the spectrum is time-independent.

#### Third-order Boussinesq Lax pair

↑ **Parent:** [Isospectral Lax equation](#isospectral-lax-equation)

The Lax equation $L_t=[L,A]$ for these operators is equivalent to

$$
q_t=3p_x,
\qquad
p_t=q_{xxx}-4(q^2)_x.
$$

Eliminating $p$ gives the [Boussinesq equation](#boussinesq-equation)

$$
q_{tt}=3q_{xxxx}-12(q^2)_{xx}.
$$

#### Trace invariants of a Lax equation

↑ **Parent:** [Isospectral Lax equation](#isospectral-lax-equation)

If

$$
\dot L=[L,A],
$$

then every positive power has constant trace:

$$
\frac d{dt}\operatorname{tr}(L^n)
=n\operatorname{tr}(L^{n-1}[A,L])=0.
$$

The final equality is the cyclic property of the [matrix trace](linear-algebra.md#matrix-trace).

#### Finite Volterra lattice

↑ **Parent:** [Isospectral Lax equation](#isospectral-lax-equation)

With boundary values $q_0=q_n=0$, the finite Volterra lattice is

$$
\dot q_j=2q_j(q_{j+1}-q_{j-1}),
\qquad 1\leq j\leq n-1,
$$

up to rescaling or reversal of time. Writing $q_j=a_j^2$ gives $\dot a_j=a_j(a_{j+1}^2-a_{j-1}^2)$.

##### Zero-diagonal Jacobi Lax pair for the finite Volterra lattice

↑ **Parent:** [Finite Volterra lattice](#finite-volterra-lattice)

Let $L$ be the symmetric zero-diagonal [Jacobi matrix](numerical-analysis.md#jacobi-matrix) with $L_{j,j+1}=L_{j+1,j}=a_j$, and let the [skew-symmetric matrix](linear-algebra.md#skew-symmetric-matrix) $B$ have

$$
B_{j,j+2}=-B_{j+2,j}=a_ja_{j+1}.
$$

Then $\dot L=[B,L]$ is equivalent to the [Finite Volterra lattice](#finite-volterra-lattice). The corresponding similarity flow makes the eigenvalues of $L$, the coefficients of its [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial), and its [trace invariants](#trace-invariants-of-a-lax-equation) first integrals.

#### Periodic KdV transfer matrix

↑ **Parent:** [Isospectral Lax equation](#isospectral-lax-equation)

For real periodic KdV data, translation by one period acts on a conjugate basis of scattering solutions by

$$
T=\begin{pmatrix}a&b\\\bar b&\bar a\end{pmatrix},
\qquad |a|^2-|b|^2=1.
$$

Lax compatibility gives $\dot T=[\Lambda,T]$ for the matrix of $\partial_t+A$ on the eigenspace. Hence $\operatorname{tr}T=2\operatorname{Re}a$ is conserved.

### Zero-curvature condition

↑ **Parent:** [Lax pair](#lax-pair)

For $\Phi_x+U\Phi=0$ and $\Phi_y+V\Phi=0$, compatibility is $V_x-U_y+[U,V]=0$.

For the auxiliary equations $\psi_x=U\psi$ and $\psi_t=V\psi$, equality of mixed derivatives gives $U_t-V_x+[U,V]=0$. This is the compatibility condition for a [Lax pair](#lax-pair).

### Global relation for the half-line free Schrodinger equation

↑ **Parent:** [Lax pair](#lax-pair)

For $u_t=iu_{xx}$ on $x>0$, the half-line Fourier transform satisfies

$$
\widehat u_t+ik^2\widehat u=kh(t)-iu_x(0,t).
$$

Subtracting the relation at $-k$ cancels the unknown Neumann datum. Fourier inversion of the resulting odd combination gives the solution in terms of the initial transform and the prescribed Dirichlet datum, with boundary kernel $G(k,t)=kh(t)$.

## Tzitzeica equation

↑ **Parent:** [Integrable systems](integrable-systems.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tzitzeica_equation)

The Tzitzeica equation in light-cone coordinates is $u_{xy}=e^u-e^{-2u}$ and admits a matrix Lax pair.

### Scaling-invariant reduction of the Tzitzeica equation

↑ **Parent:** [Tzitzeica equation](#tzitzeica-equation)

The [Tzitzeica equation](#tzitzeica-equation) $u_{xy}=e^u-e^{-2u}$ is unchanged by $(x,y)\mapsto(cx,c^{-1}y)$. The identity component has generator $x\partial_x-y\partial_y$. Locally its invariant solutions are $u=w(xy)$, reducing the equation to $zw''+w'=e^w-e^{-2w}$.

## ↑ Ancestors (3)

1. [Branches of physics](physics.md#branches-of-physics)
2. [Physics](physics.md)
3. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Integrable Hamiltonian system](classical-mechanics.md#integrable-hamiltonian-system)
- [Nonlinear Schrödinger equation](partial-differential-equation.md#nonlinear-schrodinger-equation)
- [Painlevé II equation](differential-equation.md#painleve-ii-equation)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1.md#8b/b/solution)
- [Sine-Gordon equation](#sine-gordon-equation)
