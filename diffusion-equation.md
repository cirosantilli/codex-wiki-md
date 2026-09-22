# Diffusion equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diffusion_equation)

A diffusion equation describes smoothing caused by a flux down spatial gradients.

**Table of contents**

- [Scalar integrating factor for a reaction-diffusion equation](#scalar-integrating-factor-for-a-reaction-diffusion-equation)
- [Squared diffusion-residual action](#squared-diffusion-residual-action)
  - [Time reversal of the squared diffusion-residual action](#time-reversal-of-the-squared-diffusion-residual-action)
- [Robin diffusion with a growing mode](#robin-diffusion-with-a-growing-mode)
- [Drift-diffusion equation with a potential](#drift-diffusion-equation-with-a-potential)
- [Diffusive time scale](#diffusive-time-scale)
- [Variable-coefficient conservative diffusion equation](#variable-coefficient-conservative-diffusion-equation)
- [Infinite propagation speed](#infinite-propagation-speed)
- [Periodic homogenization of a diffusion equation](#periodic-homogenization-of-a-diffusion-equation)
- [Porous medium equation](#porous-medium-equation)
  - [Spherical nonlinear-diffusion source profile](#spherical-nonlinear-diffusion-source-profile)
  - [Compact radial cubic-diffusion profile](#compact-radial-cubic-diffusion-profile)
  - [Finite propagation in porous-medium diffusion](#finite-propagation-in-porous-medium-diffusion)
  - [Forced filling similarity for power-law diffusion](#forced-filling-similarity-for-power-law-diffusion)
  - [Separable draining profile for power-law diffusion](#separable-draining-profile-for-power-law-diffusion)
  - [Barenblatt solution](#barenblatt-solution)
    - [Radial cubic-diffusion source profile](#radial-cubic-diffusion-source-profile)
    - [Planar volume-conserving nonlinear-diffusion similarity](#planar-volume-conserving-nonlinear-diffusion-similarity)
      - [Semicircular pulse under cubic diffusion](#semicircular-pulse-under-cubic-diffusion)
    - [Two-dimensional Barenblatt profile for quadratic porous-medium diffusion](#two-dimensional-barenblatt-profile-for-quadratic-porous-medium-diffusion)
- [Fick's first law](#fick-s-first-law)
- [Heat equation](#heat-equation)
  - [Heat balance with volumetric heat generation](#heat-balance-with-volumetric-heat-generation)
  - [Annual ground-temperature wave](#annual-ground-temperature-wave)
  - [Fixed-temperature and fixed-flux heat equation on an interval](#fixed-temperature-and-fixed-flux-heat-equation-on-an-interval)
  - [Heat flow from a triangular initial temperature](#heat-flow-from-a-triangular-initial-temperature)
    - [Heat flow from a triangular initial temperature with insulated endpoints](#heat-flow-from-a-triangular-initial-temperature-with-insulated-endpoints)
  - [Cooling of an initially uniform square](#cooling-of-an-initially-uniform-square)
  - [Periodic diffusion on a circle](#periodic-diffusion-on-a-circle)
    - [Periodic sine with an endpoint-correcting linear term](#periodic-sine-with-an-endpoint-correcting-linear-term)
  - [Heat equation with a single stationary sine forcing](#heat-equation-with-a-single-stationary-sine-forcing)
  - [Steady temperature of a uniformly heated cylindrical wire](#steady-temperature-of-a-uniformly-heated-cylindrical-wire)
  - [Fundamental diffusion mode](#fundamental-diffusion-mode)
  - [Heat equation on a rectangle with two insulated sides](#heat-equation-on-a-rectangle-with-two-insulated-sides)
  - [Reaction-diffusion spectral decay threshold](#reaction-diffusion-spectral-decay-threshold)
    - [Spherical reaction-diffusion growth threshold](#spherical-reaction-diffusion-growth-threshold)
  - [Heat evolution of bounded data need not converge at large times](#heat-evolution-of-bounded-data-need-not-converge-at-large-times)
  - [Dirichlet heat-reaction threshold on the unit square](#dirichlet-heat-reaction-threshold-on-the-unit-square)
  - [Heat operator](#heat-operator)
  - [Heat-equation uniqueness under Gaussian growth](#heat-equation-uniqueness-under-gaussian-growth)
  - [Backward heat equation](#backward-heat-equation)
    - [Space-time harmonic functions along Brownian motion](#space-time-harmonic-functions-along-brownian-motion)
  - [Heat equation maximum principle](#heat-equation-maximum-principle)
  - [Heat equation energy identity](#heat-equation-energy-identity)
  - [Dirichlet boundary-forcing heat-kernel formula](#dirichlet-boundary-forcing-heat-kernel-formula)
    - [Half-line drift boundary kernel](#half-line-drift-boundary-kernel)
  - [Dirichlet energy dissipation for the heat equation](#dirichlet-energy-dissipation-for-the-heat-equation)
  - [Radial heat equation in three dimensions](#radial-heat-equation-in-three-dimensions)
    - [Spherical-shell heat equation via radial rescaling](#spherical-shell-heat-equation-via-radial-rescaling)
  - [Sinusoidally forced heat equation on a half-line](#sinusoidally-forced-heat-equation-on-a-half-line)
  - [Potential Burgers equation](#potential-burgers-equation)
  - [Heat kernel](#heat-kernel)
    - [Heat kernel trace formula](#heat-kernel-trace-formula)
    - [Positive diffusivity requirement for the forward heat kernel](#positive-diffusivity-requirement-for-the-forward-heat-kernel)
    - [Heat-kernel convolution](#heat-kernel-convolution)
    - [Riemannian heat kernel](#riemannian-heat-kernel)
      - [Heat kernel on a finite isometric quotient](#heat-kernel-on-a-finite-isometric-quotient)
        - [Heat semigroup descent through a finite normal covering](#heat-semigroup-descent-through-a-finite-normal-covering)
      - [Spectral expansion of the Riemannian heat kernel](#spectral-expansion-of-the-riemannian-heat-kernel)
      - [Heat parametrix](#heat-parametrix)
        - [Heat-kernel transport equations](#heat-kernel-transport-equations)
        - [Volterra parametrix correction](#volterra-parametrix-correction)
    - [Gaussian interval mass](#gaussian-interval-mass)
    - [Heat Poisson kernel](#heat-poisson-kernel)
    - [Dirichlet heat kernel on an interval](#dirichlet-heat-kernel-on-an-interval)
      - [Survival probability from an absorbing transition density](#survival-probability-from-an-absorbing-transition-density)
        - [Symmetric absorbing-interval survival probability](#symmetric-absorbing-interval-survival-probability)
      - [Thermal trace of an interval image kernel](#thermal-trace-of-an-interval-image-kernel)
    - [Gaussian heat kernel](#gaussian-heat-kernel)
      - [Gaussian initial data for the heat equation](#gaussian-initial-data-for-the-heat-equation)
        - [Odd pair of Gaussian profiles under diffusion](#odd-pair-of-gaussian-profiles-under-diffusion)
      - [Newtonian potential of the Brownian heat kernel](#newtonian-potential-of-the-brownian-heat-kernel)
    - [Neumann heat kernel on an interval](#neumann-heat-kernel-on-an-interval)
    - [Heat semigroup](#heat-semigroup)
      - [Spectral construction of a parabolic solution](#spectral-construction-of-a-parabolic-solution)
    - [Heat kernel expansion](#heat-kernel-expansion)
      - [Heat invariants](#heat-invariants)
        - [Integrated second scalar heat coefficient](#integrated-second-scalar-heat-coefficient)
        - [Spectral determination of hyperbolic curvature on a surface](#spectral-determination-of-hyperbolic-curvature-on-a-surface)
      - [Curvature coefficient of the scalar heat kernel](#curvature-coefficient-of-the-scalar-heat-kernel)
      - [Normal-coordinate divergence-form heat parametrix](#normal-coordinate-divergence-form-heat-parametrix)
    - [Gaussian approximate identity](#gaussian-approximate-identity)
    - [Heat-kernel solution](#heat-kernel-solution)
      - [Heat-kernel convergence from a conditionally convergent Gaussian integral](#heat-kernel-convergence-from-a-conditionally-convergent-gaussian-integral)
      - [Heat-kernel convergence for Gaussian-integrable initial data](#heat-kernel-convergence-for-gaussian-integrable-initial-data)
      - [Heat equation with interval-indicator initial data](#heat-equation-with-interval-indicator-initial-data)
    - [Neumann heat kernel on a half-line](#neumann-heat-kernel-on-a-half-line)
  - [Probabilistic representation of the heat equation with time-dependent Dirichlet data](#probabilistic-representation-of-the-heat-equation-with-time-dependent-dirichlet-data)
  - [Duhamel's principle](#duhamel-s-principle)
    - [Causal diffusion from a finite-duration planar point source](#causal-diffusion-from-a-finite-duration-planar-point-source)
    - [Cancellation of two heat-kernel impulses](#cancellation-of-two-heat-kernel-impulses)
- [Advection-diffusion equation](#advection-diffusion-equation)
  - [Drift-diffusion decay time](#drift-diffusion-decay-time)
  - [Homogenization of a periodic advection-diffusion equation](#homogenization-of-a-periodic-advection-diffusion-equation)
  - [Transported step forcing in an advection-diffusion equation](#transported-step-forcing-in-an-advection-diffusion-equation)
  - [Half-line advection-diffusion global relation](#half-line-advection-diffusion-global-relation)
  - [Constant-flux tracer inlet solution](#constant-flux-tracer-inlet-solution)
  - [Constant-concentration inlet solution](#constant-concentration-inlet-solution)
  - [Dirichlet gauge transform for constant drift](#dirichlet-gauge-transform-for-constant-drift)
    - [Mixed-boundary drift-diffusion eigenmodes on a rectangle](#mixed-boundary-drift-diffusion-eigenmodes-on-a-rectangle)
    - [Weighted sine transform for half-line drift diffusion](#weighted-sine-transform-for-half-line-drift-diffusion)
    - [Resolvent kernel for Dirichlet advection-diffusion on an interval](#resolvent-kernel-for-dirichlet-advection-diffusion-on-an-interval)
  - [Gamma impulse solution for linearly increasing diffusivity](#gamma-impulse-solution-for-linearly-increasing-diffusivity)
  - [Robin gauge transform for constant drift](#robin-gauge-transform-for-constant-drift)
  - [Weighted Neumann heat kernel with constant drift](#weighted-neumann-heat-kernel-with-constant-drift)
    - [Resolvent kernel for Neumann advection-diffusion on an interval](#resolvent-kernel-for-neumann-advection-diffusion-on-an-interval)
    - [Neumann boundary-forcing formula](#neumann-boundary-forcing-formula)
  - [Advection-diffusion heat-kernel solution](#advection-diffusion-heat-kernel-solution)
    - [Half-line drift reflection kernel](#half-line-drift-reflection-kernel)
- [Nonlinear diffusion equation](#nonlinear-diffusion-equation)
  - [Quadratic profiles for nonlinear diffusion with constant loss](#quadratic-profiles-for-nonlinear-diffusion-with-constant-loss)
  - [Logarithmic diffusion](#logarithmic-diffusion)
  - [Principal diffusion coefficients](#principal-diffusion-coefficients)
  - [Perona-Malik equation](#perona-malik-equation)
    - [Forward-backward threshold for gradient-weighted exponential diffusion](#forward-backward-threshold-for-gradient-weighted-exponential-diffusion)
    - [Regularized Perona-Malik diffusion](#regularized-perona-malik-diffusion)
  - [Two-dimensional Barenblatt solution with diffusivity proportional to concentration](#two-dimensional-barenblatt-solution-with-diffusivity-proportional-to-concentration)
    - [Linear-reaction time change for quadratic nonlinear diffusion](#linear-reaction-time-change-for-quadratic-nonlinear-diffusion)
- [Reaction–diffusion system](#reaction-diffusion-system)
  - [Cubic fast-slow reaction-diffusion model](#cubic-fast-slow-reaction-diffusion-model)
  - [Diffusion-driven stationary instability](#diffusion-driven-stationary-instability)
    - [Finite-domain selection of a reaction-diffusion instability](#finite-domain-selection-of-a-reaction-diffusion-instability)
    - [Equal diffusion cannot destabilize a stable reaction Jacobian](#equal-diffusion-cannot-destabilize-a-stable-reaction-jacobian)
  - [Removing a variable scalar reaction rate by an integrating factor](#removing-a-variable-scalar-reaction-rate-by-an-integrating-factor)
  - [Positivity of the first Dirichlet reaction-diffusion coefficient](#positivity-of-the-first-dirichlet-reaction-diffusion-coefficient)
  - [Dirichlet reaction-diffusion growth threshold in a cuboid](#dirichlet-reaction-diffusion-growth-threshold-in-a-cuboid)
  - [Bistable cubic reaction-diffusion equation](#bistable-cubic-reaction-diffusion-equation)
    - [Logistic front of a bistable cubic equation](#logistic-front-of-a-bistable-cubic-equation)
  - [Basally forced quadratic activator-inhibitor model](#basally-forced-quadratic-activator-inhibitor-model)
    - [Weak focus at the Hopf threshold of a basal activator-inhibitor model](#weak-focus-at-the-hopf-threshold-of-a-basal-activator-inhibitor-model)
    - [Turing threshold of a basally forced quadratic activator-inhibitor model](#turing-threshold-of-a-basally-forced-quadratic-activator-inhibitor-model)
  - [Inhibitor in a reaction-diffusion system](#inhibitor-in-a-reaction-diffusion-system)
  - [Activator in a reaction-diffusion system](#activator-in-a-reaction-diffusion-system)
  - [Quadratic activator-inhibitor model](#quadratic-activator-inhibitor-model)
    - [Turing threshold of the quadratic activator-inhibitor model](#turing-threshold-of-the-quadratic-activator-inhibitor-model)
    - [Positive-quadrant Dulac multiplier for quadratic activation](#positive-quadrant-dulac-multiplier-for-quadratic-activation)
  - [Spatially homogeneous equilibrium](#spatially-homogeneous-equilibrium)
  - [Morphogen reaction-diffusion equation](#morphogen-reaction-diffusion-equation)
    - [Mixed Dirichlet-Neumann modes on an interval](#mixed-dirichlet-neumann-modes-on-an-interval)
      - [Critical length for a linearly growing morphogen](#critical-length-for-a-linearly-growing-morphogen)
  - [Fast-inhibitor elimination in a reaction-diffusion system](#fast-inhibitor-elimination-in-a-reaction-diffusion-system)
    - [Dispersion relation after fast-inhibitor elimination](#dispersion-relation-after-fast-inhibitor-elimination)
  - [Turing pattern](#turing-pattern)
    - [Turing instability](#turing-instability)
      - [Fast-inhibitor cubic activator growth rate](#fast-inhibitor-cubic-activator-growth-rate)
      - [Two-species diffusion-driven instability criterion](#two-species-diffusion-driven-instability-criterion)
        - [Impossibility of a two-species Turing instability at equal diffusivities](#impossibility-of-a-two-species-turing-instability-at-equal-diffusivities)
        - [Near-unity diffusivity ratio for a Turing instability](#near-unity-diffusivity-ratio-for-a-turing-instability)
  - [Brusselator](#brusselator)
    - [Hopf coefficient of the Brusselator](#hopf-coefficient-of-the-brusselator)
    - [Brusselator trapping region](#brusselator-trapping-region)
    - [Brusselator periodic-orbit criterion](#brusselator-periodic-orbit-criterion)
    - [Turing threshold of the Brusselator](#turing-threshold-of-the-brusselator)
      - [Discrete-mode Turing threshold for the Brusselator](#discrete-mode-turing-threshold-for-the-brusselator)
      - [Brusselator Turing-before-Hopf diffusivity condition](#brusselator-turing-before-hopf-diffusivity-condition)

## Scalar integrating factor for a reaction-diffusion equation

↑ **Parent:** [Diffusion equation](diffusion-equation.md)

A spatially uniform time-dependent reaction coefficient can be removed from a linear [diffusion equation](diffusion-equation.md) by a scalar [integrating factor](linear-ordinary-differential-equation.md#integrating-factor). If $A'(t)=a(t)$ and $v=e^{A(t)}u$, substitution gives $u_t=u_{xx}$. Initial data and boundary values must also be divided by $e^{A(t)}$. A nonzero boundary profile can then be removed by [boundary lifting](boundary-value-problem.md#boundary-lifting) before applying [separation of variables](partial-differential-equation.md#separation-of-variables). This reduction distinguishes growth of the whole amplitude from decay of the spatial diffusion modes.

## Squared diffusion-residual action

↑ **Parent:** [Diffusion equation](diffusion-equation.md)

For constant $\nu$, variation of this positive functional gives $(\partial_t+\nu\nabla^2)(\partial_t-\nu\nabla^2)h=0$, or $h_{tt}-\nu^2\nabla^4h=0$. The [diffusion equation](diffusion-equation.md) $h_t=\nu\nabla^2h$ gives zero-residual minima, but is only a subset of the stationary equations of the squared functional. Each nonzero spatial [Fourier mode](fourier-analysis.md#fourier-mode) has both growing and decaying temporal solutions in the stationary equation. Boundary data decide which stationary paths are admissible. In two spatial dimensions, the bulk action is invariant under the anisotropic [scale invariance](mathematics.md#scale-invariance) $x\mapsto bx$, $t\mapsto b^2t$, $h\mapsto h$.

### Time reversal of the squared diffusion-residual action

↑ **Parent:** [Squared diffusion-residual action](#squared-diffusion-residual-action)

For a real scalar height field, [integration by parts](calculus.md#integration-by-parts) gives

$$
(h_t-\nu\nabla^2h)^2=h_t^2+\nu^2(\nabla^2h)^2+\nu\partial_t|\nabla h|^2-2\nu\nabla\cdot(h_t\nabla h).
$$

The bulk expression is even under [time reversal](quantum-field-theory.md#t-symmetry). The original density is not pointwise even, but changes by a [total divergence](multivariable-calculus.md#total-divergence); its stationary equation is time-reversal invariant. The first-order [diffusion equation](diffusion-equation.md) selected by zero residual is not invariant under ordinary time reversal at fixed positive $\nu$. Boundary conditions or the probabilistic interpretation can distinguish the two time directions even when the higher-order stationary equation does not.

## Robin diffusion with a growing mode

↑ **Parent:** [Diffusion equation](diffusion-equation.md)

These [Robin boundary conditions](differential-equation.md#robin-boundary-condition) give the spatial [Sturm-Liouville operator](sturm-liouville-theory.md#sturm-liouville-operator) $-d^2/dx^2$ one negative [eigenvalue](linear-operator-theory.md#eigenvalue), $-1$, with [eigenfunction](linear-operator-theory.md#eigenfunction) $e^x$. The other eigenvalues are $n^2\pi^2$, with eigenfunctions $V_n=n\pi\cos(n\pi x)+\sin(n\pi x)$, $n\geq1$; there is no zero eigenvalue. Hence the [diffusion equation](diffusion-equation.md) has a growing contribution $c_0e^{t+x}$ in addition to decaying modes.

There is no contradiction with ordinary diffusive smoothing. The outward [normal derivative](differential-geometry.md#normal-derivative) is $-u_x$ at the left endpoint and $u_x$ at the right endpoint, so imposing the same coordinate derivative at both ends does not impose dissipative outward-normal data at both ends. The energy identity is $\tfrac12\partial_t\int u^2=[uu_x]_0^1-\int u_x^2$, whose boundary term is $u(1)^2-u(0)^2$ here and can supply energy. Orthogonal projection of initial data $f$ gives $c_0=2\int_0^1fe^x\,dx/(e^2-1)$; it vanishes precisely when the growing mode is absent.

The reflected boundary conditions $u_x(0,t)=-u(0,t)$ and $u_x(1,t)=-u(1,t)$ have the same spectrum, because reflection $x\mapsto1-x$ reverses the coordinate derivative. Here the growing eigenfunction is $e^{-x}$ and the decaying functions are $W_n=n\pi\cos(n\pi x)-\sin(n\pi x)$, giving

$$
u(x,t)=c_0e^{t-x}+\sum_{n\geq1}c_ne^{-n^2\pi^2t}W_n(x).
$$

For square-integrable initial data $f$, [orthogonal projection](hilbert-space.md#orthogonal-projection) gives

$$
c_0=\frac{2}{1-e^{-2}}\int_0^1e^{-x}f(x)dx,\qquad c_n=\frac{2}{n^2\pi^2+1}\int_0^1W_n(x)f(x)dx.
$$

The norms are $(1-e^{-2})/2$ and $(n^2\pi^2+1)/2$. The spatial [Sturm-Liouville problem](sturm-liouville-theory.md#sturm-liouville-problem) has no zero eigenvalue and exactly one negative eigenvalue for $-D^2$, namely $-1$. The energy boundary term now reads $u(0)^2-u(1)^2$, so the left endpoint can supply energy. The growing mode disappears exactly when $\int_0^1e^{-x}f(x)dx=0$.

## Drift-diffusion equation with a potential

↑ **Parent:** [Diffusion equation](diffusion-equation.md)

For positive [diffusivity](brownian-motion.md#diffusion-coefficient) $D(x)$, a [diffusion equation](diffusion-equation.md) with potential-driven drift has [diffusive flux](mathematical-physics.md#diffusive-flux) $J=-D(c_x+\beta V'c)$. On a finite interval with zero [flux](mathematical-physics.md#flux) at both endpoints, the total amount is conserved. The substitution $c=e^{-\lambda t}e^{-\beta V}y$ converts the decay [eigenvalue problem](linear-operator-theory.md#eigenvalue-problem) to the [Sturm-Liouville problem](sturm-liouville-theory.md#sturm-liouville-problem)

$$
-(py')'=\lambda wy,\qquad p=De^{-\beta V},\quad w=e^{-\beta V},\quad py'=0\text{ at the endpoints}.
$$

The [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) is $\lambda=\int p|y'|^2/\int w|y|^2\geq0$. Its zero [eigenfunction](linear-operator-theory.md#eigenfunction) is constant, giving the [stationary solution](differential-equation.md#stationary-solution) $c_{\rm eq}=C e^{-\beta V}$. This is a spatial [Boltzmann distribution](thermodynamics.md#boltzmann-distribution); $D$ changes relaxation rates but cancels out of the zero-[flux](mathematical-physics.md#flux) equilibrium profile. For a sufficiently regular positive $D$ and bounded $V$, the constant eigenfunction is the unique zero mode up to scale.

## Diffusive time scale

↑ **Parent:** [Diffusion equation](diffusion-equation.md)

A concentration varying over length $L$ has Laplacian of order its amplitude divided by $L^2$. Balancing the time derivative with $\kappa\Delta\chi$ in the [diffusion equation](diffusion-equation.md) gives the displayed relaxation time. A [multiple-scale expansion](singular-perturbation.md#method-of-multiple-scales) with spatial scale $\varepsilon x$ therefore uses slow time $\varepsilon^2t$ when the effective [diffusivity](brownian-motion.md#diffusion-coefficient) is of order one.

## Variable-coefficient conservative diffusion equation

↑ **Parent:** [Diffusion equation](diffusion-equation.md)

With positive diffusion coefficient $a(x)$, this [diffusion equation](diffusion-equation.md) expresses conservation with flux $-a(x)u_x$. For a differentiable coefficient, its spatial operator is $a u_{xx}+a'u_x$, rather than either $a u_x$ or $a u_{xx}$ alone. A [symmetric half-grid diffusion consistency](finite-difference.md#symmetric-half-grid-diffusion-consistency) discretization uses the difference of the two adjacent interface fluxes, preserving that divergence structure. Suitable [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) make the spatial operator dissipative in the [L2 norm](real-analysis.md#l2-norm).

## Infinite propagation speed

↑ **Parent:** [Diffusion equation](diffusion-equation.md)

Infinite propagation speed means that a disturbance initially confined to a bounded region can affect arbitrarily distant points after any positive time. The strictly positive [heat kernel](#heat-kernel) gives this behavior for a nontrivial nonnegative diffusion solution. It contrasts with the [finite propagation speed](wave-equation.md#finite-propagation-speed) of the [wave equation](wave-equation.md); a very small distant response is still mathematically nonzero.

## Periodic homogenization of a diffusion equation

↑ **Parent:** [Diffusion equation](diffusion-equation.md)

For $u_t=\partial_x[a(x/\epsilon)u_x]$ with positive periodic $a$, the one-dimensional homogenized diffusivity is the harmonic mean $a_{\rm eff}=\langle a^{-1}\rangle^{-1}$. Microscopic flux continuity produces this harmonic rather than arithmetic averaging.

## Porous medium equation

↑ **Parent:** [Diffusion equation](diffusion-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Porous_medium_equation)

The porous medium equation $u_t=\Delta(u^m)$ with $m>1$ is a [nonlinear partial differential equation](partial-differential-equation.md#nonlinear-partial-differential-equation) whose diffusivity vanishes at $u=0$. Unlike the [heat equation](#heat-equation), it has compactly supported solutions with finite propagation speed.

### Spherical nonlinear-diffusion source profile

↑ **Parent:** [Porous medium equation](#porous-medium-equation)

For $C_t=k\nabla\cdot(C\nabla C)$ in three dimensions and total mass $4\pi M$, the nonnegative radial source solution is $C=M^{2/5}(kt)^{-3/5}f(r/(Mkt)^{1/5})$, with $f(\xi)=(75^{2/5}-\xi^2)_+/10$. Integrating the similarity equation once gives $ff'=-\xi f/5$, and normalization $\int_0^\infty\xi^2f\,d\xi=1$ fixes the compact-support radius. The flux vanishes at the moving front, so the profile solves the equation weakly and approaches the prescribed point mass as time tends to zero.

### Compact radial cubic-diffusion profile

↑ **Parent:** [Porous medium equation](#porous-medium-equation)

For the planar diffusion equation $n_t=D_0\nabla\cdot[(n/n_0)^2\nabla n]$, a mass-preserving radial [similarity solution](partial-differential-equation.md#similarity-solution) has $n=n_0\lambda^{-2}F(r/(r_0\lambda))$. Substitution reduces the equation to $(\xi F^2F')'=-(\xi^2F)'$ when $\lambda^5\dot\lambda=D_0/r_0^2$. Zero central flux and $F(0)=1$ give the compact profile shown above, with $\lambda^6=6D_0t/r_0^2$. Its height decays as $t^{-1/3}$ and its radius grows as $t^{1/6}$; its total mass is $2\pi n_0r_0^2/3$.

### Finite propagation in porous-medium diffusion

↑ **Parent:** [Porous medium equation](#porous-medium-equation)

In a [porous medium equation](#porous-medium-equation) with exponent $m>1$, the effective [diffusion coefficient](brownian-motion.md#diffusion-coefficient) vanishes at zero density. A nonnegative compactly supported source profile can therefore retain a finite front for every finite positive time. For example, the [radial cubic-diffusion source profile](#radial-cubic-diffusion-source-profile) has support radius proportional to $t^{1/6}$. This notion concerns a moving diffusion front; it does not require the constant characteristic cone used for a [wave equation](wave-equation.md).

### Forced filling similarity for power-law diffusion

↑ **Parent:** [Porous medium equation](#porous-medium-equation)

Consider a [nonlinear diffusion equation](#nonlinear-diffusion-equation) with uniform supply, $\phi h_t=D_m(h^m h_x)_x+R$, on $x>0$, with an absorbing boundary $h(0,t)=0$ and initially $h=0$. Far from the boundary, $h=Rt/\phi$. Balancing the [time derivative](multivariable-calculus.md#time-derivative), supply, and diffusion gives

$$
h=\frac{Rt}{\phi}F(\eta),\qquad \eta=\frac{x}{\ell(t)},\qquad \ell(t)=\left[\frac{D_mR^m t^{m+1}}{\phi^{m+1}}\right]^{1/2}.
$$

The [similarity solution](partial-differential-equation.md#similarity-solution) satisfies

$$
(F^mF')'+1-F+\frac{m+1}{2}\eta F'=0,\qquad F(0)=0,\qquad F(\infty)=1.
$$

The outward boundary [volume flux per unit width](fluid-mechanics.md#volume-flux-per-unit-width) is $Q=R\ell c_m$, where $c_m=\lim_{\eta\downarrow0}F^mF'$. Integrating the equation gives

$$
c_m=\frac{m+3}{2}\int_0^\infty(1-F)\,d\eta.
$$

Thus the growing region of depleted storage fixes the discharge prefactor, and $Q\propto t^{(m+1)/2}$.

### Separable draining profile for power-law diffusion

↑ **Parent:** [Porous medium equation](#porous-medium-equation)

For $\phi h_t=D_m(h^m h_x)_x$ on $0<x<L$, with $h(0,t)=0$ and zero right-hand [volume flux](fluid-mechanics.md#volumetric-flow-rate), a [separation of variables](partial-differential-equation.md#separation-of-variables) gives

$$
h=\left(\frac{\phi L^2}{mD_m\tau}\right)^{1/m}F(x/L),\qquad \tau=t+t_0,
$$

where the positive profile satisfies

$$
(F^mF')'+F=0,\qquad F(0)=0,\qquad F'(1)=0.
$$

Its boundary [volume flux per unit width](fluid-mechanics.md#volume-flux-per-unit-width) is

$$
Q=\frac{D_m}{L}\left(\frac{\phi L^2}{mD_m\tau}\right)^{(m+1)/m}c_m,\qquad c_m=\lim_{\xi\downarrow0}F^mF'=\int_0^1F\,d\xi.
$$

These profiles are exact separated solutions and describe the leading long-time discharge for a broad class of positive initial data. The virtual origin $t_0$ depends on the initial profile; it does not make the separated solution an exact representation of every initial condition.

### Barenblatt solution

↑ **Parent:** [Porous medium equation](#porous-medium-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Barenblatt_solution)

The Barenblatt solution is a mass-preserving [similarity solution](partial-differential-equation.md#similarity-solution) of the [porous medium equation](#porous-medium-equation). For $u_t=\beta(uu_x)_x$ in one dimension it has the form

$$
u(x,t)=\left[A t^{-1/3}-\frac{x^2}{6\beta t}\right]_+.
$$

#### Radial cubic-diffusion source profile

↑ **Parent:** [Barenblatt solution](#barenblatt-solution)

For the planar [porous medium equation](#porous-medium-equation) $n_t=[D_0/(3n_0^2)]\Delta(n^3)$, the mass-$Q$ point-source [similarity solution](partial-differential-equation.md#similarity-solution) is $n=n_0\lambda^{-2}\sqrt{[1-r^2/(r_0^2\lambda^2)]_+}$, with $\lambda=(6D_0t/r_0^2)^{1/6}$ and $r_0^2=3Q/(2\pi n_0)$. Its front grows as $t^{1/6}$ and its central density falls as $t^{-1/3}$. The [mass conservation](continuum-mechanics.md#mass-conservation) integral uses the planar area element $2\pi r\,dr$. Although the density slope diverges at the front, its diffusion flux vanishes there, giving a compactly supported [weak solution](partial-differential-equation.md#weak-solution) with initial measure $Q\delta^{(2)}$.

#### Planar volume-conserving nonlinear-diffusion similarity

↑ **Parent:** [Barenblatt solution](#barenblatt-solution)

For $n,A>0$, the one-dimensional [porous medium equation](#porous-medium-equation) $h_t=A(h^nh_x)_x$ has a volume-preserving [similarity solution](partial-differential-equation.md#similarity-solution) $h=[c_n(R^2-x^2)/(At)]_+^{1/n}$, where $c_n=n/[2(n+2)]$ and $R\propto t^{1/(n+2)}$. On a reflecting half-line with conserved area $M$, $R=[M(At/c_n)^{1/n}/I_n]^{n/(n+2)}$, where $I_n=\tfrac12 B(\tfrac12,1+1/n)$. For a whole symmetric release use half its total area as $M$. The [Beta function](complex-analysis.md#beta-function) fixes normalization, while finite-front zero [volume flux](fluid-mechanics.md#volumetric-flow-rate) fixes the edge condition.

##### Semicircular pulse under cubic diffusion

↑ **Parent:** [Planar volume-conserving nonlinear-diffusion similarity](#planar-volume-conserving-nonlinear-diffusion-similarity)

The source-type [similarity solution](partial-differential-equation.md#similarity-solution) of $h_t=D(h^2h_x)_x$ with whole-line conserved area $\mathcal V$ is $h=H(t)[1-x^2/L(t)^2]_+^{1/2}$, where $L=2(\mathcal V/\pi)^{1/2}(Dt)^{1/4}$ and $H=(\mathcal V/\pi)^{1/2}(Dt)^{-1/4}$. Its [volume flux](fluid-mechanics.md#volumetric-flow-rate) vanishes at the finite front, while the velocity tends to $\dot L=L/(4t)$. A reflecting half-line uses twice its prescribed area in these formulas.

#### Two-dimensional Barenblatt profile for quadratic porous-medium diffusion

↑ **Parent:** [Barenblatt solution](#barenblatt-solution)

For the radially symmetric equation

$$
n_t=D\nabla\cdot(n\nabla n)
$$

in two dimensions, the mass-$N$ similarity solution has the compactly supported form

$$
n(r,t)=\left(\frac N{Dt}\right)^{1/2}
\left[\frac{x_0^2-x^2}{8}\right]_+,
\qquad
x=\frac r{(NDt)^{1/4}},
$$

where mass normalization gives $x_0=(16/\pi)^{1/4}$. Its support radius grows as $t^{1/4}$ and its occupied area grows as $t^{1/2}$.

<h2 id="fick-s-first-law">Fick's first law</h2>

↑ **Parent:** [Diffusion equation](diffusion-equation.md)

[Fick's laws](mathematical-physics.md#fick-s-laws) describe diffusion through a flux law and [conservation of mass](continuum-mechanics.md#mass-conservation). The first law says that [diffusive flux](mathematical-physics.md#diffusive-flux) points down the concentration [gradient](multivariable-calculus.md#gradient):

$$
\mathbf J=-D(C)\nabla C.
$$

Combining it with local conservation gives  
$C_t=\nabla\cdot(D(C)\nabla C)$.

## Heat equation

↑ **Parent:** [Diffusion equation](diffusion-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heat_equation)

The heat equation

$$
u_t=D\nabla^2u,
\qquad D>0,
$$

models diffusion with constant diffusivity $D$.

### Heat balance with volumetric heat generation

↑ **Parent:** [Heat equation](#heat-equation)

Integrating [energy](energy.md) conservation over a fixed material volume gives storage equal to incoming conductive [heat flux](heat.md#heat-flux-density) plus internally generated [heat](heat.md). Here $c_{\rm vol}$ is [volumetric heat capacity](heat.md#volumetric-heat-capacity), with units $\mathrm{J\,m^{-3}\,K^{-1}}$. For a mass-specific [heat capacity](heat.md#heat-capacity), the [density](fluid-mechanics.md#density) factor must be included. Constant isotropic conductivity reduces the divergence to $k\nabla^2T$; variable conductivity must remain inside the divergence.

### Annual ground-temperature wave

↑ **Parent:** [Heat equation](#heat-equation)

A sinusoidal surface [temperature](temperature.md) applied to a homogeneous semi-infinite conductor produces a periodic depth profile with penetration length $\delta=\sqrt{2\kappa/(\omega C)}$. It follows by substituting a complex exponential into $C\partial_tT=\kappa\partial_z^2T$ and taking the root that decays at depth. A depth $z$ attenuates the amplitude by $e^{-z/\delta}$ and delays the phase by $z/\delta$. This is [diffusion](thermodynamics.md#diffusion) with phase delay, rather than a nondispersive travelling wave.

### Fixed-temperature and fixed-flux heat equation on an interval

↑ **Parent:** [Heat equation](#heat-equation)

For positive thermal [diffusivity](brownian-motion.md#diffusion-coefficient) $\nu$, [thermal conductivity](heat.md#thermal-conductivity) $k$ and length $L$, subtract the [stationary solution](differential-equation.md#stationary-solution) $w(x)=Hx/k$. The remainder satisfies the [heat equation](#heat-equation) with a homogeneous [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) at zero and a homogeneous [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) at $L$. The [mixed Dirichlet-Neumann modes on an interval](#mixed-dirichlet-neumann-modes-on-an-interval) are $\sin(k_nx)$, where $k_n=(n+1/2)\pi/L$. Thus for an initial [temperature](temperature.md) profile $u_0$,

$$
u(x,t)=\frac{Hx}k+\sum_{n=0}^\infty b_n\sin(k_nx)e^{-\nu k_n^2t},\qquad b_n=\frac2L\int_0^L\left(u_0(x)-\frac{Hx}k\right)\sin(k_nx)dx.
$$

For zero initial [temperature](temperature.md), $b_n=-2H(-1)^n/(kLk_n^2)$. The series gives the initial profile in the usual [Fourier series](fourier-series.md) sense and a smooth solution for $t>0$. If $H\ne0$, the zero initial profile does not satisfy the prescribed endpoint derivative at $t=0$: the [temperature](temperature.md) can be continuous there without its spatial [derivative](calculus.md#derivative) extending continuously to that corner. The sign $k u_x(L,t)=H>0$ describes incoming [heat flux](heat.md#heat-flux-density), since the outward conductive [heat flux](heat.md#heat-flux-density) is $-k u_x$.

### Heat flow from a triangular initial temperature

↑ **Parent:** [Heat equation](#heat-equation)

On $0<x<L$ with zero-temperature endpoints, let the initial [temperature](temperature.md) rise linearly from zero to height $H$ at $L/2$ and then fall linearly to zero. [Integration by parts](calculus.md#integration-by-parts) on the two halves gives [Fourier sine series](fourier-series.md#fourier-sine-series) coefficients $8H\sin(n\pi/2)/(\pi^2n^2)$. Under the [heat equation](#heat-equation) $T_t=DT_{xx}$ with $D>0$, each coefficient decays by $e^{-D(n\pi/L)^2t}$, giving the displayed solution. Only odd spatial modes occur; absolute coefficient summability proves [uniform convergence](sequence-and-series.md#uniform-convergence) for $t\geq0$ via the [Weierstrass M-test](probability-and-statistics.md#weierstrass-m-test). This spatial profile also occurs in a [midpoint-plucked fixed-end string](wave-equation.md#midpoint-plucked-fixed-end-string), where the time factors oscillate instead of decaying.

#### Heat flow from a triangular initial temperature with insulated endpoints

↑ **Parent:** [Heat flow from a triangular initial temperature](#heat-flow-from-a-triangular-initial-temperature)

On a bar of length $L$, let the initial [temperature](temperature.md) increase linearly from zero at either endpoint to height $H$ at the midpoint. With thermal diffusivity $D>0$ and insulated [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition), a [Fourier cosine series](fourier-series.md#fourier-cosine-series) gives the displayed solution. Its constant term is the initial [integral average](measure-theory.md#integral-average) $H/2$. [Integration by parts](calculus.md#integration-by-parts) on the two straight segments gives zero coefficients for odd modes and modes divisible by four; the remaining coefficients are $-4H/[\pi^2(2j+1)^2]$. Nonconstant modes decay, leaving the uniform temperature $H/2$, consistent with conservation of the total heat. This contrasts with the zero-temperature boundary solution in [heat flow from a triangular initial temperature](#heat-flow-from-a-triangular-initial-temperature), where heat can leave the bar and the limit is zero. The initial endpoint slopes do not satisfy the insulated condition, so derivatives need not converge to their initial endpoint values as $t\downarrow0$; the series satisfies the Neumann condition for every $t>0$ and recovers the continuous initial profile.

### Cooling of an initially uniform square

↑ **Parent:** [Heat equation](#heat-equation)

For a square of side $\ell$ initially at constant temperature $T_0$, held at zero boundary temperature for $t>0$, the [heat equation](#heat-equation) $T_t=\kappa\Delta T$ with $\kappa>0$ has solution

$$
T=\frac{16T_0}{\pi^2}\sum_{\substack{m,n\geq1\\m,n\text{ odd}}}\frac{\sin(m\pi x/\ell)\sin(n\pi y/\ell)}{mn}\,e^{-\kappa\pi^2(m^2+n^2)t/\ell^2}.
$$

The [double Fourier sine series](fourier-series.md#double-fourier-sine-series) of the initial constant gives the coefficients. The spatial modes are [Dirichlet Laplacian eigenfunctions](partial-differential-equation.md#dirichlet-laplacian-eigenfunction), so [separation of variables](partial-differential-equation.md#separation-of-variables) gives their decay rates. At late times the $(1,1)$ mode dominates, giving the displayed profile; the next nonzero decay exponent is $10\kappa\pi^2/\ell^2$. At early times the series approaches the constant at each interior point and in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space), while the boundary remains at zero. An instantaneous change to the boundary condition therefore need not produce a solution continuous at the initial boundary in space-time.

### Periodic diffusion on a circle

↑ **Parent:** [Heat equation](#heat-equation)

For a circle of circumference $2\pi$, the [heat equation](#heat-equation) $u_t=Du_{xx}$ has periodic matching of both $u$ and $u_x$ at $x=\pm\pi$. For $D>0$, the displayed [Fourier series](fourier-series.md) solves the initial-value problem, with $\bar f=(2\pi)^{-1}\int_{-\pi}^\pi f(x)dx$ and the usual real [Fourier coefficients](fourier-series.md#fourier-coefficient). Every nonconstant [normal mode](wave-equation.md#normal-mode) decays, leaving the conserved mean. In particular $f(x)=(\pi-|x|)^2$ gives $\bar f=\pi^2/3$, $a_n=4/n^2$ and $b_n=0$. The initial cusp is smoothed for every positive time.

#### Periodic sine with an endpoint-correcting linear term

↑ **Parent:** [Periodic diffusion on a circle](#periodic-diffusion-on-a-circle)

For $L>0$, extend $f_L(x)=\sin x-x\sin L/L$ from $[-L,L]$ periodically. The linear term makes both endpoint values zero and the endpoint first [derivatives](calculus.md#derivative) match. The function is [odd](calculus.md#odd-function), so its [Fourier series](fourier-series.md) has only sine terms, with the displayed [Fourier coefficients](fourier-series.md#fourier-coefficient). Indeed, for $k_n=n\pi/L\ne1$,

$$
\int_0^L\sin x\sin(k_nx)dx=\frac{(-1)^nk_n\sin L}{1-k_n^2},\qquad \int_0^Lx\sin(k_nx)dx=-\frac{L(-1)^n}{k_n};
$$

subtracting and multiplying by $2/L$ proves the formula. The coefficients decay as $O(n^{-3})$. At $L=m\pi$, the single coefficient $b_m$ has removable [limit](calculus.md#limit-of-a-function) $1$, with all others zero. Multiplying $b_n$ by $e^{-\kappa k_n^2t}$ solves the corresponding [heat equation](#heat-equation) on the [circle](topology.md#circle).

### Heat equation with a single stationary sine forcing

↑ **Parent:** [Heat equation](#heat-equation)

On $0<x<L$, let $u_t=\nu u_{xx}+G\sin(n\pi x/L)$, with $\nu>0$, zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), and zero initial data. Write $k_n=n\pi/L$. Its stationary solution is $u_s=G\sin(k_nx)/(\nu k_n^2)$. Subtracting it removes the forcing from the [partial differential equation](partial-differential-equation.md) and leaves a [heat equation](#heat-equation) with initial data $-u_s$.

Because the forcing is a single spatial [eigenfunction](linear-operator-theory.md#eigenfunction), [separation of variables](partial-differential-equation.md#separation-of-variables) gives the entire solution without mixing modes:

$$
u(x,t)=\frac{G}{\nu k_n^2}(1-e^{-\nu k_n^2t})\sin(k_nx).
$$

Its integral is $G[1-(-1)^n](1-e^{-\nu k_n^2t})/(\nu k_n^3)$; [even](calculus.md#even-function) modes have zero signed net integral. Removing forcing from the evolution equation does not remove its amplitude from the initial data for the transient.

### Steady temperature of a uniformly heated cylindrical wire

↑ **Parent:** [Heat equation](#heat-equation)

For a long homogeneous circular wire of radius $a$, uniform volumetric heating $H$, constant [thermal conductivity](heat.md#thermal-conductivity) $\kappa$ and negligible end losses, the steady [heat equation](#heat-equation) is $\kappa\rho^{-1}(\rho T')'+H=0$. Regularity at the axis excludes a [logarithm](calculus.md#logarithm) term, giving $T=T_s+H(a^2-\rho^2)/(4\kappa)$. If the surface obeys [Newton's law of cooling](linear-ordinary-differential-equation.md#newton-s-law-of-cooling), $-\kappa T'(a)=\gamma(T_s-T_{\rm air})$, then $T_s=T_{\rm air}+Ha/(2\gamma)$. Here $\gamma$ has units $\mathrm{W\,m^{-2}K^{-1}}$ and $H$ has units $\mathrm{W\,m^{-3}}$. For uniform [electric current](electric-charge.md#electric-current) $I$ and constant [electrical conductivity](electric-charge.md#electrical-conductivity) $\sigma$, [Joule heating](electric-charge.md#joule-heating) gives $H=I^2/(\sigma\pi^2a^4)$.

### Fundamental diffusion mode

↑ **Parent:** [Heat equation](#heat-equation)

For a [diffusion equation](diffusion-equation.md) with fixed homogeneous [boundary conditions](differential-equation.md#boundary-condition), a fundamental diffusion mode is an [eigenfunction](linear-operator-theory.md#eigenfunction) of its nonnegative decay operator belonging to the smallest decay [eigenvalue](linear-operator-theory.md#eigenvalue) $\nu_0$, when such an [eigenvalue](linear-operator-theory.md#eigenvalue) exists. It is the slowest decaying separated [normal mode](wave-equation.md#normal-mode). With a discrete [spectrum](linear-operator-theory.md#spectrum-functional-analysis) and an isolated lowest [eigenvalue](linear-operator-theory.md#eigenvalue), initial data having a nonzero projection onto its [eigenspace](linear-operator-theory.md#eigenspace) approach this decay law at late times. Strongly vanishing [thermal diffusivity](heat.md#thermal-diffusivity) can destroy existence of a lowest mode, as illustrated by the [loss of a spectral gap under strongly degenerate radial diffusion](linear-operator-theory.md#loss-of-a-spectral-gap-under-strongly-degenerate-radial-diffusion).

### Heat equation on a rectangle with two insulated sides

↑ **Parent:** [Heat equation](#heat-equation)

On $0<x<a$, $0<y<b$, impose zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) at $x=0,a$ and zero [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) at $y=0,b$. [Separation of variables](partial-differential-equation.md#separation-of-variables) for $T_t=\lambda\Delta T$ gives the displayed sine-cosine expansion. The zero cosine mode must be included: its norm is $b$, whereas the positive cosine modes have norm $b/2$. Thus $A_{n0}=2(ab)^{-1}\int\!\int T_0\sin(n\pi x/a)$ and $A_{nm}=4(ab)^{-1}\int\!\int T_0\sin(n\pi x/a)\cos(m\pi y/b)$ for $m\geq1$. Expanding $x(a-x)$ gives sine coefficient $4a^2[1-(-1)^n]/(n^3\pi^3)$. Initial data $x(a-x)\sin^2(2\pi y/b)$ therefore involve only $m=0,4$ and odd $n$. Their leading long-time mode is $4a^2\sin(\pi x/a)e^{-\lambda\pi^2t/a^2}/\pi^3$.

### Reaction-diffusion spectral decay threshold

↑ **Parent:** [Heat equation](#heat-equation)

On the unit interval with zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), $u_t=u_{xx}+\kappa u$ has sine-mode growth rates $\kappa-j^2\pi^2$. Every finite-energy initial condition decays exactly when the largest rate is negative, namely $\kappa<\pi^2$. A centered [finite difference](finite-difference.md) grid with $h=1/(M+1)$ has eigenvectors $\sin(j\pi m/(M+1))$ and growth rates $\kappa-4h^{-2}\sin^2(j\pi/(2(M+1)))$. Its all-data decay threshold is the displayed $\kappa_h$, strictly less than $\pi^2$ and approaching it from below. Equality leaves a stationary lowest mode; exceeding the threshold allows growth.

#### Spherical reaction-diffusion growth threshold

↑ **Parent:** [Reaction-diffusion spectral decay threshold](#reaction-diffusion-spectral-decay-threshold)

For $n_t=D\Delta n+\gamma n$ in a sphere of radius $a$, with zero surface density and regularity at the origin, the lowest spherically symmetric [normal mode](wave-equation.md#normal-mode) is $n(r,t)=n_c\sin(\pi r/a)/(\pi r/a)\exp[(\gamma-\pi^2D/a^2)t]$. Substitution of $R=f/r$ in the radial [Laplacian](multivariable-calculus.md#laplacian) gives $f''+k^2f=0$, and regularity removes the cosine solution. The [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) gives $k=m\pi/a$; a radial mode with no interior zeros requires $m=1$. Thus [diffusion](thermodynamics.md#diffusion) leakage suppresses growth below the displayed threshold, while the mode is stationary at equality. The expression at $r=0$ uses its continuous limit. In a linear [neutron](neutron.md) multiplication model this is the competition between bulk production and surface loss.

### Heat evolution of bounded data need not converge at large times

↑ **Parent:** [Heat equation](#heat-equation)

Bounded smooth initial data alone do not guarantee a pointwise large-time limit for the [heat equation](#heat-equation) on Euclidean space. In four dimensions, $g(x)=(1+|x|^2)^i$ has modulus one. At the origin its [heat kernel](#heat-kernel) average is asymptotic to $4^i\Gamma(2+i)t^i$, which oscillates indefinitely. Initial data vanishing at infinity do have heat averages tending to zero. This distinction matters when using [Duhamel principle](#duhamel-s-principle) to construct a stationary solution for a time-independent source.

### Dirichlet heat-reaction threshold on the unit square

↑ **Parent:** [Heat equation](#heat-equation)

For zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) on the unit square, the modes $2\sin(j\pi x)\sin(k\pi y)$ have heat-reaction growth rates $\kappa-\pi^2(j^2+k^2)$. Their largest rate is $\kappa-2\pi^2$. Hence the solution is an [L2 norm](real-analysis.md#l2-norm) contraction for $\kappa\leq2\pi^2$ and decays uniformly at positive times as $t\to\infty$ when the inequality is strict. At equality the first sine mode is stationary. For larger fixed $\kappa$ the equation remains well posed on every finite time interval, but has a growing mode; long-time contractivity is a different property from finite-time well-posedness.

### Heat operator

↑ **Parent:** [Heat equation](#heat-equation)

For the sign convention $\Delta=\operatorname{div}\nabla$, the heat operator is the [differential operator](analysis.md#differential-operator) $L=\partial_t-\Delta$. The [heat equation](#heat-equation) is $Lu=0$. If $P=-\Delta$ is the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator), the same operator is $\partial_t+P$. A [Riemannian heat kernel](#riemannian-heat-kernel) is a fundamental solution with the initial [Dirac delta distribution](distribution-theory.md#dirac-delta-function).

### Heat-equation uniqueness under Gaussian growth

↑ **Parent:** [Heat equation](#heat-equation)

Classical [heat equation](#heat-equation) solutions with identical [continuous](calculus.md#continuous-function) initial data and a uniform Gaussian spatial growth bound on each finite time interval are unique. For the zero-data difference, choose $b>a$ and compare on a short slab with $\varepsilon\Phi_b$, where $\Phi_b=(1-4bt)^{-n/2}\exp(b|x|^2/(1-4bt))$ solves the equation for $t<1/(4b)$. Its faster spatial growth controls the lateral boundary of large cylinders. The [heat equation maximum principle](#heat-equation-maximum-principle) bounds both signs of the difference by $\varepsilon\Phi_b$ inside. Increasing the cylinder radius and then sending $\varepsilon$ to zero proves uniqueness on that slab; repeating slabs covers the finite interval.

### Backward heat equation

↑ **Parent:** [Heat equation](#heat-equation)

A [Fourier mode](fourier-analysis.md#fourier-mode) has multiplier $e^{Dk^2t}$, amplifying arbitrarily small high-frequency data. For a fixed positive time $t_0$, initial modes $e^{-Dn^2t_0/2}\sin(nx)$ tend to zero in $L^2$ while their values at $t_0$ grow without bound. This violates [continuous dependence on initial data](partial-differential-equation.md#continuous-dependence-on-initial-data) and gives an [ill-posed problem](partial-differential-equation.md#ill-posed-problem) in ordinary unweighted spaces. An analytic-data restriction or physical short-scale regularization changes that conclusion.

#### Space-time harmonic functions along Brownian motion

↑ **Parent:** [Backward heat equation](#backward-heat-equation)

For $f\in C^2(\mathbb R^2)$ and standard [Brownian motion](brownian-motion.md) $B$, the drift in [Itô formula](stochastic-calculus.md#ito-s-lemma) for $f(B_t,t)$ vanishes exactly when the displayed equation holds for every spatial point and every $t\geq0$. Necessity follows because a zero finite-variation integral has continuous integrand $f_t(B_t,t)+\tfrac12f_{xx}(B_t,t)$ equal to zero, and at every positive time the [normal distribution](probability-distribution.md#normal-distribution) of $B_t$ has full support. Continuity extends the equation to time zero. There is no condition at negative times except compatibility with the global smoothness of $f$.

### Heat equation maximum principle

↑ **Parent:** [Heat equation](#heat-equation)

On a [closed manifold](smooth-manifold.md#closed-manifold) with a [Riemannian metric](riemannian-metric.md), the minimum of a smooth heat solution cannot fall below its initial minimum. At a spatial minimum, $\Delta u\le0$ for the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator). Adding a small increasing function of time and considering the first crossing gives the assertion. Applying the result to nonnegative initial functions shows that the [Riemannian heat kernel](#riemannian-heat-kernel) is nonnegative.

### Heat equation energy identity

↑ **Parent:** [Heat equation](#heat-equation)

On a [closed manifold](smooth-manifold.md#closed-manifold) with a [Riemannian metric](riemannian-metric.md), a smooth solution of $\partial_tu+\Delta u=0$ for the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) satisfies the displayed identity by [integration by parts](calculus.md#integration-by-parts). Zero initial data force the solution to vanish, proving uniqueness and the [semigroup property](functional-analysis.md#semigroup-property) for heat evolution.

### Dirichlet boundary-forcing heat-kernel formula

↑ **Parent:** [Heat equation](#heat-equation)

If $K$ is the zero-[Dirichlet heat kernel on an interval](#dirichlet-heat-kernel-on-an-interval) for $w_t=w_{xx}-cw$, [integration by parts](calculus.md#integration-by-parts) gives

$$
w(x,t)=\int_0^LK(x,y,t)w_0(y)\,dy+\int_0^t[K_y(x,0,t-s)g(s)-K_y(x,L,t-s)h(s)]\,ds.
$$

The opposite endpoint signs are essential. Nonzero boundary values are limits of the full formula; evaluating each homogeneous sine mode at the boundary prematurely loses the forcing.

#### Half-line drift boundary kernel

↑ **Parent:** [Dirichlet boundary-forcing heat-kernel formula](#dirichlet-boundary-forcing-heat-kernel-formula)

Convolution of this kernel with [Dirichlet boundary data](differential-equation.md#dirichlet-boundary-data) supplies the boundary forcing for $u_t=u_{xx}+\alpha u_x$ on $x>0$. It is $-(2\partial_x+\alpha)H(x+\alpha t,t)$. For $\alpha\ge0$, its total time mass is $e^{-\alpha x}$, tending to one as $x\downarrow0$, and its mass away from zero time tends to zero. Thus the boundary value is recovered through an [approximate identity](fourier-analysis.md#approximate-identity), not by pointwise substitution $x=0$ in the kernel.

### Dirichlet energy dissipation for the heat equation

↑ **Parent:** [Heat equation](#heat-equation)

For a real smooth solution $w_t=\Delta w$ on a bounded regular domain with $w_t=0$ on its boundary, differentiation and [Green's first identity](partial-differential-equation.md#green-s-first-identity) yield

$$
\frac d{dt}\int_V|\nabla w|^2\,dV=-2\int_V(\Delta w)^2\,dV\leq0.
$$

The boundary term is zero because the boundary values are fixed in time, not because the normal derivative vanishes. Equality at a particular time is equivalent to $\Delta w=0$ throughout the domain at that time.

### Radial heat equation in three dimensions

↑ **Parent:** [Heat equation](#heat-equation)

For a spherically symmetric field $u(r,t)$ in three dimensions,

$$
\nabla^2u=\frac1{r^2}\frac\partial{\partial r}\left(r^2u_r\right)
=\frac1r\frac{\partial^2}{\partial r^2}(ru).
$$

Thus the [heat equation](#heat-equation) becomes $u_t=D r^{-1}(ru)_{rr}$. Introducing $w=ru$ reduces its spatial part to the one-dimensional second derivative $w_{rr}$, while regularity at the centre requires $w(0,t)=0$.

#### Spherical-shell heat equation via radial rescaling

↑ **Parent:** [Radial heat equation in three dimensions](#radial-heat-equation-in-three-dimensions)

On a shell $0<r_-<r<r_+$ with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), put $L=r_+-r_-$ and $u=r\psi$. The [radial heat equation in three dimensions](#radial-heat-equation-in-three-dimensions) becomes $u_t=\kappa u_{rr}$, with zero values at both endpoints. Expanding $u(0,r)=r\psi(0,r)$ in a [Fourier sine series](fourier-series.md#fourier-sine-series) gives the displayed solution, with $b_n=(2/L)\int_{r_-}^{r_+}r\psi(0,r)\sin[n\pi(r-r_-)/L]dr$. Each radial mode decays at the square of its wave number. The positive inner radius makes division by $r$ harmless throughout the shell.

### Sinusoidally forced heat equation on a half-line

↑ **Parent:** [Heat equation](#heat-equation)

For $T_t=\kappa T_{xx}$ on $x>0$, with $T(x,0)=0$ and $T(0,t)=\sin\omega t$,

$$
\widetilde T(x,p)=\frac{\omega}{p^2+\omega^2}
\exp\left(-x\sqrt{\frac p\kappa}\right).
$$

Consequently the transform of $I(t)=\int_0^\infty T(x,t)\,dx$ is

$$
\widetilde I(p)=\frac{\omega\sqrt\kappa}
{\sqrt p\,(p^2+\omega^2)}.
$$

### Potential Burgers equation

↑ **Parent:** [Heat equation](#heat-equation)

The nonlinear equation

$$
u_t=u_{xx}+u_x^2
$$

is the potential form of the viscous Burgers equation. The substitution $w=e^u$ converts it to the [heat equation](#heat-equation) $w_t=w_{xx}$.

### Heat kernel

↑ **Parent:** [Heat equation](#heat-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heat_kernel)

For $u_t=\kappa u_{xx}$ on the real line,

$$
K_t(x)=\frac1{\sqrt{4\pi\kappa t}}e^{-x^2/(4\kappa t)}
$$

has total mass one and converges to the delta distribution as $t$ decreases to zero. The solution is $u(t)=K_t*u_0$.

#### Heat kernel trace formula

↑ **Parent:** [Heat kernel](#heat-kernel)

On a [closed manifold](smooth-manifold.md#closed-manifold), the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) has a smooth [heat kernel](#heat-kernel) and its [heat semigroup](#heat-semigroup) is a [trace-class operator](compact-operator.md#trace-class-operator) for positive time. Expanding in a smooth [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) gives $K_t(x,y)=\sum_je^{-t\lambda_j}\phi_j(x)\overline{\phi_j(y)}$. [Elliptic regularity](distribution-theory.md#elliptic-regularity) bounds each derivative of $\phi_j$ polynomially in $\lambda_j$, while the exponential dominates those powers, so the expansion converges with all derivatives. Integrating the diagonal and using the unit norm of each [eigenfunction](linear-operator-theory.md#eigenfunction) proves the formula. For a bundle operator, insert the fibre [matrix trace](linear-algebra.md#matrix-trace) inside the integral.

#### Positive diffusivity requirement for the forward heat kernel

↑ **Parent:** [Heat kernel](#heat-kernel)

The real [Gaussian function](calculus.md#gaussian-function) [heat kernel](#heat-kernel) $(4\pi\varepsilon z)^{-1/2}\exp[-(\phi-\theta)^2/(4\varepsilon z)]$ is integrable only when $\varepsilon z>0$. For forward time $z>0$, this requires positive diffusivity. A [Cole-Hopf transformation](partial-differential-equation.md#cole-hopf-transformation) is an algebraic substitution for any nonzero coefficient, but that does not make the real forward [convolution](fourier-analysis.md#convolution) valid for negative diffusivity. Constant initial heat data already produce a divergent integral with the wrong sign.

#### Heat-kernel convolution

↑ **Parent:** [Heat kernel](#heat-kernel)

For the [heat equation](#heat-equation) on $\mathbb R^n$ with diffusion coefficient one, the [heat kernel](#heat-kernel) is $K_t(x)=(4\pi t)^{-n/2}e^{-|x|^2/(4t)}$. Its [convolution](fourier-analysis.md#convolution) with bounded initial data is smooth for positive time, solves the equation by differentiation under the integral, and returns [continuous](calculus.md#continuous-function) initial data locally uniformly through the [approximate identity](fourier-analysis.md#approximate-identity) property. It is [Gaussian filtering](computer-science.md#gaussian-blur) with per-coordinate variance $2t$.

#### Riemannian heat kernel

↑ **Parent:** [Heat kernel](#heat-kernel)

For the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator), the kernel solving $(\partial_t+\Delta_x)H=0$ with initial [Dirac delta distribution](distribution-theory.md#dirac-delta-function) on the diagonal represents the [heat semigroup](#heat-semigroup). On a [closed manifold](smooth-manifold.md#closed-manifold) with a [Riemannian metric](riemannian-metric.md) it is smooth for $t>0$, symmetric, nonnegative, preserves constants, and obeys the [semigroup property](functional-analysis.md#semigroup-property).

##### Heat kernel on a finite isometric quotient

↑ **Parent:** [Riemannian heat kernel](#riemannian-heat-kernel)

For a finite free action by [Riemannian isometries](differential-geometry.md#riemannian-isometry), the [Riemannian heat kernel](#riemannian-heat-kernel) on the quotient is the image sum shown above. Integrating over a fundamental domain combines all images into the integral on the covering manifold, proving the initial condition and showing that there is no averaging factor in the kernel. The [heat trace](riemannian-geometry.md#heat-trace) does have an averaging factor $1/|U|$, because the integral of a quotient function over the cover is $|U|$ times its quotient integral. Mere freeness of a general nondiscrete group action is not enough for this covering formula.

###### Heat semigroup descent through a finite normal covering

↑ **Parent:** [Heat kernel on a finite isometric quotient](#heat-kernel-on-a-finite-isometric-quotient)

The normalized pullback is a unitary map from $L^2$ of the quotient onto the deck-invariant subspace of $L^2$ of the cover. Local isometry and the sheet-counting integration formula preserve the Dirichlet quadratic form. Therefore the [Friedrichs extension](linear-operator-theory.md#friedrichs-extension) and its [heat semigroup](#heat-semigroup) intertwine with this map. A finite sum of lifted [Riemannian heat kernels](#riemannian-heat-kernel) gives the quotient kernel; independence of lifts follows by reindexing the deck group. This formulation avoids a uniqueness claim for unrestricted heat-equation solutions on a noncompact or incomplete manifold.

##### Spectral expansion of the Riemannian heat kernel

↑ **Parent:** [Riemannian heat kernel](#riemannian-heat-kernel)

On a [closed manifold](smooth-manifold.md#closed-manifold) with a [Riemannian metric](riemannian-metric.md), an [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) for the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) gives this formula, with [eigenvalues](linear-operator-theory.md#eigenvalue) counted with multiplicity. Polynomial elliptic bounds and exponential time decay give convergence of every derivative away from time zero. The conjugate is necessary for a complex basis.

##### Heat parametrix

↑ **Parent:** [Riemannian heat kernel](#riemannian-heat-kernel)

An approximate [Riemannian heat kernel](#riemannian-heat-kernel) with the correct delta initial limit and a residual extending with enough regularity to time zero. A cutoff Gaussian times transport coefficients supplies a local construction. Increasing the expansion order, or summing the full asymptotic series smoothly, makes the residual regular enough for a [Volterra parametrix correction](#volterra-parametrix-correction).

###### Heat-kernel transport equations

↑ **Parent:** [Heat parametrix](#heat-parametrix)

In [normal coordinates](general-relativity.md#normal-coordinates) $q=\exp_p x$, write the [Riemannian volume form](riemannian-metric.md#riemannian-volume-form) as $J(p,x)\,dx$ and let $r=|x|$. With the [heat operator](#heat-operator) $\partial_t-\Delta_q$, the Gaussian times a power-series amplitude has its singular terms cancelled by the displayed radial equations for $i\geq1$. The initial coefficient is $w_0=J^{-1/2}$, and

$$
w_i(p,\exp_p x)=J(p,x)^{-1/2}\int_0^1s^{i-1}J(p,sx)^{1/2}(\Delta_qw_{i-1})(p,\exp_p(sx))\,ds.
$$

Multiplying the equation by $r^{i-1}J^{1/2}$ gives the derivative of $r^iJ^{1/2}w_i$. Smoothness forces the integration constant to vanish. The integral on a fixed compact interval proves smoothness across the diagonal by induction; it yields $w_i(p,p)=\Delta_qw_{i-1}(p,p)/i$. A truncated [heat parametrix](#heat-parametrix) therefore has residual $-g t^k\Delta_qw_k$.

###### Volterra parametrix correction

↑ **Parent:** [Heat parametrix](#heat-parametrix)

If $R=(\partial_t+\Delta_x)P$ is smooth and bounded up to time zero on a [closed manifold](smooth-manifold.md#closed-manifold), the [Volterra convolution of kernels](analysis.md#volterra-convolution-of-kernels) solves $Q+R+R*Q=0$ by $Q=\sum_{k\ge1}(-1)^kR^{*k}$. Bounds by $C^k\operatorname{vol}(M)^{k-1}t^{k-1}/(k-1)!$ prove convergence. Then $H=P+P*Q$ is the exact [Riemannian heat kernel](#riemannian-heat-kernel) and has the same initial delta limit.

#### Gaussian interval mass

↑ **Parent:** [Heat kernel](#heat-kernel)

The normalized Gaussian mass of an interval is

$$
I_\alpha(\theta,b,w)=\frac1{\sqrt{4\pi\alpha w}}\int_{-b}^{b}e^{-(\varphi-\theta)^2/(4\alpha w)}d\varphi,\qquad\alpha,w>0.
$$

It is the convolution of an interval indicator with the [heat kernel](#heat-kernel), and has an [error function](integral.md#error-function) representation. As the variance tends to zero it converges to the interval indicator away from its endpoints, with value one half at an endpoint. This is a concrete [approximate identity](fourier-analysis.md#approximate-identity).

#### Heat Poisson kernel

↑ **Parent:** [Heat kernel](#heat-kernel)

For $x>0$ and the [heat equation](#heat-equation) on a half-line, the zero-initial-data solution with prescribed [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) $g$ is $\int_0^tP(x,t-s)g(s)ds$, where

$$
P(x,t)=\frac{x}{2\sqrt\pi\,t^{3/2}}e^{-x^2/(4t)},\qquad\mathcal L_tP=e^{-x\sqrt p}.
$$

Its mass concentrates at $t=0$ as $x\downarrow0$, recovering the boundary trace.

#### Dirichlet heat kernel on an interval

↑ **Parent:** [Heat kernel](#heat-kernel)

For the [heat equation](#heat-equation) with zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) on $(0,L)$,

$$
H_L(x,y,t)=\frac2L\sum_{n\ge1}e^{-(n\pi/L)^2t}\sin(n\pi x/L)\sin(n\pi y/L).
$$

It is also obtained by the [method of images](mathematics.md#method-of-images), taking the difference between Gaussian sources at $y+2jL$ and $-y+2jL$. The [eigenfunction expansion](algebra.md#eigenfunction-expansion) is useful at long times; the image expansion is useful at short times.

##### Survival probability from an absorbing transition density

↑ **Parent:** [Dirichlet heat kernel on an interval](#dirichlet-heat-kernel-on-an-interval)

A transition density with absorbing boundaries counts the joint event of survival up to [time](classical-mechanics.md#time-in-physics) $t$ and a specified final [position](classical-mechanics.md#position). Its integrated [mass](classical-mechanics.md#mass) is [survival probability](markov-chain.md#survival-probability), not generally one. Dividing by that [mass](classical-mechanics.md#mass) gives the endpoint density conditional on survival, a different object.

###### Symmetric absorbing-interval survival probability

↑ **Parent:** [Survival probability from an absorbing transition density](#survival-probability-from-an-absorbing-transition-density)

For [diffusion](thermodynamics.md#diffusion) starting at the centre of $(-L,L)$ with absorbing endpoints, only even-parity spatial [eigenfunctions](linear-operator-theory.md#eigenfunction) contribute. Integrating their cosine expansion gives the displayed series. The leading late-time term has prefactor $4/\pi$ and decay rate $\pi^2D/(4L^2)$; its first relative correction is $-\frac13e^{-2\pi^2Dt/L^2}$.

##### Thermal trace of an interval image kernel

↑ **Parent:** [Dirichlet heat kernel on an interval](#dirichlet-heat-kernel-on-an-interval)

For a particle with mass $m$ on $(0,L)$, put $K_0(x;\beta)=\sqrt{m/(2\pi\hbar^2\beta)}e^{-mx^2/(2\hbar^2\beta)}$. The [method of images](mathematics.md#method-of-images) gives $K_D(q_f,q_i;\beta)=\sum_r[K_0(q_f-q_i+2rL;\beta)-K_0(q_f+q_i+2rL;\beta)]$. The diagonal integral is

$$
Z=L\sqrt{\frac m{2\pi\hbar^2\beta}}\sum_{r\in\mathbb Z}e^{-2mL^2r^2/(\hbar^2\beta)}-\frac12.
$$

The reflected intervals tile the real line, giving the subtraction $1/2$. The [Poisson summation formula](fourier-analysis.md#poisson-summation-formula) converts this to $\sum_{n\ge1}e^{-\beta\hbar^2\pi^2n^2/(2mL^2)}$, proving equality between the image and [energy eigenstate](energy-eigenvalue.md#energy-eigenstate) calculations.

#### Gaussian heat kernel

↑ **Parent:** [Heat kernel](#heat-kernel)

For standard [Brownian motion](brownian-motion.md) in $\mathbb R^d$, $p_t(y-x)$ is the transition density from $x$ to $y$. It is the [heat kernel](#heat-kernel) for generator $\tfrac12\Delta$. For every unit vector $e$, $\int|\partial_e p_t(x)|dx=\sqrt{2/\pi}/\sqrt t$, which bounds the change in this density under a spatial translation and proves the [Gaussian heat-kernel proof of the harmonic Liouville theorem](partial-differential-equation.md#gaussian-heat-kernel-proof-of-the-harmonic-liouville-theorem).

##### Gaussian initial data for the heat equation

↑ **Parent:** [Gaussian heat kernel](#gaussian-heat-kernel)

For $D,\gamma>0$, the displayed [function](function.md) solves the [heat equation](#heat-equation) $u_t=Du_{xx}$ and has [initial condition](differential-equation.md#initial-condition) $u(x,0)=Ae^{-\gamma(x-x_0)^2}$. Set $s=1+4\gamma Dt$. Direct [differentiation](calculus.md#differentiation) gives

$$
u_t=\left(-\frac{2\gamma D}{s}+\frac{4\gamma^2D(x-x_0)^2}{s^2}\right)u,
\qquad
u_{xx}=\left(-\frac{2\gamma}{s}+\frac{4\gamma^2(x-x_0)^2}{s^2}\right)u.
$$

These identities prove the equation. The total [integral](integral.md) is $A\sqrt{\pi/\gamma}$, independent of time. The real smooth formula is valid for $t>-1/(4\gamma D)$, including a finite interval of negative time for this particular initial profile. For nonzero $A$, its value at $x_0$ diverges as the lower time endpoint is approached. The [superposition principle](vector-space.md#superposition-principle) combines finitely many such profiles with different centers or widths.

###### Odd pair of Gaussian profiles under diffusion

↑ **Parent:** [Gaussian initial data for the heat equation](#gaussian-initial-data-for-the-heat-equation)

For $D,\gamma,a>0$, apply the [superposition principle](vector-space.md#superposition-principle) to two translated solutions for [Gaussian initial data for the heat equation](#gaussian-initial-data-for-the-heat-equation). The displayed solution of $u_t=Du_{xx}$ has [odd](calculus.md#odd-function) initial profile $A(e^{-\gamma(x-a)^2}-e^{-\gamma(x+a)^2})$. Its total spatial [integral](integral.md) is zero. For $A>0$, it is positive on $x>0$ and negative on $x<0$ at every $t\geq0$.

Writing it as $2As^{-1/2}e^{-\gamma(x^2+a^2)/s}\sinh(2\gamma ax/s)$ shows how cancellation affects its late-time shape. On the diffusive scale $x=O(\sqrt{s})$, its leading form is $4A\gamma ax s^{-3/2}e^{-\gamma x^2/s}$. Thus the two lobe maxima asymptotically lie at $x=\pm\sqrt{s/(2\gamma)}$, while their absolute heights decay as $s^{-1}$. Their centers are not fixed at the initial Gaussian centers. The first spatial moment remains $\int_{\mathbb R}xu(x,t)dx=2Aa\sqrt{\pi/\gamma}$, as follows directly from the [Gaussian integral](integral.md#gaussian-integral) and translation.

##### Newtonian potential of the Brownian heat kernel

↑ **Parent:** [Gaussian heat kernel](#gaussian-heat-kernel)

For $d\geq3$, $A_d=\Gamma(d/2-1)/(2\pi^{d/2})$. Substitute $u=|x|^2/(2s)$ to obtain the displayed identity for $x\ne0$. The [semigroup property](functional-analysis.md#semigroup-property) and [Tonelli theorem](measure-theory.md#tonelli-theorem) then give $P_t(|\cdot|^{2-d})(x)=A_d^{-1}\int_t^\infty p_s(x)ds$. The coefficient multiplying the time integral is the reciprocal of the coefficient in the full Green integral, a distinction important in [Brownian motion](brownian-motion.md) hitting asymptotics.

#### Neumann heat kernel on an interval

↑ **Parent:** [Heat kernel](#heat-kernel)

For $L>0$ and $t>0$, the [Sturm-Liouville eigenfunction expansion](sturm-liouville-theory.md#sturm-liouville-eigenfunction-expansion) for $u_t=u_{xx}$ on $(0,L)$ with homogeneous [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) gives

$$
K_N(x,y,t)=\frac1L+\frac2L\sum_{n=1}^\infty e^{-(n\pi/L)^2t}\cos\frac{n\pi x}{L}\cos\frac{n\pi y}{L}.
$$

The constant [eigenfunction](linear-operator-theory.md#eigenfunction) mode preserves the spatial [integral](integral.md). This is the $\beta=0$ limit of the [weighted Neumann heat kernel with constant drift](#weighted-neumann-heat-kernel-with-constant-drift), and its boundary inputs have the signs in the [Neumann boundary-forcing formula](#neumann-boundary-forcing-formula).

#### Heat semigroup

↑ **Parent:** [Heat kernel](#heat-kernel)

The heat semigroup acts by convolution with the heat kernel: $P_tf=K_t*f$. The identity $K_s*K_t=K_{s+t}$ gives $P_sP_t=P_{s+t}$, and its infinitesimal generator is a constant multiple of the Laplacian.

##### Spectral construction of a parabolic solution

↑ **Parent:** [Heat semigroup](#heat-semigroup)

For a time-independent strictly positive [Dirichlet realization of an elliptic operator](elliptic-boundary-value-problem.md#dirichlet-realization-of-an-elliptic-operator) and $\psi\in L^2(U)$, the [eigenfunction expansion](algebra.md#eigenfunction-expansion)

$$
u(t)=\sum_m e^{-t\lambda_m}(\psi,w_m)w_m
$$

solves $u_t+Lu=0$ with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition). For $t\geq\varepsilon>0$, every power $\lambda_m^N$ times the exponential is bounded, so the series and all its time derivatives converge in all the [Sobolev domains of powers of an elliptic Dirichlet operator](distribution-theory.md#sobolev-domains-of-powers-of-an-elliptic-dirichlet-operator). [Elliptic regularity](distribution-theory.md#elliptic-regularity) and the [Sobolev embedding theorem](sobolev-space.md#sobolev-embedding-theorem) give smoothness up to the spatial boundary for positive time. [Parseval identity](fourier-analysis.md#parseval-identity) and the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) give $u(t)\to\psi$ in $L^2$ as $t\downarrow0$.

#### Heat kernel expansion

↑ **Parent:** [Heat kernel](#heat-kernel)

A heat kernel expansion is the short-time asymptotic expansion of the trace or diagonal kernel of an elliptic operator. Its local coefficients are polynomials in background curvatures and field strengths; in quantum field theory they extract ultraviolet divergences and anomalies.

##### Heat invariants

↑ **Parent:** [Heat kernel expansion](#heat-kernel-expansion)

For the positive scalar [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) on a compact manifold without boundary, the heat invariants are the integrated coefficients $a_j=\int_Mu_j(x,x)\,dV_g$ in the short-time [heat kernel expansion](#heat-kernel-expansion). In particular $a_0=\operatorname{Vol}(M)$ and $a_1=\tfrac16\int_M R_g\,dV_g$, with $R_g$ the [scalar curvature](second-fundamental-form.md#scalar-curvature). They are determined by the [heat trace](riemannian-geometry.md#heat-trace), hence by the [spectrum](linear-operator-theory.md#spectrum-functional-analysis) with multiplicities. The leading positive coefficient recovers the dimension from $\lim_{t\downarrow0}\log\operatorname{Tr}(e^{-t\Delta})/\log(1/t)=d/2$.

###### Integrated second scalar heat coefficient

↑ **Parent:** [Heat invariants](#heat-invariants)

For the positive scalar [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) on a [closed manifold](smooth-manifold.md#closed-manifold) with a [Riemannian metric](riemannian-metric.md), the coefficient of $t^2$ in the normalized [heat trace](riemannian-geometry.md#heat-trace) is the displayed integral. The local coefficient additionally has a scalar-curvature divergence term whose integral vanishes. In dimension two, $R=2K$, $|\operatorname{Ric}|^2=2K^2$, $|\operatorname{Rm}|^2=4K^2$, giving $a_2=\frac1{15}\int_MK^2\,dA$. Together with volume and total [Gaussian curvature](second-fundamental-form.md#gaussian-curvature), it determines the variance of curvature and detects constant curvature.

###### Spectral determination of hyperbolic curvature on a surface

↑ **Parent:** [Heat invariants](#heat-invariants)

On a closed two-dimensional [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), the first three integrated scalar [heat invariants](#heat-invariants) are $A$, $\tfrac13\int K\,dA$, and $\tfrac1{15}\int K^2\,dA$, where $K$ is [Gaussian curvature](second-fundamental-form.md#gaussian-curvature). If its scalar spectrum agrees with that of a [hyperbolic surface](hyperbolic-geometry.md#hyperbolic-surface) of area $A$, these integrals are $A,-A/3,A/15$. Expanding the displayed square then forces $K=-1$ everywhere. Thus constant negative curvature is spectrally determined in this setting, although the global hyperbolic metric need not be determined up to [isometry](riemannian-geometry.md#isometry).

##### Curvature coefficient of the scalar heat kernel

↑ **Parent:** [Heat kernel expansion](#heat-kernel-expansion)

For $L=-\nabla^a\nabla_a$ on scalar functions, the leading coefficient of the [heat parametrix](#heat-parametrix) in [normal coordinates](general-relativity.md#normal-coordinates) is the inverse square root of the metric volume density: $u_0=1+R_{ab}\xi^a\xi^b/12+O(|\xi|^3)$. The [heat-kernel transport equations](#heat-kernel-transport-equations) give $u_1(x,x)=\nabla^a\nabla_a u_0(x,x)=R(x)/6$. This gives the displayed diagonal expansion. The coefficient is specific to the minimally coupled scalar operator; a bundle connection or a curvature-dependent potential changes the general Laplace-type coefficients.

##### Normal-coordinate divergence-form heat parametrix

↑ **Parent:** [Heat kernel expansion](#heat-kernel-expansion)

For $L=-\partial_j(g^{ij}\partial_i)$ in [geodesic normal coordinates](riemannian-geometry.md#geodesic-normal-coordinates), the [Gauss lemma](riemannian-geometry.md#gauss-s-lemma-riemannian-geometry) gives $g^{ij}x_i=x_j$. Substituting $F=(4\pi t)^{-n/2}e^{-|x|^2/(4t)}\sum_{k\geq0}t^kB_k$ into $(\partial_t+L)F=0$ therefore yields $(x\cdot\nabla+k)B_k=-LB_{k-1}$, with $B_0=1$. Integration along radial rays gives the displayed formula. Every coefficient is smooth at the centre. Any smooth solution of $(x\cdot\nabla+k)h=0$ is zero for $k>0$, since $s^kh(sx)$ is constant and tends to zero at $s=0$. This proves uniqueness. In this special divergence-form case $L1=0$, so every $B_k$ for $k>0$ is zero: the Gaussian itself solves the equation exactly on the coordinate ball. The [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) instead has a metric volume-density term and a nonconstant leading amplitude.

#### Gaussian approximate identity

↑ **Parent:** [Heat kernel](#heat-kernel)

The centered normal densities

$$
g_t(x)=\frac1{\sqrt{2\pi t}}e^{-x^2/(2t)}
$$

form an [approximate identity](fourier-analysis.md#approximate-identity): for every $f\in L^1(\mathbb R)$, $f*g_t\to f$ at almost every point where the [Lebesgue differentiation theorem](measure-theory.md#lebesgue-differentiation-theorem) applies. Their Fourier transforms are $e^{-t\xi^2/2}$ in the angular-frequency convention.

#### Heat-kernel solution

↑ **Parent:** [Heat kernel](#heat-kernel)

For initial data $u_0$ on the real line, Fourier transformation or convolution with the fundamental solution gives

$$
u(x,t)=\int_{-\infty}^{\infty}
\frac{e^{-(x-\xi)^2/(4Dt)}}{\sqrt{4\pi Dt}}
u_0(\xi)\,d\xi.
$$

For a [bounded function](function.md#bounded-function) $u_0$, the [convolution](fourier-analysis.md#convolution) is well defined at every positive time because the [heat kernel](#heat-kernel) has integral one. The [error-function diffusion front](integral.md#error-function-diffusion-front) uses a [Heaviside step function](integral-transform.md#heaviside-step-function) [initial condition](differential-equation.md#initial-condition) and gives one smoothed interface. The [heat equation with interval-indicator initial data](#heat-equation-with-interval-indicator-initial-data) instead has two interfaces; subtracting their two [error functions](integral.md#error-function) produces the finite-interval profile.

##### Heat-kernel convergence from a conditionally convergent Gaussian integral

↑ **Parent:** [Heat-kernel solution](#heat-kernel-solution)

Let $\varphi$ be continuous and suppose that the displayed [improper integral](real-analysis.md#improper-integral) converges separately at both infinite endpoints for some $T>0$. Absolute convergence is not required. Then its [heat-kernel solution](#heat-kernel-solution) exists, is smooth and solves the [heat equation](#heat-equation) for $0<t<T$, and tends to $\varphi(x)$ as $t\downarrow0$ at each fixed $x$.

To prove the smoothing claim, take a primitive $H$ of $\varphi(\xi)e^{-\xi^2/(4T)}$. The assumed convergence makes $H$ bounded. For $q(x,\xi,t)=K_t(x-\xi)e^{\xi^2/(4T)}$, [integration by parts](calculus.md#integration-by-parts) gives

$$
\int\varphi(\xi)K_t(x-\xi)\,d\xi=-\int H(\xi)q_\xi(x,\xi,t)\,d\xi.
$$

The endpoint term vanishes. The coefficient of $\xi^2$ in the exponent of $q$ is $-(T-t)/(4tT)<0$. Its [derivatives](calculus.md#derivative) therefore have Gaussian decay on every compact subset of $\mathbb R\times(0,T)$, justifying [differentiation under the integral sign](analysis.md#differentiation-under-the-integral-sign) in the absolutely convergent right-hand expression. Since $q_t=q_{xx}$, it satisfies the [heat equation](#heat-equation).

For the initial limit, apply the same construction to $\varphi(\xi)-\varphi(x)$ and split at $|\xi-x|=\delta$. [Continuity](calculus.md#continuous-function) controls the local part by its small oscillation times the unit kernel mass. On each remaining tail, $q$ is monotone for sufficiently small $t$: its maximum lies at $\xi=xT/(T-t)$, approaching $x$. If the relevant primitive has absolute bound $M$, [integration by parts](calculus.md#integration-by-parts) bounds that tail by $2M$ times the value of $q$ at its finite endpoint. For either endpoint $\xi=x\pm\delta$, that value tends to zero like $t^{-1/2}e^{-\delta^2/(4t)}$ times a fixed constant. Both tails vanish, proving the limit. Separate endpoint convergence matters here; merely assuming a symmetric [Cauchy principal value](complex-analysis.md#cauchy-principal-value) does not provide the bounded primitive used in this proof.

##### Heat-kernel convergence for Gaussian-integrable initial data

↑ **Parent:** [Heat-kernel solution](#heat-kernel-solution)

Suppose $\varphi$ is continuous at $x$ and, for some $T>0$,

$$
\int_{\mathbb R}|\varphi(\xi)|e^{-\xi^2/(4T)}\,d\xi<\infty.
$$

For $0<t<T$, its [convolution](fourier-analysis.md#convolution) with the [heat kernel](#heat-kernel) $K_t(s)=(4\pi t)^{-1/2}e^{-s^2/(4t)}$ is smooth and solves the [heat equation](#heat-equation). On every [compact set](topology.md#compact-space) in $\mathbb R\times(0,T)$, spatial or time [derivatives](calculus.md#derivative) of the [heat kernel](#heat-kernel) are bounded by the displayed integrable weight times a constant: their [polynomial](polynomial.md) factors are absorbed by the strictly narrower Gaussian. This justifies [differentiation under the integral sign](analysis.md#differentiation-under-the-integral-sign).

Moreover, $\int K_t=1$, so

$$
(K_t*\varphi)(x)-\varphi(x)=\int K_t(x-\xi)\bigl(\varphi(\xi)-\varphi(x)\bigr)\,d\xi.
$$

Inside $|\xi-x|<\delta$, [continuity](calculus.md#continuous-function) makes the difference uniformly small. Outside that interval, for $t\leq T/4$, the inequality $\xi^2\leq2(\xi-x)^2+2x^2$ gives

$$
K_t(x-\xi)e^{\xi^2/(4T)}
\leq\frac{e^{x^2/(2T)}}{\sqrt{4\pi t}}e^{-\delta^2/(8t)}.
$$

The right side tends to zero, proving that the weighted tail contribution vanishes; the constant term $\varphi(x)$ is controlled by the vanishing Gaussian tail mass. Thus $(K_t*\varphi)(x)\to\varphi(x)$ as $t\downarrow0$. In particular, continuous data of [polynomial growth](analysis.md#polynomial-growth) satisfy this hypothesis, even when they are unbounded. This extends the [Gaussian approximate identity](#gaussian-approximate-identity) argument beyond bounded data.

##### Heat equation with interval-indicator initial data

↑ **Parent:** [Heat-kernel solution](#heat-kernel-solution)

For $u_t=Du_{xx}$ and $u(x,0)=\mathbf1_{[-a,a]}(x)$, convolution with the [heat kernel](#heat-kernel) gives

$$
u(x,t)=\frac12\left[
\operatorname{erf}\left(\frac{x+a}{2\sqrt{Dt}}\right)
-\operatorname{erf}\left(\frac{x-a}{2\sqrt{Dt}}\right)
\right].
$$

#### Neumann heat kernel on a half-line

↑ **Parent:** [Heat kernel](#heat-kernel)

For the [heat equation](#heat-equation) $u_t=\frac12u_{xx}$ on $x>0$ with the [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) $u_x(t,0)=0$, the method of images gives

$$
K_t^N(x,y)=p_t(x-y)+p_t(x+y),
\qquad
p_t(z)=\frac1{\sqrt{2\pi t}}e^{-z^2/(2t)}.
$$

Thus $u(t,x)=\int_0^\infty K_t^N(x,y)f(y)dy$. This is also the transition kernel of [Reflected Brownian motion](brownian-motion.md#reflected-brownian-motion).

### Probabilistic representation of the heat equation with time-dependent Dirichlet data

↑ **Parent:** [Heat equation](#heat-equation)

For $u_t=\frac12u_{xx}$ on $(0,1)$ with initial data $g$ and time-dependent [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) $f_1,f_2$, stop [Brownian motion](brownian-motion.md) at its first hit of $0$ or $1$. Applying [Itô formula](stochastic-calculus.md#ito-s-lemma) to $u(t-s,B_s)$ yields

$$
u(t,x)=\mathbb E_x\!\left[g(B_t)\mathbf1_{\{t<\tau_0\wedge\tau_1\}}+f_1(t-\tau_0)\mathbf1_{\{\tau_0<t\wedge\tau_1\}}+f_2(t-\tau_1)\mathbf1_{\{\tau_1<t\wedge\tau_0\}}\right].
$$

<h3 id="duhamel-s-principle">Duhamel's principle</h3>

↑ **Parent:** [Heat equation](#heat-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Duhamel's_principle)

For a linear evolution equation with zero initial data, Duhamel's principle integrates the homogeneous propagator against the forcing time. For the forced heat equation,

$$
u(x,t)=\int_0^t\int_{-\infty}^{\infty}
K_{t-\tau}(x-\xi)f(\xi,\tau)\,d\xi\,d\tau.
$$

#### Causal diffusion from a finite-duration planar point source

↑ **Parent:** [Duhamel's principle](#duhamel-s-principle)

For the planar [heat equation](#heat-equation) with point injection of strength $p(s)$, zero initial data gives $\Psi(t,\mathbf r)=\int_0^t p(s)e^{-r^2/[4D(t-s)]}/[4\pi D(t-s)]\,ds$. If injection is $p_0$ until $t_0$ and zero later, then for $t>t_0$ this equals $p_0[\operatorname{Ei}(-b/(t-t_0))-\operatorname{Ei}(-b/t)]/(4\pi D)$, where $b=r^2/(4D)$. The [exponential integral](complex-analysis.md#exponential-integral) expansion gives $p_0\ln[t/(t-t_0)]/(4\pi D)$ when $b/(t-t_0)\ll1$.

#### Cancellation of two heat-kernel impulses

↑ **Parent:** [Duhamel's principle](#duhamel-s-principle)

On the real line, initial data $\delta(x-2\sqrt D)$ and a source $-A\delta(x+2\sqrt D)\delta(t-1)$ produce

$$
K_t(x-2\sqrt D)-AH(t-1)K_{t-1}(x+2\sqrt D).
$$

At $x=0,t=2$, the two terms cancel exactly for $A=\sqrt{e/2}$.

## Advection-diffusion equation

↑ **Parent:** [Diffusion equation](diffusion-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Advection-diffusion_equation)

The constant-coefficient one-dimensional advection-diffusion equation is

$$
u_t+a u_x=\kappa u_{xx}.
$$

Translation to coordinates moving at speed $a$ reduces it to the heat equation.

### Drift-diffusion decay time

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

For constant [diffusion coefficient](brownian-motion.md#diffusion-coefficient) $D$ and [drift velocity](electric-charge.md#drift-velocity) $v\ne0$, the balance $|v|t\sim\sqrt{Dt}$ gives the characteristic [length](physics.md#length) $D/|v|$ and [time](classical-mechanics.md#time-in-physics) $D/v^2$. The fundamental [Gaussian distribution](probability-distribution.md#normal-distribution) of the [advection-diffusion equation](#advection-diffusion-equation) has a fixed-position exponential factor $\exp[-v^2t/(4D)]$. Total [probability](probability-theory.md#probability) is still conserved: this describes [probability](probability-theory.md#probability) moving away from a fixed observation region, rather than disappearance of the [particle](physics.md#particle-physics). At zero drift, this finite exponential [time](classical-mechanics.md#time-in-physics) scale is absent.

### Homogenization of a periodic advection-diffusion equation

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

At long wavelengths and on a [diffusive time scale](#diffusive-time-scale), a rapidly varying periodic [advection-diffusion equation](#advection-diffusion-equation) can have a constant effective [diffusivity](brownian-motion.md#diffusion-coefficient). A [multiple-scale expansion](singular-perturbation.md#method-of-multiple-scales) solves periodic cell equations for the fast variables. The [solvability condition](linear-operator-theory.md#solvability-condition) at the next order gives the macroscopic equation. For a periodic sinusoidal shear this is the [effective diffusivity of a periodic sinusoidal shear](fluid-mechanics.md#effective-diffusivity-of-a-periodic-sinusoidal-shear); its transverse zero-mean cell modes decay, leaving the slow conserved concentration. This use of homogenization concerns differential equations, rather than polynomial [homogenization](projective-space.md#homogenization-algebra).

### Transported step forcing in an advection-diffusion equation

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

In coordinates $s=t$, $y=x-t$, the transport derivative $u_t+u_x$ becomes $U_s$. A [Heaviside step function](integral-transform.md#heaviside-step-function) moving at that speed becomes stationary, and its twice-integrated profile gives the displayed continuously differentiable solution of $u_t+u_x=u_{xx}+H(x-t)$. Its second spatial derivative has a jump, so the equation holds away from the moving interface and in the distributional sense there.

### Half-line advection-diffusion global relation

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

For $u_t=u_{xx}+\beta u_x$ on $x>0$, integration by parts in its half-line [Fourier transform](fourier-transform.md) gives $\widehat u_t+(k^2-i\beta k)\widehat u=-(ik+\beta)u(0,t)-u_x(0,t)$. Its time-integrated identity relates initial data and boundary values. The spectral involution $k\mapsto-k+i\beta$ preserves $\omega=k^2-i\beta k$. Evaluating the relation at both arguments eliminates the unknown Neumann transform from a Dirichlet problem; the residual unknown solution transform vanishes upon closing the upper contour for $x>0$.

### Constant-flux tracer inlet solution

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

For a [passive scalar](scalar-transport.md#passive-scalar) on a half-line, impose constant total solute flux at its inlet, with initially zero [concentration](mathematical-physics.md#concentration) and constant positive [advection](fluid-mechanics.md#advection) speed $U$ and [mass diffusivity](fluid-mechanics.md#mass-diffusivity) $\mathcal D$. A [Laplace transform](integral-transform.md#laplace-transform) in time gives

$$
\widetilde C(x,p)=\frac{2j_0}{p(U+\sqrt{U^2+4\mathcal D p})}\exp\left[\frac{U-\sqrt{U^2+4\mathcal D p}}{2\mathcal D}x\right].
$$

With $\xi=Ux/\mathcal D$, $\vartheta=U^2t/\mathcal D$ and $z_\pm=(\xi\pm\vartheta)/(2\sqrt\vartheta)$, its inverse is

$$
\frac{C(x,t)}{j_0/U}=\frac12\operatorname{erfc}(z_-)+\sqrt{\vartheta/\pi}e^{-z_-^2}-\frac12(1+\xi+\vartheta)e^\xi\operatorname{erfc}(z_+).
$$

The [complementary error function](integral.md#complementary-error-function) describes the smeared front. This is a flux boundary condition, not the [constant-concentration inlet solution](#constant-concentration-inlet-solution). At large axial [Péclet number](fluid-mechanics.md#peclet-number), both have the leading advancing front $\tfrac12\operatorname{erfc}(z_-)$.

### Constant-concentration inlet solution

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

The half-line solution of $C_t+UC_x=DC_{xx}$ with initially zero concentration, unit inlet concentration for positive time, and decay at infinity at fixed time. Both [complementary error functions](integral.md#complementary-error-function) are needed to satisfy the inlet exactly. A [Laplace transform](integral-transform.md#laplace-transform) gives $\widetilde C=p^{-1}e^{(U-\sqrt{U^2+4Dp})x/(2D)}$. A finite layer requires an additional downstream boundary condition.

### Dirichlet gauge transform for constant drift

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

For the [advection-diffusion equation](#advection-diffusion-equation) $u_t=u_{xx}+2au_x$, the multiplication $w=e^{ax}u$ gives $w_t=w_{xx}-a^2w$. A [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) remains a prescribed value, multiplied by $e^{ax}$ at the endpoint. This real exponential conjugation removes the first [derivative](calculus.md#derivative) without changing a bounded spatial interval.

#### Mixed-boundary drift-diffusion eigenmodes on a rectangle

↑ **Parent:** [Dirichlet gauge transform for constant drift](#dirichlet-gauge-transform-for-constant-drift)

For $u_t=u_{xx}+u_{yy}+\beta u_x$ on $(0,L_x)\times(0,L_y)$, impose zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) on the two vertical sides and the top, and a zero [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) at the bottom. The [Dirichlet gauge transform for constant drift](#dirichlet-gauge-transform-for-constant-drift) $u=e^{-\beta x/2}v$ gives $v_t=\Delta v-\beta^2v/4$. [Separation of variables](partial-differential-equation.md#separation-of-variables) produces the displayed modes, with $m,n\geq1$ and $\lambda_{mn}=(m\pi/L_x)^2+((n-1/2)\pi/L_y)^2+\beta^2/4$. Their spatial parts are orthogonal with weight $e^{\beta x}$; equivalently, expand $e^{\beta x/2}u_0$ in the ordinary sine-cosine basis.

#### Weighted sine transform for half-line drift diffusion

↑ **Parent:** [Dirichlet gauge transform for constant drift](#dirichlet-gauge-transform-for-constant-drift)

For $q_t=q_{xx}+\alpha q_x$, the exponential change of unknown gives $u_t=u_{xx}-\alpha^2u/4$. Its [Fourier sine transform](fourier-transform.md#fourier-sine-transform) satisfies a closed scalar evolution with a boundary forcing term. The initial transform uses $e^{\alpha x/2}q_0(x)$; ordinary integrable-transform arguments require sufficient decay of this weighted datum. For $q_0=e^{-ax}$ this requires $a>\alpha/2$. In contrast, the unweighted sine transform of $q$ couples to its cosine transform through the drift term, so it does not directly diagonalize this half-line problem.

#### Resolvent kernel for Dirichlet advection-diffusion on an interval

↑ **Parent:** [Dirichlet gauge transform for constant drift](#dirichlet-gauge-transform-for-constant-drift)

After the [Dirichlet gauge transform for constant drift](#dirichlet-gauge-transform-for-constant-drift), put $q=\sqrt{p+a^2}$. The [Dirichlet Green function](green-s-function.md#dirichlet-green-function) of $p-\partial_x^2+a^2$ is

$$
R_q(x,y)=\frac{\sinh(q\min(x,y))\sinh(q[L-\max(x,y)])}{q\sinh(qL)}.
$$

The original unweighted resolvent kernel is $e^{-ax}R_q(x,y)e^{ay}$. Its poles are $p=-a^2-(n\pi/L)^2$. The kernel is even in $q$, so the apparent square-root branch point is removable.

### Gamma impulse solution for linearly increasing diffusivity

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

On $z>0$, consider $p_t+a p_z=D(zp_z)_z$ with $a,D>0$, zero scalar flux $ap-Dzp_z$ at the endpoints for $t>0$, and unit initial impulse at the origin. Put $r=a/D$ and $\eta=z/(Dt)$. The normalized [similarity solution](partial-differential-equation.md#similarity-solution) is

$$
p(z,t)=\frac{\eta^r e^{-\eta}}{Dt\,\Gamma(1+r)}.
$$

The ansatz $p=(Dt)^{-1}f(\eta)$ gives $[\eta f'+(\eta-r)f]'=0$. Endpoint decay sets this integrated constant to zero and hence $f\propto\eta^re^{-\eta}$; the [gamma function](complex-analysis.md#gamma-function) normalizes its [integral](integral.md) to one. Its scale is $Dt$, so it converges weakly to a unit impulse as $t\downarrow0$. Its [gamma distribution](continuous-probability-distribution.md#gamma-distribution) shape is $1+r$, its maximum occurs at $z=at$, and its [expected value](expected-value.md) is $(a+D)t$. For width proportional to $z$, the associated [horizontally averaged plume concentration](scalar-transport.md#horizontally-averaged-plume-concentration) is proportional to $z^{r-1}e^{-z/(Dt)}$: its interior maximum is $(a-D)t$ when $a>D$, its supremum occurs at the origin when $a=D$, and it is singular there when $0<a<D$. The physical finite source regularizes this ideal-origin behaviour.

### Robin gauge transform for constant drift

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

Writing $u=e^{-\beta x/2}v$ transforms $u_t=u_{xx}+\beta u_x$ into $v_t=v_{xx}-\beta^2v/4$. A prescribed coordinate derivative $u_x=g$ at an endpoint becomes $v_x-(\beta/2)v=e^{\beta x/2}g$ there. Thus a [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) becomes a [Robin boundary condition](differential-equation.md#robin-boundary-condition). The signs are coordinate-derivative signs at both endpoints; outward normal derivatives require a sign change at the left endpoint.

### Weighted Neumann heat kernel with constant drift

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

On $(0,L)$, the [differential operator](analysis.md#differential-operator) $\mathcal L=\partial_x^2+\beta\partial_x=e^{-\beta x}\partial_x(e^{\beta x}\partial_x)$ with homogeneous [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) is [self-adjoint](linear-operator-theory.md#self-adjoint-operator) in the [weighted inner product](inner-product.md#weighted-inner-product) with weight $e^{\beta x}$. Its [eigenfunctions](linear-operator-theory.md#eigenfunction) and nonnegative decay rates are

$$
\phi_0=1,\quad\lambda_0=0,\qquad
\phi_k=e^{-\beta x/2}\left[\cos(q_kx)+\frac\beta{2q_k}\sin(q_kx)\right],\quad
\lambda_k=q_k^2+\frac{\beta^2}4,\quad q_k=\frac{k\pi}L.
$$

Their squared [norms](normed-vector-space.md#norm) are $N_0=(e^{\beta L}-1)/\beta$ and $N_k=L[1+\beta^2/(4q_k^2)]/2$. The [Sturm-Liouville eigenfunction expansion](sturm-liouville-theory.md#sturm-liouville-eigenfunction-expansion) gives

$$
K_\beta(x,y,t)=\sum_{k=0}^\infty\frac{e^{-\lambda_kt}\phi_k(x)\phi_k(y)}{N_k}.
$$

This kernel acts against the measure $e^{\beta y}dy$, not Lebesgue measure alone. It is symmetric in $x,y$; the transition density against Lebesgue measure is $e^{\beta y}K_\beta(x,y,t)$.

#### Resolvent kernel for Neumann advection-diffusion on an interval

↑ **Parent:** [Weighted Neumann heat kernel with constant drift](#weighted-neumann-heat-kernel-with-constant-drift)

For $L>0$, constant $\beta>0$ and $\operatorname{Re}p>0$, on $(0,L)$ put $b=\beta/2$, $\kappa=\sqrt{p+b^2}$ with the [principal square root](analysis.md#principal-square-root-of-a-complex-number), and

$$
u_p(x)=e^{-bx}\left[\cosh(\kappa x)+\frac b\kappa\sinh(\kappa x)\right],\quad
v_p(x)=e^{-b(x-L)}\left[\cosh(\kappa(L-x))-\frac b\kappa\sinh(\kappa(L-x))\right].
$$

These satisfy $(p-\partial_x^2-\beta\partial_x)u_p=(p-\partial_x^2-\beta\partial_x)v_p=0$ and the left and right homogeneous [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition), respectively. The weighted [Wronskian](linear-ordinary-differential-equation.md#wronskian) gives

$$
D_p=e^{\beta x}(u_p'v_p-u_pv_p')=e^{bL}\frac p\kappa\sinh(\kappa L),\qquad
\mathcal R_p(x,y)=\frac{u_p(\min(x,y))v_p(\max(x,y))}{D_p}.
$$

The first [derivative](calculus.md#derivative) jumps by $-e^{-\beta y}$, so the resolvent integrates against $e^{\beta y}\,dy$. Its time [Laplace transform](integral-transform.md#laplace-transform) interpretation is $\mathcal R_p=\int_0^\infty e^{-pt}K_\beta(t)dt$. The factor $p$ records the zero [eigenvalue](linear-operator-theory.md#eigenvalue) and constant stationary [eigenfunction](linear-operator-theory.md#eigenfunction).

#### Neumann boundary-forcing formula

↑ **Parent:** [Weighted Neumann heat kernel with constant drift](#weighted-neumann-heat-kernel-with-constant-drift)

For $u_t=u_{xx}+\beta u_x$ with $u_x(0,t)=g(t)$ and $u_x(L,t)=h(t)$, two applications of [integration by parts](calculus.md#integration-by-parts) against a [Neumann eigenfunction](differential-equation.md#neumann-eigenfunction) give the boundary forcing $e^{\beta L}\phi_k(L)h-\phi_k(0)g$. Solving the resulting modal [linear differential equation](differential-equation.md#linear-differential-equation) gives

$$
u(x,t)=\int_0^LK_\beta(x,y,t)e^{\beta y}u_0(y)\,dy+\int_0^t\left[e^{\beta L}K_\beta(x,L,t-s)h(s)-K_\beta(x,0,t-s)g(s)\right]ds.
$$

The endpoint [derivatives](calculus.md#derivative) are interior limits: the short-time singularity prevents evaluating each homogeneous boundary derivative before the time integral and infinite sum. The constant [eigenfunction](linear-operator-theory.md#eigenfunction) gives the weighted-mass law $\partial_t\int_0^Le^{\beta x}u\,dx=e^{\beta L}h-g$.

### Advection-diffusion heat-kernel solution

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

The Cauchy problem with initial value $u_0$ has

$$
u(t,x)=\int_{-\infty}^{\infty}K_t(x-at-y)u_0(y)\,dy.
$$

#### Half-line drift reflection kernel

↑ **Parent:** [Advection-diffusion heat-kernel solution](#advection-diffusion-heat-kernel-solution)

The homogeneous [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) kernel for $u_t=u_{xx}+\alpha u_x$ on $x>0$. Here $H(r,t)=e^{-r^2/(4t)}/\sqrt{4\pi t}$ is the [heat kernel](#heat-kernel). The exponential reflection weight makes $K_\alpha(0,y,t)=0$. Gaussian decay makes its initial-data integral convergent even when the exponentially weighted initial data are not integrable separately.

## Nonlinear diffusion equation

↑ **Parent:** [Diffusion equation](diffusion-equation.md)

A nonlinear diffusion equation lets diffusivity depend on the evolving field; the porous-medium equation is a standard example.

### Quadratic profiles for nonlinear diffusion with constant loss

↑ **Parent:** [Nonlinear diffusion equation](#nonlinear-diffusion-equation)

For the displayed [nonlinear diffusion equation](#nonlinear-diffusion-equation), a quadratic ansatz $h=A(t)+B(t)x^2$ reduces the [partial differential equation](partial-differential-equation.md) exactly to

$$
B'=6B^2,\qquad A'=2AB-1.
$$

Indeed $(hh_x)_x=2AB+6B^2x^2$, and equality of the constant and quadratic [coefficients](vector-space.md#coefficient) proves the reduction. For nonzero curvature, integration gives $B=-1/[6(t-t_0)]$. On $\tau=t-t_0>0$, the remaining [linear ordinary differential equation](linear-ordinary-differential-equation.md) is $A'+A/(3\tau)=-1$, whose [integrating factor](linear-ordinary-differential-equation.md#integrating-factor) is $\tau^{1/3}$. Thus, including spatial translation,

$$
h(x,t)=C\tau^{-1/3}-\frac{(x-x_0)^2}{6\tau}-\frac34\tau.
$$

All three constants $C,x_0,t_0$ are arbitrary, on a domain with $\tau>0$. When the quadratic coefficient vanishes, the more general affine ansatz gives $h=px+(p^2-1)t+q$.

A narrower ansatz $h=a t^{-1/3}(1-x^2/t^{2/3})-bt$ fixes two coefficients together and permits exactly $(a,b)=(1/6,3/4)$ or $(0,1)$. The zero value of $a$ is a valid spatially constant branch, not an algebraic exception to discard. These finite-parameter families are exact solutions; they are not the complete general solution of the nonlinear [partial differential equation](partial-differential-equation.md), and their sums need not be solutions.

### Logarithmic diffusion

↑ **Parent:** [Nonlinear diffusion equation](#nonlinear-diffusion-equation)

For a positive density $u$, logarithmic diffusion is the [nonlinear diffusion equation](#nonlinear-diffusion-equation) $u_t=\kappa\Delta\log u$, equivalently $u_t=\kappa\operatorname{div}(u^{-1}\nabla u)$. Its [diffusion coefficient](brownian-motion.md#diffusion-coefficient) is inversely proportional to the density. In one dimension, a mass-$M$ [self-similar solution](partial-differential-equation.md#similarity-solution) is

$$
u(x,t)=\frac{2\kappa t}{x^2+(2\pi\kappa t/M)^2}.
$$

Its integral is $M$, and substitution verifies the equation. This is $M$ times a [Cauchy distribution](probability-distribution.md#cauchy-distribution) density of scale $2\pi\kappa t/M$. It tends weakly to $M$ times the [Dirac delta distribution](distribution-theory.md#dirac-delta-function) as $t\downarrow0$; the slow algebraic tails illustrate the enhanced diffusion where density is small.

### Principal diffusion coefficients

↑ **Parent:** [Nonlinear diffusion equation](#nonlinear-diffusion-equation)

For flux $c(|\nabla u|)\nabla u$, the [derivative](calculus.md#derivative) matrix is $c(s)I+c'(s)\nabla u\otimes\nabla u/s$ with $s=|\nabla u|>0$. Its tangential and normal coefficients are $c(s)$ and $c(s)+sc'(s)$. Positivity of the scalar conductance alone therefore does not guarantee forward parabolicity.

### Perona-Malik equation

↑ **Parent:** [Nonlinear diffusion equation](#nonlinear-diffusion-equation)

The Perona-Malik equation uses decreasing diffusivity to smooth low-gradient image regions while reducing transport across edges. For $r=|\nabla u|>0$, its principal diffusion coefficients are $c(r)$ tangent to a level set and $c(r)+rc'(r)$ normal to it. A negative normal coefficient allows formal sharpening but causes forward-backward [ill-posedness](partial-differential-equation.md#ill-posed-problem). Positivity of $c$ alone is insufficient for parabolicity.

#### Forward-backward threshold for gradient-weighted exponential diffusion

↑ **Parent:** [Perona-Malik equation](#perona-malik-equation)

For one-dimensional flux $F(p)=p|p|e^{-p^2/(2\lambda^2)}$, the [nonlinear diffusion equation](#nonlinear-diffusion-equation) is $u_t=F'(u_x)u_{xx}$. The sole one-dimensional member of the [principal diffusion coefficients](#principal-diffusion-coefficients) is positive for $0<|u_x|<\sqrt2\lambda$, negative above $\sqrt2\lambda$, and zero at the two endpoints. Negative diffusion gives formal sharpening with [ill-posedness](partial-differential-equation.md#ill-posed-problem) through high-frequency growth. The extra factor $|p|$ matters: the unweighted exponential conductance has threshold $\lambda$ instead.

#### Regularized Perona-Malik diffusion

↑ **Parent:** [Perona-Malik equation](#perona-malik-equation)

Computing conductance from a smoothed [gradient](multivariable-calculus.md#gradient) gives $u_t=\operatorname{div}(c(|\nabla(G_\sigma*u)|)\nabla u)$. The [image edge](computer-science.md#image-edge) detector is nonlocal, while the local highest-order diffusion has positive coefficient when conductance is positive. A smooth kernel, lower conductance bound and appropriate regularity/boundary hypotheses support a well-posed regularized filter.

### Two-dimensional Barenblatt solution with diffusivity proportional to concentration

↑ **Parent:** [Nonlinear diffusion equation](#nonlinear-diffusion-equation)

For $C_t=k\nabla\cdot(C\nabla C)$ with total mass $2\pi M$,

$$
C(r,t)=\sqrt{\frac{M}{kt}}
\left(\frac1{\sqrt2}-\frac18\frac{r^2}{\sqrt{Mkt}}\right)_+.
$$

Its compact support has radius $r_0(t)=(32Mkt)^{1/4}$.

#### Linear-reaction time change for quadratic nonlinear diffusion

↑ **Parent:** [Two-dimensional Barenblatt solution with diffusivity proportional to concentration](#two-dimensional-barenblatt-solution-with-diffusivity-proportional-to-concentration)

The substitution

$$
C(x,t)=e^{at}G(x,\tau(t)),
\qquad
\tau(t)=
\begin{cases}
(e^{at}-1)/a,&a\ne0,\\
t,&a=0,
\end{cases}
$$

reduces $C_t=k\nabla\cdot(C\nabla C)+aC$ to  
$G_\tau=k\nabla\cdot(G\nabla G)$.

<h2 id="reaction-diffusion-system">Reaction–diffusion system</h2>

↑ **Parent:** [Diffusion equation](diffusion-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reaction–diffusion_system)

A reaction-diffusion system combines local reaction kinetics with spatial diffusion,

$$
u_t=D\Delta u+f(u).
$$

### Cubic fast-slow reaction-diffusion model

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

This nondimensional two-variable [reaction–diffusion system](#reaction-diffusion-system) combines a fast cubic local response with slow negative feedback. With $D>0$, $0<\alpha<1$, $\beta>0$ and $\varepsilon\ll1$, its spatially uniform rest state at $I=0$ is linearly stable: the Jacobian has [trace](linear-algebra.md#matrix-trace) $-\alpha-\varepsilon\beta$ and [determinant](multilinear-algebra.md#determinant) $\varepsilon(1+\alpha\beta)$. For suitable parameters a finite perturbation can nevertheless cause a large excursion followed by recovery. Frozen recovery gives a [bistable cubic reaction-diffusion equation](#bistable-cubic-reaction-diffusion-equation); the full coupled travelling-wave boundary-value problem determines whether front pairs form a pulse. This is a generic excitable-medium formulation of the [FitzHugh-Nagumo model](mathematical-biology.md#fitzhugh-nagumo-model), without assigning any biological variable or application.

### Diffusion-driven stationary instability

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

For reaction Jacobian $J=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ with $\operatorname{tr}J<0$ and $\det J>0$, a Fourier mode evolves under $J-q^2\operatorname{diag}(D_u,D_v)$. Its determinant is $D_uD_vq^4-(D_va+D_ud)q^2+\det J$. A finite unstable band requires $D_va+D_ud>0$ and $(D_va+D_ud)^2>4D_uD_v\det J$, with an allowed domain mode in that band.

#### Finite-domain selection of a reaction-diffusion instability

↑ **Parent:** [Diffusion-driven stationary instability](#diffusion-driven-stationary-instability)

#### Equal diffusion cannot destabilize a stable reaction Jacobian

↑ **Parent:** [Diffusion-driven stationary instability](#diffusion-driven-stationary-instability)

If both [diffusion](thermodynamics.md#diffusion) coefficients equal $D$, each spatial mode has matrix $J-Dq^2I$. Its eigenvalues are those of $J$ shifted by the negative real number $Dq^2$. Thus a reaction-stable homogeneous state remains stable under this equal-[diffusion](thermodynamics.md#diffusion) linear mechanism.

### Removing a variable scalar reaction rate by an integrating factor

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

For $u_t=u_{xx}-a(t)u$, the displayed substitution converts the equation exactly into the [heat equation](#heat-equation) $v_t=v_{xx}$. The scalar prefactor preserves homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition). Consequently each spatial [eigenfunction](linear-operator-theory.md#eigenfunction) $X_n$ with $X_n''=-\lambda_nX_n$ acquires temporal factor $\exp[-\lambda_nt-\int_0^ta(s)ds]$. The same algebra works with an evolution variable named $y$; calling that variable spatial does not alter the [separation of variables](partial-differential-equation.md#separation-of-variables). For $a(t)=1+\sin t$, the prefactor normalized to one at zero is $e^{-t+\cos t-1}$.

### Positivity of the first Dirichlet reaction-diffusion coefficient

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

For nonnegative nonzero integrable initial data $f$ on $(0,L)$, the first coefficient in the normalized [Fourier sine series](fourier-series.md#fourier-sine-series) is strictly positive, because the first sine [eigenfunction](linear-operator-theory.md#eigenfunction) is positive throughout the interval. For $\rho_t=D\rho_{xx}+\gamma\rho$ with zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), the first decay rate is $\lambda_1=D\pi^2/L^2-\gamma$. Every higher rate exceeds it by $D\pi^2(n^2-1)/L^2$, so smoothing for positive time and the spectral gap imply $e^{\lambda_1t}\rho(x,t)\to a_1\sqrt{2/L}\sin(\pi x/L)$ uniformly. Thus all interior points share the growth/decay threshold $\gamma=D\pi^2/L^2$; the endpoints remain zero. At equality the limiting profile is nonzero and stationary.

### Dirichlet reaction-diffusion growth threshold in a cuboid

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

For $n_t=\mu\Delta n+\gamma n$ in a rectangular box with zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), [separation of variables](partial-differential-equation.md#separation-of-variables) gives spatial [eigenfunctions](linear-operator-theory.md#eigenfunction) $\sin(p\pi x/L_x)\sin(q\pi y/L_y)\sin(r\pi z/L_z)$ and temporal rates $\gamma-\mu\pi^2(p^2/L_x^2+q^2/L_y^2+r^2/L_z^2)$. The largest rate is the displayed one. Every nonzero nonnegative initial density has positive projection onto this first [eigenfunction](linear-operator-theory.md#eigenfunction), so its sign determines eventual exponential growth or decay; equality leaves a stationary first mode. At fixed volume, write $a_j=L_j^{-2}$: their product is fixed, and the [arithmetic-geometric mean inequality](mathematical-optimization.md#arithmetic-geometric-mean-inequality) minimizes their sum when all three are equal. Thus the cube maximizes the growth rate among rectangular boxes of fixed volume; making a box sufficiently thin suppresses growth.

### Bistable cubic reaction-diffusion equation

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

The scalar equation $u_t=Du_{xx}+u(1-u)(u-r)$ with $D>0$ and $0<r<1$ has two stable homogeneous phases $u=0,1$ and an unstable intervening equilibrium $u=r$. Indeed the reaction derivatives at these three equilibria are $-r$, $-(1-r)$ and $r(1-r)$, respectively. A [travelling wave](analysis.md#travelling-wave) can connect the two stable phases. At the equal-depth value $r=1/2$, its decreasing [heteroclinic orbit](dynamical-systems.md#heteroclinic-orbit) is stationary. Away from this value the phases have unequal potential depths and the front propagates.

#### Logistic front of a bistable cubic equation

↑ **Parent:** [Bistable cubic reaction-diffusion equation](#bistable-cubic-reaction-diffusion-equation)

For the decreasing front connecting $1$ to $0$, the balanced stationary [travelling-wave reduction of a reaction-diffusion system](analysis.md#travelling-wave-reduction-of-a-reaction-diffusion-system) has first integral $DU_x^2/2-U^2(1-U)^2/4=0$. Choosing the negative derivative gives $U_x=-U(1-U)/\sqrt{2D}$ and hence $U=[1+e^{(x-q)/\sqrt{2D}}]^{-1}$. This logistic profile remains an exact [travelling wave](analysis.md#travelling-wave) when the reaction parameter differs from $1/2$: using $z=(x-ct-q_0)/\sqrt D$, its derivative is $U_z=-U(1-U)/\sqrt2$, and the wave equation is satisfied for $c=\sqrt{D/2}(1-2r)$. Thus the speed changes with the potential bias while the shape, apart from [translation](geometry-and-topology.md#translation-geometry), does not.

### Basally forced quadratic activator-inhibitor model

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

A quadratic [activator](#activator-in-a-reaction-diffusion-system) can have both basal production and activation inhibited by a second species. A normalized example has reaction rates $f(u,v)=1+ru^2/v-u$ and $g(u,v)=q(u^2-v)$, with $r,q>0$ and positive concentrations. At its [spatially homogeneous equilibrium](#spatially-homogeneous-equilibrium), $v=u^2$, so $u_*=1+r$ and $v_*=(1+r)^2$. Writing $a=(r-1)/(r+1)$, its reaction [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) is $J=\begin{pmatrix}a&-r/(1+r)^2\\2q(1+r)&-q\end{pmatrix}$. Thus $\operatorname{tr}J=a-q$ and $\det J=q>0$, giving linear [asymptotic stability](dynamical-systems.md#asymptotic-stability) when $q>a$ and instability when $q<a$. Basal production makes $a$ change sign at $r=1$; a positive activation feedback needed for a conventional [Turing instability](#turing-instability) requires $r>1$.

#### Weak focus at the Hopf threshold of a basal activator-inhibitor model

↑ **Parent:** [Basally forced quadratic activator-inhibitor model](#basally-forced-quadratic-activator-inhibitor-model)

At $q=a=(r-1)/(r+1)>0$, the reaction [eigenvalues](linear-operator-theory.md#eigenvalue) are $\pm i\sqrt a$. This linear marginal case is a weakly attracting focus, not a nonlinear center. To check it directly, put $u=(1+r)(1+x)$, $v=(1+r)^2(1+y)$, $h=(1+a)/2$, $\beta=(1-a)/2$, $\omega=\sqrt a$, and $X=x$, $Y=(hy-a x)/\omega$. The equations become $\dot X=-\omega Y+F_2+F_3+O(4)$, $\dot Y=\omega X+G_2+G_3+O(4)$, with

$$
F_2=(\beta X-\omega Y)^2/h,\quad F_3=-(aX+\omega Y)(\beta X-\omega Y)^2/h^2,\quad G_2=\omega(hX^2-F_2),\quad G_3=-\omega F_3.
$$

On the [unit circle](complex-analysis.md#complex-unit-circle) write $A=\cos\theta F_2+\sin\theta G_2$, $B=\cos\theta F_3+\sin\theta G_3$, $C=\cos\theta G_2-\sin\theta F_2$. In [polar coordinates](multivariable-calculus.md#polar-coordinates), $d\varrho/d\theta=(A/\omega)\varrho^2+(B/\omega-AC/\omega^2)\varrho^3+O(\varrho^4)$. The quadratic angular average vanishes. Integrating the quadratic correction over a whole cycle contributes its final squared integral, also zero, leaving the cubic average. Using the even trigonometric moments gives $\langle B\rangle=a/4$ and $\langle AC\rangle/\omega=(a+1)/8$. The [Poincaré map](dynamical-systems.md#poincare-map) is therefore $\varrho\mapsto\varrho+[2\pi/\omega](a-1)\varrho^3/8+O(\varrho^4)$. Since $0<a<1$, it contracts sufficiently small positive radii and proves nonlinear [asymptotic stability](dynamical-systems.md#asymptotic-stability) at the threshold.

#### Turing threshold of a basally forced quadratic activator-inhibitor model

↑ **Parent:** [Basally forced quadratic activator-inhibitor model](#basally-forced-quadratic-activator-inhibitor-model)

Add diffusivities $1,p$ to the [basally forced quadratic activator-inhibitor model](#basally-forced-quadratic-activator-inhibitor-model). A [Fourier mode](fourier-analysis.md#fourier-mode) with $s=k^2$ has matrix $J-s\operatorname{diag}(1,p)$ and [determinant](multilinear-algebra.md#determinant) $D(s)=ps^2+(q-pa)s+q$. When $q>a$, its [trace](linear-algebra.md#matrix-trace) is negative for every $s\geq0$. A positive-growth mode therefore occurs precisely when $D(s)<0$ for some positive $s$. The parabola has a positive minimizer only if $pa>q$, and its minimum is negative exactly when $(pa-q)^2>4pq$. Thus the ordinary [Turing instability](#turing-instability) requires $a>0$, $q>a$ and $p>q/(\sqrt{1+a}-1)^2$. At onset, $k_c^2=(pa-q)/(2p)=\sqrt{q/p}$ and the critical [wavelength](wave-equation.md#wavelength) is $2\pi(p/q)^{1/4}$. A bounded spatial domain further requires an allowed mode inside the unstable band.

### Inhibitor in a reaction-diffusion system

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

An inhibitor in an activator-inhibitor [reaction–diffusion system](#reaction-diffusion-system) suppresses the [activator](#activator-in-a-reaction-diffusion-system). Its diffusion and reaction feedback can stabilize a spatially uniform state while allowing some nonzero [wavenumbers](wave-equation.md#wavenumber) to grow through a [Turing instability](#turing-instability).

### Activator in a reaction-diffusion system

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

An activator in an activator-inhibitor [reaction–diffusion system](#reaction-diffusion-system) is a species whose local feedback enhances activation. Near a homogeneous equilibrium, positive self-feedback is reflected in the corresponding diagonal entry of the reaction [Jacobian matrix](multivariable-calculus.md#jacobian-matrix). Cross-coupling to an [inhibitor](#inhibitor-in-a-reaction-diffusion-system) and differing diffusion rates can generate a [Turing instability](#turing-instability).

### Quadratic activator-inhibitor model

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

For positive concentrations and positive parameters, this [reaction–diffusion system](#reaction-diffusion-system) has homogeneous equilibrium $(u_*,v_*)=(1/b,1/b^2)$ and reaction [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) $\begin{pmatrix}b&-b^2\\2/b&-1\end{pmatrix}$. Its trace is $b-1$ and determinant is $b$, making the equilibrium reaction-stable exactly when $0<b<1$. Stable complex eigenvalues permit damped oscillations, which must be distinguished from sustained periodic oscillations.

#### Turing threshold of the quadratic activator-inhibitor model

↑ **Parent:** [Quadratic activator-inhibitor model](#quadratic-activator-inhibitor-model)

A mode with squared [wavenumber](wave-equation.md#wavenumber) $q$ in the [quadratic activator-inhibitor model](#quadratic-activator-inhibitor-model) has negative trace $b-1-(1+d)q$ when $0<b<1$. Its determinant is $D(q)=dq^2+(1-db)q+b$. A positive minimum location and a negative minimum require $db>1$ and $(db-1)^2>4db$, equivalent to $db>3+2\sqrt2$. At onset, the double determinant root is $q_c=(1+\sqrt2)/d$. In a bounded domain an admissible nonzero spatial mode must additionally lie in the open negative-determinant band.

#### Positive-quadrant Dulac multiplier for quadratic activation

↑ **Parent:** [Quadratic activator-inhibitor model](#quadratic-activator-inhibitor-model)

For the diffusionless [quadratic activator-inhibitor model](#quadratic-activator-inhibitor-model), choose the [Dulac function](dynamical-systems.md#dulac-function) $u^{-2}$. Then $u^{-2}f=1/v-b/u$ and $u^{-2}g=1-v/u^2$, giving divergence $(b-1)/u^2$. For $0<b<1$ it is strictly negative throughout the simply connected positive quadrant. [Green's theorem](multivariable-calculus.md#green-theorem) rules out a periodic orbit: its boundary flux would be zero because the rescaled vector field is tangent to the orbit, while its interior divergence integral would be negative.

### Spatially homogeneous equilibrium

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

A spatially homogeneous equilibrium of a [reaction–diffusion system](#reaction-diffusion-system) is a constant state $u_*$ satisfying $f(u_*)=0$. Since its spatial derivatives vanish, its stability to homogeneous perturbations is determined by the [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) $Df(u_*)$; diffusion can additionally destabilize nonconstant modes.

### Morphogen reaction-diffusion equation

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

A morphogen reaction-diffusion equation models a spatial concentration by diffusion and local production or decay. Linearization at a homogeneous equilibrium $C=0$ replaces $f(C)$ by $f'(0)C$.

It is a transport-and-reaction model for a [morphogen](biology.md#morphogen), rather than the identity of the signaling molecule concept.

#### Mixed Dirichlet-Neumann modes on an interval

↑ **Parent:** [Morphogen reaction-diffusion equation](#morphogen-reaction-diffusion-equation)

The eigenfunctions satisfying $X(0)=0$ and $X'(L)=0$ are

$$
X_n(x)=\sin(k_nx),
\qquad
k_n=\frac{(n+1/2)\pi}{L},\quad n\geq0.
$$

##### Critical length for a linearly growing morphogen

↑ **Parent:** [Mixed Dirichlet-Neumann modes on an interval](#mixed-dirichlet-neumann-modes-on-an-interval)

For $C_t=DC_{xx}+aC$ with $a>0$, $C(0,t)=0$, and $C_x(L,t)=0$, every mode decays exactly when

$$
L<\frac\pi2\sqrt{\frac Da}.
$$

### Fast-inhibitor elimination in a reaction-diffusion system

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

If a fast inhibitor satisfies $0=v_{xx}+u-v$, then its spatial [Fourier transform](fourier-transform.md) obeys

$$
\widehat v(k)=\frac{\widehat u(k)}{1+k^2}.
$$

Substitution produces a nonlocal scalar equation for the activator.

#### Dispersion relation after fast-inhibitor elimination

↑ **Parent:** [Fast-inhibitor elimination in a reaction-diffusion system](#fast-inhibitor-elimination-in-a-reaction-diffusion-system)

For activator diffusion $D$, local linear decay $r$, and coupling $\rho(u-v)$, eliminating the fast inhibitor gives

$$
\sigma(k)=-Dk^2-r+\rho\frac{k^2}{1+k^2}.
$$

Its pattern-forming threshold is

$$
\rho_c=(\sqrt r+\sqrt D)^2,
\qquad
k_c=(r/D)^{1/4}.
$$

### Turing pattern

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Turing_pattern)

A [Turing pattern](#turing-pattern) is a spatially structured state produced by interactions between local reactions and diffusion. A [Turing instability](#turing-instability) explains linear pattern onset when a homogeneous equilibrium is stable without diffusion but unstable to a nonzero spatial mode.

#### Turing instability

↑ **Parent:** [Turing pattern](#turing-pattern)

A Turing, or diffusion-driven, instability occurs when a spatially homogeneous equilibrium is stable to homogeneous perturbations but unstable to a nonzero spatial Fourier mode after unequal diffusion is introduced.

##### Fast-inhibitor cubic activator growth rate

↑ **Parent:** [Turing instability](#turing-instability)

For $u_t=Du_{xx}-u(u-r)(u-1)-\rho(v-u)$ and $0=v_{xx}-v+u$, a [Fourier mode](fourier-analysis.md#fourier-mode) perturbation about zero has $v=u/(1+k^2)$ and [growth rate](dispersion-relation.md#growth-rate) $\sigma(k)=-r-Dk^2+\rho k^2/(1+k^2)$. If $\rho>D$, its maximum is $-r+(\sqrt\rho-\sqrt D)^2$ at $k^2=\sqrt{\rho/D}-1$; if $\rho\leq D$, its maximum is $-r$ at zero. Replacing $(u,v,r)$ by $(1-u,1-v,1-r)$ gives the corresponding criterion at the other homogeneous equilibrium.

##### Two-species diffusion-driven instability criterion

↑ **Parent:** [Turing instability](#turing-instability)

Let a stable two-species reaction equilibrium have Jacobian

$$
J=\begin{pmatrix}a&b\\c&d\end{pmatrix},
\qquad \operatorname{tr}J<0,
\qquad \det J>0,
$$

and diffusion matrix $\operatorname{diag}(D_u,D_v)$. A mode with $q=k^2$ has determinant

$$
\det(J-qD)=\det J-(D_va+D_ud)q+D_uD_vq^2.
$$

Since its trace decreases with $q$, diffusion-driven instability occurs exactly when

$$
D_va+D_ud>0,
\qquad
(D_va+D_ud)^2>4D_uD_v\det J.
$$

###### Impossibility of a two-species Turing instability at equal diffusivities

↑ **Parent:** [Two-species diffusion-driven instability criterion](#two-species-diffusion-driven-instability-criterion)

When $D_u=D_v=D$, every spatial Fourier mode replaces the reaction Jacobian $J$ by $J-Dk^2I$. Each eigenvalue is shifted left by $Dk^2$, so diffusion cannot destabilize a stable homogeneous equilibrium.

###### Near-unity diffusivity ratio for a Turing instability

↑ **Parent:** [Two-species diffusion-driven instability criterion](#two-species-diffusion-driven-instability-criterion)

For reaction Jacobian

$$
\begin{pmatrix}-1&-1\\1+\delta&1-\delta\end{pmatrix},
$$

the critical diffusivity ratio is

$$
d_c=
\left(
\frac{\sqrt{2\delta}+\sqrt{1+\delta}}{1-\delta}
\right)^2
=1+2\sqrt{2\delta}+O(\delta).
$$

It approaches one as the stable reaction system approaches marginality.

### Brusselator

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brusselator)

The Brusselator is a two-species autocatalytic reaction model. In the parametrization

$$
f(u,v)=\alpha-(\beta+1)u+u^2v,
\qquad
g(u,v)=\beta u-u^2v,
$$

its positive homogeneous equilibrium is $(u_*,v_*)=(\alpha,\beta/\alpha)$.

#### Hopf coefficient of the Brusselator

↑ **Parent:** [Brusselator](#brusselator)

For $u'=1-(b+1)u+au^2v$, $v'=bu-au^2v$, the equilibrium $(1,b/a)$ has a [Hopf bifurcation](bifurcation-theory.md#hopf-bifurcation) at $b=1+a$. Coordinates $x=u-1$, $y=-\sqrt a[(u-1)+(v-b/a)]$ give the threshold equations $x'=-\sqrt a\,y+(1-a)x^2-2\sqrt a\,xy-ax^3-\sqrt a\,x^2y$, $y'=\sqrt a\,x$. In the usual planar radial normalization the cubic coefficient is $-(a+2)/8<0$, proving a nondegenerate supercritical bifurcation. The leading small-amplitude angular frequency is $\sqrt a$.

#### Brusselator trapping region

↑ **Parent:** [Brusselator](#brusselator)

For the spatially homogeneous Brusselator with parameters $r,s>0$, set $\alpha=r/(1+s)$. The quadrilateral

$$
\alpha\leq x,\qquad
0\leq y\leq\frac s\alpha,\qquad
x+y\leq r+\frac s\alpha
$$

is a [trapping region](dynamical-systems.md#trapping-region). The four inward-pointing tests use $\dot x\geq0$ on $x=\alpha$, $\dot y\geq0$ on $y=0$, $\dot y\leq0$ on $y=s/\alpha$, and $\dot x+\dot y=r-x\leq0$ on the sloping edge.

#### Brusselator periodic-orbit criterion

↑ **Parent:** [Brusselator](#brusselator)

The spatially homogeneous Brusselator has its unique positive equilibrium at $(r,s/r)$. Its Jacobian there has determinant $r^2$ and trace $s-1-r^2$. If $s-1>r^2$, the equilibrium is a repeller inside the [Brusselator trapping region](#brusselator-trapping-region); the [Poincaré-Bendixson theorem](dynamical-systems.md#poincare-bendixson-theorem) then supplies a periodic orbit.

#### Turing threshold of the Brusselator

↑ **Parent:** [Brusselator](#brusselator)

When $u$ and $v$ have diffusivities $D$ and $1$, respectively, and the homogeneous Brusselator equilibrium is stable, a [Turing instability](#turing-instability) occurs precisely when

$$
\beta>(1+\alpha\sqrt D)^2.
$$

At onset,

$$
D_c=\frac{(\sqrt\beta-1)^2}{\alpha^2},
\qquad
k_*^2=\frac{\alpha^2}{\sqrt\beta-1}.
$$

##### Discrete-mode Turing threshold for the Brusselator

↑ **Parent:** [Turing threshold of the Brusselator](#turing-threshold-of-the-brusselator)

On a specified finite domain, only its boundary-compatible wavenumbers can grow. Solve the [Brusselator](#brusselator) mode determinant for its neutral value of $b$ and minimize over those nonzero modes. Minimizing over all continuous $k$ instead gives the usual threshold and $k_c^2=a/\sqrt{D_uD_v}$. The finite-mode minimum must still precede the homogeneous threshold to describe a [Turing instability](#turing-instability).

##### Brusselator Turing-before-Hopf diffusivity condition

↑ **Parent:** [Turing threshold of the Brusselator](#turing-threshold-of-the-brusselator)

For the [Brusselator](#brusselator), the stationary spatial threshold is $b_T=(1+a\sqrt{D_u/D_v})^2$ and the homogeneous oscillatory threshold is $b_H=1+a^2$. A genuine [Turing instability](#turing-instability) appears first only if $b_T<b_H$, which rearranges to the displayed diffusivity-ratio bound. Equality gives simultaneous stationary spatial and homogeneous oscillatory neutral modes. Otherwise homogeneous loss of stability occurs first.

## ↑ Ancestors (5)

1. [Partial differential equation](partial-differential-equation.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (70)

- [Complex Ginzburg–Landau equation](partial-differential-equation.md#complex-ginzburg-landau-equation)
- [Constant-reservoir diffusion-controlled particle growth](critical-phenomenon.md#constant-reservoir-diffusion-controlled-particle-growth)
- [Diffusion](thermodynamics.md#diffusion)
- [Diffusion-controlled solute gravity current](reduced-gravity.md#diffusion-controlled-solute-gravity-current)
- [Diffusion image processing](computer-science.md#diffusion-image-processing)
- [Diffusive flux](mathematical-physics.md#diffusive-flux)
- [Diffusive time scale](#diffusive-time-scale)
- [Drift-diffusion equation with a potential](#drift-diffusion-equation-with-a-potential)
- [Ekman spin-down in a shallow-water layer](geophysical-fluid-dynamics.md#ekman-spin-down-in-a-shallow-water-layer)
- [Error-function diffusion front](integral.md#error-function-diffusion-front)
- [Fick's laws](mathematical-physics.md#fick-s-laws)
- [Fundamental diffusion mode](#fundamental-diffusion-mode)
- [Gaussian integral](integral.md#gaussian-integral)
- [Gershgorin stability bound for a variable-coefficient diffusion stencil](numerical-analysis.md#gershgorin-stability-bound-for-a-variable-coefficient-diffusion-stencil)
- [Initial corner compatibility for a Dirichlet heat problem](differential-equation.md#initial-corner-compatibility-for-a-dirichlet-heat-problem)
- [Isothermal diffusion with position-dependent drag](stochastic-calculus.md#isothermal-diffusion-with-position-dependent-drag)
- [Keplerian viscous diffusion equation](astrophysical-disk.md#keplerian-viscous-diffusion-equation)
- [Kinematic viscosity](dynamic-viscosity.md#kinematic-viscosity)
- [Molecular diffusion](thermodynamics.md#molecular-diffusion)
- [Momentum diffusion](dynamic-viscosity.md#momentum-diffusion)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2.md#7/c/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2.md#7/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-55.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3.md#12d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-73.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-71.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-71.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3.md#15b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-318.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-321.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-321.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-321.md#1/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-321.md#1/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-331.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-332.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4.md#17b/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4.md#17b/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-331.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-331.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-332.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3.md#41e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#13b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3.md#16a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-3.md#16c/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-329.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-332.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-332.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2.md#section-b/10/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-2.md#14/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2.md#20/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2.md#20/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2.md#1/a/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-c/c12/diffusion-with-a-heat-source/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2007.md#section-a/a2/d/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2018.md#3/c/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2018.md#3/d/solution)
- [Robin diffusion with a growing mode](#robin-diffusion-with-a-growing-mode)
- [Saline Stefan problem](geophysics.md#saline-stefan-problem)
- [Scalar integrating factor for a reaction-diffusion equation](#scalar-integrating-factor-for-a-reaction-diffusion-equation)
- [Scalar transport](scalar-transport.md)
- [Scalar variance](scalar-transport.md#scalar-variance)
- [Solutal diffusivity](brownian-motion.md#solutal-diffusivity)
- [Squared diffusion-residual action](#squared-diffusion-residual-action)
- [Thermal diffusion wave](heat.md#thermal-diffusion-wave)
- [Time reversal of the squared diffusion-residual action](#time-reversal-of-the-squared-diffusion-residual-action)
- [Variable-coefficient conservative diffusion equation](#variable-coefficient-conservative-diffusion-equation)
