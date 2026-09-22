# Diffusion equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diffusion_equation)

A diffusion equation describes smoothing caused by a flux down spatial gradients.

**Table of contents**

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
  - [Reaction-diffusion spectral decay threshold](#reaction-diffusion-spectral-decay-threshold)
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
      - [Thermal trace of an interval image kernel](#thermal-trace-of-an-interval-image-kernel)
    - [Gaussian heat kernel](#gaussian-heat-kernel)
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
      - [Heat equation with interval-indicator initial data](#heat-equation-with-interval-indicator-initial-data)
    - [Neumann heat kernel on a half-line](#neumann-heat-kernel-on-a-half-line)
  - [Probabilistic representation of the heat equation with time-dependent Dirichlet data](#probabilistic-representation-of-the-heat-equation-with-time-dependent-dirichlet-data)
  - [Duhamel's principle](#duhamel-s-principle)
    - [Causal diffusion from a finite-duration planar point source](#causal-diffusion-from-a-finite-duration-planar-point-source)
    - [Cancellation of two heat-kernel impulses](#cancellation-of-two-heat-kernel-impulses)
- [Advection-diffusion equation](#advection-diffusion-equation)
  - [Homogenization of a periodic advection-diffusion equation](#homogenization-of-a-periodic-advection-diffusion-equation)
  - [Transported step forcing in an advection-diffusion equation](#transported-step-forcing-in-an-advection-diffusion-equation)
  - [Half-line advection-diffusion global relation](#half-line-advection-diffusion-global-relation)
  - [Constant-flux tracer inlet solution](#constant-flux-tracer-inlet-solution)
  - [Constant-concentration inlet solution](#constant-concentration-inlet-solution)
  - [Dirichlet gauge transform for constant drift](#dirichlet-gauge-transform-for-constant-drift)
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
  - [Logarithmic diffusion](#logarithmic-diffusion)
  - [Principal diffusion coefficients](#principal-diffusion-coefficients)
  - [Perona-Malik equation](#perona-malik-equation)
    - [Forward-backward threshold for gradient-weighted exponential diffusion](#forward-backward-threshold-for-gradient-weighted-exponential-diffusion)
    - [Regularized Perona-Malik diffusion](#regularized-perona-malik-diffusion)
  - [Two-dimensional Barenblatt solution with diffusivity proportional to concentration](#two-dimensional-barenblatt-solution-with-diffusivity-proportional-to-concentration)
    - [Linear-reaction time change for quadratic nonlinear diffusion](#linear-reaction-time-change-for-quadratic-nonlinear-diffusion)
- [Reaction–diffusion system](#reaction-diffusion-system)
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

## Diffusive time scale

↑ **Parent:** [Diffusion equation](diffusion-equation.md)

A concentration varying over length $L$ has Laplacian of order its amplitude divided by $L^2$. Balancing the time derivative with $\kappa\Delta\chi$ in the [diffusion equation](diffusion-equation.md) gives the displayed relaxation time. A [multiple-scale expansion](differential-equation.md#method-of-multiple-scales) with spatial scale $\varepsilon x$ therefore uses slow time $\varepsilon^2t$ when the effective [diffusivity](brownian-motion.md#diffusion-coefficient) is of order one.

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

Consider a [nonlinear diffusion equation](#nonlinear-diffusion-equation) with uniform supply, $\phi h_t=D_m(h^m h_x)_x+R$, on $x>0$, with an absorbing boundary $h(0,t)=0$ and initially $h=0$. Far from the boundary, $h=Rt/\phi$. Balancing the [time derivative](calculus.md#time-derivative), supply, and diffusion gives

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

[Fick's laws](physics.md#fick-s-laws) describe diffusion through a flux law and [conservation of mass](continuum-mechanics.md#mass-conservation). The first law says that [diffusive flux](physics.md#diffusive-flux) points down the concentration [gradient](calculus.md#gradient):

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

### Reaction-diffusion spectral decay threshold

↑ **Parent:** [Heat equation](#heat-equation)

On the unit interval with zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), $u_t=u_{xx}+\kappa u$ has sine-mode growth rates $\kappa-j^2\pi^2$. Every finite-energy initial condition decays exactly when the largest rate is negative, namely $\kappa<\pi^2$. A centered [finite difference](finite-difference.md) grid with $h=1/(M+1)$ has eigenvectors $\sin(j\pi m/(M+1))$ and growth rates $\kappa-4h^{-2}\sin^2(j\pi/(2(M+1)))$. Its all-data decay threshold is the displayed $\kappa_h$, strictly less than $\pi^2$ and approaching it from below. Equality leaves a stationary lowest mode; exceeding the threshold allows growth.

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

For $f\in C^2(\mathbb R^2)$ and standard [Brownian motion](brownian-motion.md) $B$, the drift in [Itô formula](stochastic-calculus.md#ito-s-lemma) for $f(B_t,t)$ vanishes exactly when the displayed equation holds for every spatial point and every $t\geq0$. Necessity follows because a zero finite-variation integral has continuous integrand $f_t(B_t,t)+\tfrac12f_{xx}(B_t,t)$ equal to zero, and at every positive time the [normal distribution](probability-theory.md#normal-distribution) of $B_t$ has full support. Continuity extends the equation to time zero. There is no condition at negative times except compatibility with the global smoothness of $f$.

### Heat equation maximum principle

↑ **Parent:** [Heat equation](#heat-equation)

On a [closed manifold](differential-geometry.md#closed-manifold) with a [Riemannian metric](differential-geometry.md#riemannian-metric), the minimum of a smooth heat solution cannot fall below its initial minimum. At a spatial minimum, $\Delta u\le0$ for the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator). Adding a small increasing function of time and considering the first crossing gives the assertion. Applying the result to nonnegative initial functions shows that the [Riemannian heat kernel](#riemannian-heat-kernel) is nonnegative.

### Heat equation energy identity

↑ **Parent:** [Heat equation](#heat-equation)

On a [closed manifold](differential-geometry.md#closed-manifold) with a [Riemannian metric](differential-geometry.md#riemannian-metric), a smooth solution of $\partial_tu+\Delta u=0$ for the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) satisfies the displayed identity by [integration by parts](calculus.md#integration-by-parts). Zero initial data force the solution to vanish, proving uniqueness and the [semigroup property](functional-analysis.md#semigroup-property) for heat evolution.

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

On a [closed manifold](differential-geometry.md#closed-manifold), the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) has a smooth [heat kernel](#heat-kernel) and its [heat semigroup](#heat-semigroup) is a [trace-class operator](compact-operator.md#trace-class-operator) for positive time. Expanding in a smooth [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) gives $K_t(x,y)=\sum_je^{-t\lambda_j}\phi_j(x)\overline{\phi_j(y)}$. [Elliptic regularity](distribution-theory.md#elliptic-regularity) bounds each derivative of $\phi_j$ polynomially in $\lambda_j$, while the exponential dominates those powers, so the expansion converges with all derivatives. Integrating the diagonal and using the unit norm of each [eigenfunction](linear-operator-theory.md#eigenfunction) proves the formula. For a bundle operator, insert the fibre [matrix trace](linear-algebra.md#matrix-trace) inside the integral.

#### Positive diffusivity requirement for the forward heat kernel

↑ **Parent:** [Heat kernel](#heat-kernel)

The real [Gaussian function](calculus.md#gaussian-function) [heat kernel](#heat-kernel) $(4\pi\varepsilon z)^{-1/2}\exp[-(\phi-\theta)^2/(4\varepsilon z)]$ is integrable only when $\varepsilon z>0$. For forward time $z>0$, this requires positive diffusivity. A [Cole-Hopf transformation](partial-differential-equation.md#cole-hopf-transformation) is an algebraic substitution for any nonzero coefficient, but that does not make the real forward [convolution](fourier-analysis.md#convolution) valid for negative diffusivity. Constant initial heat data already produce a divergent integral with the wrong sign.

#### Heat-kernel convolution

↑ **Parent:** [Heat kernel](#heat-kernel)

For the [heat equation](#heat-equation) on $\mathbb R^n$ with diffusion coefficient one, the [heat kernel](#heat-kernel) is $K_t(x)=(4\pi t)^{-n/2}e^{-|x|^2/(4t)}$. Its [convolution](fourier-analysis.md#convolution) with bounded initial data is smooth for positive time, solves the equation by differentiation under the integral, and returns [continuous](calculus.md#continuous-function) initial data locally uniformly through the [approximate identity](fourier-analysis.md#approximate-identity) property. It is [Gaussian filtering](computer-science.md#gaussian-blur) with per-coordinate variance $2t$.

#### Riemannian heat kernel

↑ **Parent:** [Heat kernel](#heat-kernel)

For the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator), the kernel solving $(\partial_t+\Delta_x)H=0$ with initial [Dirac delta distribution](distribution-theory.md#dirac-delta-function) on the diagonal represents the [heat semigroup](#heat-semigroup). On a [closed manifold](differential-geometry.md#closed-manifold) with a [Riemannian metric](differential-geometry.md#riemannian-metric) it is smooth for $t>0$, symmetric, nonnegative, preserves constants, and obeys the [semigroup property](functional-analysis.md#semigroup-property).

##### Heat kernel on a finite isometric quotient

↑ **Parent:** [Riemannian heat kernel](#riemannian-heat-kernel)

For a finite free action by [Riemannian isometries](differential-geometry.md#riemannian-isometry), the [Riemannian heat kernel](#riemannian-heat-kernel) on the quotient is the image sum shown above. Integrating over a fundamental domain combines all images into the integral on the covering manifold, proving the initial condition and showing that there is no averaging factor in the kernel. The [heat trace](riemannian-geometry.md#heat-trace) does have an averaging factor $1/|U|$, because the integral of a quotient function over the cover is $|U|$ times its quotient integral. Mere freeness of a general nondiscrete group action is not enough for this covering formula.

###### Heat semigroup descent through a finite normal covering

↑ **Parent:** [Heat kernel on a finite isometric quotient](#heat-kernel-on-a-finite-isometric-quotient)

The normalized pullback is a unitary map from $L^2$ of the quotient onto the deck-invariant subspace of $L^2$ of the cover. Local isometry and the sheet-counting integration formula preserve the Dirichlet quadratic form. Therefore the [Friedrichs extension](linear-operator-theory.md#friedrichs-extension) and its [heat semigroup](#heat-semigroup) intertwine with this map. A finite sum of lifted [Riemannian heat kernels](#riemannian-heat-kernel) gives the quotient kernel; independence of lifts follows by reindexing the deck group. This formulation avoids a uniqueness claim for unrestricted heat-equation solutions on a noncompact or incomplete manifold.

##### Spectral expansion of the Riemannian heat kernel

↑ **Parent:** [Riemannian heat kernel](#riemannian-heat-kernel)

On a [closed manifold](differential-geometry.md#closed-manifold) with a [Riemannian metric](differential-geometry.md#riemannian-metric), an [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) for the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) gives this formula, with [eigenvalues](linear-operator-theory.md#eigenvalue) counted with multiplicity. Polynomial elliptic bounds and exponential time decay give convergence of every derivative away from time zero. The conjugate is necessary for a complex basis.

##### Heat parametrix

↑ **Parent:** [Riemannian heat kernel](#riemannian-heat-kernel)

An approximate [Riemannian heat kernel](#riemannian-heat-kernel) with the correct delta initial limit and a residual extending with enough regularity to time zero. A cutoff Gaussian times transport coefficients supplies a local construction. Increasing the expansion order, or summing the full asymptotic series smoothly, makes the residual regular enough for a [Volterra parametrix correction](#volterra-parametrix-correction).

###### Heat-kernel transport equations

↑ **Parent:** [Heat parametrix](#heat-parametrix)

In [normal coordinates](general-relativity.md#normal-coordinates) $q=\exp_p x$, write the [Riemannian volume form](differential-geometry.md#riemannian-volume-form) as $J(p,x)\,dx$ and let $r=|x|$. With the [heat operator](#heat-operator) $\partial_t-\Delta_q$, the Gaussian times a power-series amplitude has its singular terms cancelled by the displayed radial equations for $i\geq1$. The initial coefficient is $w_0=J^{-1/2}$, and

$$
w_i(p,\exp_p x)=J(p,x)^{-1/2}\int_0^1s^{i-1}J(p,sx)^{1/2}(\Delta_qw_{i-1})(p,\exp_p(sx))\,ds.
$$

Multiplying the equation by $r^{i-1}J^{1/2}$ gives the derivative of $r^iJ^{1/2}w_i$. Smoothness forces the integration constant to vanish. The integral on a fixed compact interval proves smoothness across the diagonal by induction; it yields $w_i(p,p)=\Delta_qw_{i-1}(p,p)/i$. A truncated [heat parametrix](#heat-parametrix) therefore has residual $-g t^k\Delta_qw_k$.

###### Volterra parametrix correction

↑ **Parent:** [Heat parametrix](#heat-parametrix)

If $R=(\partial_t+\Delta_x)P$ is smooth and bounded up to time zero on a [closed manifold](differential-geometry.md#closed-manifold), the [Volterra convolution of kernels](analysis.md#volterra-convolution-of-kernels) solves $Q+R+R*Q=0$ by $Q=\sum_{k\ge1}(-1)^kR^{*k}$. Bounds by $C^k\operatorname{vol}(M)^{k-1}t^{k-1}/(k-1)!$ prove convergence. Then $H=P+P*Q$ is the exact [Riemannian heat kernel](#riemannian-heat-kernel) and has the same initial delta limit.

#### Gaussian interval mass

↑ **Parent:** [Heat kernel](#heat-kernel)

The normalized Gaussian mass of an interval is

$$
I_\alpha(\theta,b,w)=\frac1{\sqrt{4\pi\alpha w}}\int_{-b}^{b}e^{-(\varphi-\theta)^2/(4\alpha w)}d\varphi,\qquad\alpha,w>0.
$$

It is the convolution of an interval indicator with the [heat kernel](#heat-kernel), and has an [error function](calculus.md#error-function) representation. As the variance tends to zero it converges to the interval indicator away from its endpoints, with value one half at an endpoint. This is a concrete [approximate identity](fourier-analysis.md#approximate-identity).

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

##### Thermal trace of an interval image kernel

↑ **Parent:** [Dirichlet heat kernel on an interval](#dirichlet-heat-kernel-on-an-interval)

For a particle with mass $m$ on $(0,L)$, put $K_0(x;\beta)=\sqrt{m/(2\pi\hbar^2\beta)}e^{-mx^2/(2\hbar^2\beta)}$. The [method of images](mathematics.md#method-of-images) gives $K_D(q_f,q_i;\beta)=\sum_r[K_0(q_f-q_i+2rL;\beta)-K_0(q_f+q_i+2rL;\beta)]$. The diagonal integral is

$$
Z=L\sqrt{\frac m{2\pi\hbar^2\beta}}\sum_{r\in\mathbb Z}e^{-2mL^2r^2/(\hbar^2\beta)}-\frac12.
$$

The reflected intervals tile the real line, giving the subtraction $1/2$. The [Poisson summation formula](fourier-analysis.md#poisson-summation-formula) converts this to $\sum_{n\ge1}e^{-\beta\hbar^2\pi^2n^2/(2mL^2)}$, proving equality between the image and [energy eigenstate](quantum-mechanics.md#energy-eigenstate) calculations.

#### Gaussian heat kernel

↑ **Parent:** [Heat kernel](#heat-kernel)

For standard [Brownian motion](brownian-motion.md) in $\mathbb R^d$, $p_t(y-x)$ is the transition density from $x$ to $y$. It is the [heat kernel](#heat-kernel) for generator $\tfrac12\Delta$. For every unit vector $e$, $\int|\partial_e p_t(x)|dx=\sqrt{2/\pi}/\sqrt t$, which bounds the change in this density under a spatial translation and proves the [Gaussian heat-kernel proof of the harmonic Liouville theorem](partial-differential-equation.md#gaussian-heat-kernel-proof-of-the-harmonic-liouville-theorem).

##### Newtonian potential of the Brownian heat kernel

↑ **Parent:** [Gaussian heat kernel](#gaussian-heat-kernel)

For $d\geq3$, $A_d=\Gamma(d/2-1)/(2\pi^{d/2})$. Substitute $u=|x|^2/(2s)$ to obtain the displayed identity for $x\ne0$. The [semigroup property](functional-analysis.md#semigroup-property) and [Tonelli theorem](measure-theory.md#tonelli-theorem) then give $P_t(|\cdot|^{2-d})(x)=A_d^{-1}\int_t^\infty p_s(x)ds$. The coefficient multiplying the time integral is the reciprocal of the coefficient in the full Green integral, a distinction important in [Brownian motion](brownian-motion.md) hitting asymptotics.

#### Neumann heat kernel on an interval

↑ **Parent:** [Heat kernel](#heat-kernel)

For $L>0$ and $t>0$, the [Sturm-Liouville eigenfunction expansion](analysis.md#sturm-liouville-eigenfunction-expansion) for $u_t=u_{xx}$ on $(0,L)$ with homogeneous [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) gives

$$
K_N(x,y,t)=\frac1L+\frac2L\sum_{n=1}^\infty e^{-(n\pi/L)^2t}\cos\frac{n\pi x}{L}\cos\frac{n\pi y}{L}.
$$

The constant [eigenfunction](linear-operator-theory.md#eigenfunction) mode preserves the spatial [integral](calculus.md#integral). This is the $\beta=0$ limit of the [weighted Neumann heat kernel with constant drift](#weighted-neumann-heat-kernel-with-constant-drift), and its boundary inputs have the signs in the [Neumann boundary-forcing formula](#neumann-boundary-forcing-formula).

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

For the positive scalar [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) on a [closed manifold](differential-geometry.md#closed-manifold) with a [Riemannian metric](differential-geometry.md#riemannian-metric), the coefficient of $t^2$ in the normalized [heat trace](riemannian-geometry.md#heat-trace) is the displayed integral. The local coefficient additionally has a scalar-curvature divergence term whose integral vanishes. In dimension two, $R=2K$, $|\operatorname{Ric}|^2=2K^2$, $|\operatorname{Rm}|^2=4K^2$, giving $a_2=\frac1{15}\int_MK^2\,dA$. Together with volume and total [Gaussian curvature](second-fundamental-form.md#gaussian-curvature), it determines the variance of curvature and detects constant curvature.

###### Spectral determination of hyperbolic curvature on a surface

↑ **Parent:** [Heat invariants](#heat-invariants)

On a closed two-dimensional [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), the first three integrated scalar [heat invariants](#heat-invariants) are $A$, $\tfrac13\int K\,dA$, and $\tfrac1{15}\int K^2\,dA$, where $K$ is [Gaussian curvature](second-fundamental-form.md#gaussian-curvature). If its scalar spectrum agrees with that of a [hyperbolic surface](geometry-and-topology.md#hyperbolic-surface) of area $A$, these integrals are $A,-A/3,A/15$. Expanding the displayed square then forces $K=-1$ everywhere. Thus constant negative curvature is spectrally determined in this setting, although the global hyperbolic metric need not be determined up to [isometry](riemannian-geometry.md#isometry).

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

### Homogenization of a periodic advection-diffusion equation

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

At long wavelengths and on a [diffusive time scale](#diffusive-time-scale), a rapidly varying periodic [advection-diffusion equation](#advection-diffusion-equation) can have a constant effective [diffusivity](brownian-motion.md#diffusion-coefficient). A [multiple-scale expansion](differential-equation.md#method-of-multiple-scales) solves periodic cell equations for the fast variables. The [solvability condition](linear-operator-theory.md#solvability-condition) at the next order gives the macroscopic equation. For a periodic sinusoidal shear this is the [effective diffusivity of a periodic sinusoidal shear](fluid-mechanics.md#effective-diffusivity-of-a-periodic-sinusoidal-shear); its transverse zero-mean cell modes decay, leaving the slow conserved concentration. This use of homogenization concerns differential equations, rather than polynomial [homogenization](projective-space.md#homogenization-algebra).

### Transported step forcing in an advection-diffusion equation

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

In coordinates $s=t$, $y=x-t$, the transport derivative $u_t+u_x$ becomes $U_s$. A [Heaviside step function](analysis.md#heaviside-step-function) moving at that speed becomes stationary, and its twice-integrated profile gives the displayed continuously differentiable solution of $u_t+u_x=u_{xx}+H(x-t)$. Its second spatial derivative has a jump, so the equation holds away from the moving interface and in the distributional sense there.

### Half-line advection-diffusion global relation

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

For $u_t=u_{xx}+\beta u_x$ on $x>0$, integration by parts in its half-line [Fourier transform](analysis.md#fourier-transform) gives $\widehat u_t+(k^2-i\beta k)\widehat u=-(ik+\beta)u(0,t)-u_x(0,t)$. Its time-integrated identity relates initial data and boundary values. The spectral involution $k\mapsto-k+i\beta$ preserves $\omega=k^2-i\beta k$. Evaluating the relation at both arguments eliminates the unknown Neumann transform from a Dirichlet problem; the residual unknown solution transform vanishes upon closing the upper contour for $x>0$.

### Constant-flux tracer inlet solution

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

For a [passive scalar](fluid-mechanics.md#passive-scalar) on a half-line, impose constant total solute flux at its inlet, with initially zero [concentration](physics.md#concentration) and constant positive [advection](fluid-mechanics.md#advection) speed $U$ and [mass diffusivity](fluid-mechanics.md#mass-diffusivity) $\mathcal D$. A [Laplace transform](analysis.md#laplace-transform) in time gives

$$
\widetilde C(x,p)=\frac{2j_0}{p(U+\sqrt{U^2+4\mathcal D p})}\exp\left[\frac{U-\sqrt{U^2+4\mathcal D p}}{2\mathcal D}x\right].
$$

With $\xi=Ux/\mathcal D$, $\vartheta=U^2t/\mathcal D$ and $z_\pm=(\xi\pm\vartheta)/(2\sqrt\vartheta)$, its inverse is

$$
\frac{C(x,t)}{j_0/U}=\frac12\operatorname{erfc}(z_-)+\sqrt{\vartheta/\pi}e^{-z_-^2}-\frac12(1+\xi+\vartheta)e^\xi\operatorname{erfc}(z_+).
$$

The [complementary error function](calculus.md#complementary-error-function) describes the smeared front. This is a flux boundary condition, not the [constant-concentration inlet solution](#constant-concentration-inlet-solution). At large axial [Péclet number](fluid-mechanics.md#peclet-number), both have the leading advancing front $\tfrac12\operatorname{erfc}(z_-)$.

### Constant-concentration inlet solution

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

The half-line solution of $C_t+UC_x=DC_{xx}$ with initially zero concentration, unit inlet concentration for positive time, and decay at infinity at fixed time. Both [complementary error functions](calculus.md#complementary-error-function) are needed to satisfy the inlet exactly. A [Laplace transform](analysis.md#laplace-transform) gives $\widetilde C=p^{-1}e^{(U-\sqrt{U^2+4Dp})x/(2D)}$. A finite layer requires an additional downstream boundary condition.

### Dirichlet gauge transform for constant drift

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

For the [advection-diffusion equation](#advection-diffusion-equation) $u_t=u_{xx}+2au_x$, the multiplication $w=e^{ax}u$ gives $w_t=w_{xx}-a^2w$. A [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) remains a prescribed value, multiplied by $e^{ax}$ at the endpoint. This real exponential conjugation removes the first [derivative](calculus.md#derivative) without changing a bounded spatial interval.

#### Weighted sine transform for half-line drift diffusion

↑ **Parent:** [Dirichlet gauge transform for constant drift](#dirichlet-gauge-transform-for-constant-drift)

For $q_t=q_{xx}+\alpha q_x$, the exponential change of unknown gives $u_t=u_{xx}-\alpha^2u/4$. Its [Fourier sine transform](analysis.md#fourier-sine-transform) satisfies a closed scalar evolution with a boundary forcing term. The initial transform uses $e^{\alpha x/2}q_0(x)$; ordinary integrable-transform arguments require sufficient decay of this weighted datum. For $q_0=e^{-ax}$ this requires $a>\alpha/2$. In contrast, the unweighted sine transform of $q$ couples to its cosine transform through the drift term, so it does not directly diagonalize this half-line problem.

#### Resolvent kernel for Dirichlet advection-diffusion on an interval

↑ **Parent:** [Dirichlet gauge transform for constant drift](#dirichlet-gauge-transform-for-constant-drift)

After the [Dirichlet gauge transform for constant drift](#dirichlet-gauge-transform-for-constant-drift), put $q=\sqrt{p+a^2}$. The [Dirichlet Green function](analysis.md#dirichlet-green-function) of $p-\partial_x^2+a^2$ is

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

The ansatz $p=(Dt)^{-1}f(\eta)$ gives $[\eta f'+(\eta-r)f]'=0$. Endpoint decay sets this integrated constant to zero and hence $f\propto\eta^re^{-\eta}$; the [gamma function](complex-analysis.md#gamma-function) normalizes its [integral](calculus.md#integral) to one. Its scale is $Dt$, so it converges weakly to a unit impulse as $t\downarrow0$. Its [gamma distribution](continuous-probability-distribution.md#gamma-distribution) shape is $1+r$, its maximum occurs at $z=at$, and its [expected value](probability-theory.md#expected-value) is $(a+D)t$. For width proportional to $z$, the associated [horizontally averaged plume concentration](fluid-mechanics.md#horizontally-averaged-plume-concentration) is proportional to $z^{r-1}e^{-z/(Dt)}$: its interior maximum is $(a-D)t$ when $a>D$, its supremum occurs at the origin when $a=D$, and it is singular there when $0<a<D$. The physical finite source regularizes this ideal-origin behaviour.

### Robin gauge transform for constant drift

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

Writing $u=e^{-\beta x/2}v$ transforms $u_t=u_{xx}+\beta u_x$ into $v_t=v_{xx}-\beta^2v/4$. A prescribed coordinate derivative $u_x=g$ at an endpoint becomes $v_x-(\beta/2)v=e^{\beta x/2}g$ there. Thus a [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) becomes a [Robin boundary condition](differential-equation.md#robin-boundary-condition). The signs are coordinate-derivative signs at both endpoints; outward normal derivatives require a sign change at the left endpoint.

### Weighted Neumann heat kernel with constant drift

↑ **Parent:** [Advection-diffusion equation](#advection-diffusion-equation)

On $(0,L)$, the [differential operator](analysis.md#differential-operator) $\mathcal L=\partial_x^2+\beta\partial_x=e^{-\beta x}\partial_x(e^{\beta x}\partial_x)$ with homogeneous [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) is [self-adjoint](linear-operator-theory.md#self-adjoint-operator) in the [weighted inner product](linear-algebra.md#weighted-inner-product) with weight $e^{\beta x}$. Its [eigenfunctions](linear-operator-theory.md#eigenfunction) and nonnegative decay rates are

$$
\phi_0=1,\quad\lambda_0=0,\qquad
\phi_k=e^{-\beta x/2}\left[\cos(q_kx)+\frac\beta{2q_k}\sin(q_kx)\right],\quad
\lambda_k=q_k^2+\frac{\beta^2}4,\quad q_k=\frac{k\pi}L.
$$

Their squared [norms](functional-analysis.md#norm) are $N_0=(e^{\beta L}-1)/\beta$ and $N_k=L[1+\beta^2/(4q_k^2)]/2$. The [Sturm-Liouville eigenfunction expansion](analysis.md#sturm-liouville-eigenfunction-expansion) gives

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

These satisfy $(p-\partial_x^2-\beta\partial_x)u_p=(p-\partial_x^2-\beta\partial_x)v_p=0$ and the left and right homogeneous [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition), respectively. The weighted [Wronskian](differential-equation.md#wronskian) gives

$$
D_p=e^{\beta x}(u_p'v_p-u_pv_p')=e^{bL}\frac p\kappa\sinh(\kappa L),\qquad
\mathcal R_p(x,y)=\frac{u_p(\min(x,y))v_p(\max(x,y))}{D_p}.
$$

The first [derivative](calculus.md#derivative) jumps by $-e^{-\beta y}$, so the resolvent integrates against $e^{\beta y}\,dy$. Its time [Laplace transform](analysis.md#laplace-transform) interpretation is $\mathcal R_p=\int_0^\infty e^{-pt}K_\beta(t)dt$. The factor $p$ records the zero [eigenvalue](linear-operator-theory.md#eigenvalue) and constant stationary [eigenfunction](linear-operator-theory.md#eigenfunction).

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

### Logarithmic diffusion

↑ **Parent:** [Nonlinear diffusion equation](#nonlinear-diffusion-equation)

For a positive density $u$, logarithmic diffusion is the [nonlinear diffusion equation](#nonlinear-diffusion-equation) $u_t=\kappa\Delta\log u$, equivalently $u_t=\kappa\operatorname{div}(u^{-1}\nabla u)$. Its [diffusion coefficient](brownian-motion.md#diffusion-coefficient) is inversely proportional to the density. In one dimension, a mass-$M$ [self-similar solution](partial-differential-equation.md#similarity-solution) is

$$
u(x,t)=\frac{2\kappa t}{x^2+(2\pi\kappa t/M)^2}.
$$

Its integral is $M$, and substitution verifies the equation. This is $M$ times a [Cauchy distribution](probability-theory.md#cauchy-distribution) density of scale $2\pi\kappa t/M$. It tends weakly to $M$ times the [Dirac delta distribution](distribution-theory.md#dirac-delta-function) as $t\downarrow0$; the slow algebraic tails illustrate the enhanced diffusion where density is small.

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

Computing conductance from a smoothed [gradient](calculus.md#gradient) gives $u_t=\operatorname{div}(c(|\nabla(G_\sigma*u)|)\nabla u)$. The [image edge](computer-science.md#image-edge) detector is nonlocal, while the local highest-order diffusion has positive coefficient when conductance is positive. A smooth kernel, lower conductance bound and appropriate regularity/boundary hypotheses support a well-posed regularized filter.

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

### Bistable cubic reaction-diffusion equation

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

The scalar equation $u_t=Du_{xx}+u(1-u)(u-r)$ with $D>0$ and $0<r<1$ has two stable homogeneous phases $u=0,1$ and an unstable intervening equilibrium $u=r$. Indeed the reaction derivatives at these three equilibria are $-r$, $-(1-r)$ and $r(1-r)$, respectively. A [travelling wave](analysis.md#travelling-wave) can connect the two stable phases. At the equal-depth value $r=1/2$, its decreasing [heteroclinic orbit](dynamical-systems.md#heteroclinic-orbit) is stationary. Away from this value the phases have unequal potential depths and the front propagates.

#### Logistic front of a bistable cubic equation

↑ **Parent:** [Bistable cubic reaction-diffusion equation](#bistable-cubic-reaction-diffusion-equation)

For the decreasing front connecting $1$ to $0$, the balanced stationary [travelling-wave reduction of a reaction-diffusion system](analysis.md#travelling-wave-reduction-of-a-reaction-diffusion-system) has first integral $DU_x^2/2-U^2(1-U)^2/4=0$. Choosing the negative derivative gives $U_x=-U(1-U)/\sqrt{2D}$ and hence $U=[1+e^{(x-q)/\sqrt{2D}}]^{-1}$. This logistic profile remains an exact [travelling wave](analysis.md#travelling-wave) when the reaction parameter differs from $1/2$: using $z=(x-ct-q_0)/\sqrt D$, its derivative is $U_z=-U(1-U)/\sqrt2$, and the wave equation is satisfied for $c=\sqrt{D/2}(1-2r)$. Thus the speed changes with the potential bias while the shape, apart from [translation](geometry-and-topology.md#translation-geometry), does not.

### Basally forced quadratic activator-inhibitor model

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

A quadratic [activator](#activator-in-a-reaction-diffusion-system) can have both basal production and activation inhibited by a second species. A normalized example has reaction rates $f(u,v)=1+ru^2/v-u$ and $g(u,v)=q(u^2-v)$, with $r,q>0$ and positive concentrations. At its [spatially homogeneous equilibrium](#spatially-homogeneous-equilibrium), $v=u^2$, so $u_*=1+r$ and $v_*=(1+r)^2$. Writing $a=(r-1)/(r+1)$, its reaction [Jacobian matrix](calculus.md#jacobian-matrix) is $J=\begin{pmatrix}a&-r/(1+r)^2\\2q(1+r)&-q\end{pmatrix}$. Thus $\operatorname{tr}J=a-q$ and $\det J=q>0$, giving linear [asymptotic stability](dynamical-systems.md#asymptotic-stability) when $q>a$ and instability when $q<a$. Basal production makes $a$ change sign at $r=1$; a positive activation feedback needed for a conventional [Turing instability](#turing-instability) requires $r>1$.

#### Weak focus at the Hopf threshold of a basal activator-inhibitor model

↑ **Parent:** [Basally forced quadratic activator-inhibitor model](#basally-forced-quadratic-activator-inhibitor-model)

At $q=a=(r-1)/(r+1)>0$, the reaction [eigenvalues](linear-operator-theory.md#eigenvalue) are $\pm i\sqrt a$. This linear marginal case is a weakly attracting focus, not a nonlinear center. To check it directly, put $u=(1+r)(1+x)$, $v=(1+r)^2(1+y)$, $h=(1+a)/2$, $\beta=(1-a)/2$, $\omega=\sqrt a$, and $X=x$, $Y=(hy-a x)/\omega$. The equations become $\dot X=-\omega Y+F_2+F_3+O(4)$, $\dot Y=\omega X+G_2+G_3+O(4)$, with

$$
F_2=(\beta X-\omega Y)^2/h,\quad F_3=-(aX+\omega Y)(\beta X-\omega Y)^2/h^2,\quad G_2=\omega(hX^2-F_2),\quad G_3=-\omega F_3.
$$

On the [unit circle](complex-analysis.md#complex-unit-circle) write $A=\cos\theta F_2+\sin\theta G_2$, $B=\cos\theta F_3+\sin\theta G_3$, $C=\cos\theta G_2-\sin\theta F_2$. In [polar coordinates](calculus.md#polar-coordinates), $d\varrho/d\theta=(A/\omega)\varrho^2+(B/\omega-AC/\omega^2)\varrho^3+O(\varrho^4)$. The quadratic angular average vanishes. Integrating the quadratic correction over a whole cycle contributes its final squared integral, also zero, leaving the cubic average. Using the even trigonometric moments gives $\langle B\rangle=a/4$ and $\langle AC\rangle/\omega=(a+1)/8$. The [Poincaré map](dynamical-systems.md#poincare-map) is therefore $\varrho\mapsto\varrho+[2\pi/\omega](a-1)\varrho^3/8+O(\varrho^4)$. Since $0<a<1$, it contracts sufficiently small positive radii and proves nonlinear [asymptotic stability](dynamical-systems.md#asymptotic-stability) at the threshold.

#### Turing threshold of a basally forced quadratic activator-inhibitor model

↑ **Parent:** [Basally forced quadratic activator-inhibitor model](#basally-forced-quadratic-activator-inhibitor-model)

Add diffusivities $1,p$ to the [basally forced quadratic activator-inhibitor model](#basally-forced-quadratic-activator-inhibitor-model). A [Fourier mode](fourier-analysis.md#fourier-mode) with $s=k^2$ has matrix $J-s\operatorname{diag}(1,p)$ and [determinant](linear-algebra.md#determinant) $D(s)=ps^2+(q-pa)s+q$. When $q>a$, its [trace](linear-algebra.md#matrix-trace) is negative for every $s\geq0$. A positive-growth mode therefore occurs precisely when $D(s)<0$ for some positive $s$. The parabola has a positive minimizer only if $pa>q$, and its minimum is negative exactly when $(pa-q)^2>4pq$. Thus the ordinary [Turing instability](#turing-instability) requires $a>0$, $q>a$ and $p>q/(\sqrt{1+a}-1)^2$. At onset, $k_c^2=(pa-q)/(2p)=\sqrt{q/p}$ and the critical [wavelength](wave-equation.md#wavelength) is $2\pi(p/q)^{1/4}$. A bounded spatial domain further requires an allowed mode inside the unstable band.

### Inhibitor in a reaction-diffusion system

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

An inhibitor in an activator-inhibitor [reaction–diffusion system](#reaction-diffusion-system) suppresses the [activator](#activator-in-a-reaction-diffusion-system). Its diffusion and reaction feedback can stabilize a spatially uniform state while allowing some nonzero [wavenumbers](wave-equation.md#wavenumber) to grow through a [Turing instability](#turing-instability).

### Activator in a reaction-diffusion system

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

An activator in an activator-inhibitor [reaction–diffusion system](#reaction-diffusion-system) is a species whose local feedback enhances activation. Near a homogeneous equilibrium, positive self-feedback is reflected in the corresponding diagonal entry of the reaction [Jacobian matrix](calculus.md#jacobian-matrix). Cross-coupling to an [inhibitor](#inhibitor-in-a-reaction-diffusion-system) and differing diffusion rates can generate a [Turing instability](#turing-instability).

### Quadratic activator-inhibitor model

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

For positive concentrations and positive parameters, this [reaction–diffusion system](#reaction-diffusion-system) has homogeneous equilibrium $(u_*,v_*)=(1/b,1/b^2)$ and reaction [Jacobian matrix](calculus.md#jacobian-matrix) $\begin{pmatrix}b&-b^2\\2/b&-1\end{pmatrix}$. Its trace is $b-1$ and determinant is $b$, making the equilibrium reaction-stable exactly when $0<b<1$. Stable complex eigenvalues permit damped oscillations, which must be distinguished from sustained periodic oscillations.

#### Turing threshold of the quadratic activator-inhibitor model

↑ **Parent:** [Quadratic activator-inhibitor model](#quadratic-activator-inhibitor-model)

A mode with squared [wavenumber](wave-equation.md#wavenumber) $q$ in the [quadratic activator-inhibitor model](#quadratic-activator-inhibitor-model) has negative trace $b-1-(1+d)q$ when $0<b<1$. Its determinant is $D(q)=dq^2+(1-db)q+b$. A positive minimum location and a negative minimum require $db>1$ and $(db-1)^2>4db$, equivalent to $db>3+2\sqrt2$. At onset, the double determinant root is $q_c=(1+\sqrt2)/d$. In a bounded domain an admissible nonzero spatial mode must additionally lie in the open negative-determinant band.

#### Positive-quadrant Dulac multiplier for quadratic activation

↑ **Parent:** [Quadratic activator-inhibitor model](#quadratic-activator-inhibitor-model)

For the diffusionless [quadratic activator-inhibitor model](#quadratic-activator-inhibitor-model), choose the [Dulac function](dynamical-systems.md#dulac-function) $u^{-2}$. Then $u^{-2}f=1/v-b/u$ and $u^{-2}g=1-v/u^2$, giving divergence $(b-1)/u^2$. For $0<b<1$ it is strictly negative throughout the simply connected positive quadrant. [Green's theorem](calculus.md#green-theorem) rules out a periodic orbit: its boundary flux would be zero because the rescaled vector field is tangent to the orbit, while its interior divergence integral would be negative.

### Spatially homogeneous equilibrium

↑ **Parent:** [Reaction–diffusion system](#reaction-diffusion-system)

A spatially homogeneous equilibrium of a [reaction–diffusion system](#reaction-diffusion-system) is a constant state $u_*$ satisfying $f(u_*)=0$. Since its spatial derivatives vanish, its stability to homogeneous perturbations is determined by the [Jacobian matrix](calculus.md#jacobian-matrix) $Df(u_*)$; diffusion can additionally destabilize nonconstant modes.

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

If a fast inhibitor satisfies $0=v_{xx}+u-v$, then its spatial [Fourier transform](analysis.md#fourier-transform) obeys

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

For $u_t=Du_{xx}-u(u-r)(u-1)-\rho(v-u)$ and $0=v_{xx}-v+u$, a [Fourier mode](fourier-analysis.md#fourier-mode) perturbation about zero has $v=u/(1+k^2)$ and [growth rate](wave-equation.md#growth-rate) $\sigma(k)=-r-Dk^2+\rho k^2/(1+k^2)$. If $\rho>D$, its maximum is $-r+(\sqrt\rho-\sqrt D)^2$ at $k^2=\sqrt{\rho/D}-1$; if $\rho\leq D$, its maximum is $-r$ at zero. Replacing $(u,v,r)$ by $(1-u,1-v,1-r)$ gives the corresponding criterion at the other homogeneous equilibrium.

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

For $u'=1-(b+1)u+au^2v$, $v'=bu-au^2v$, the equilibrium $(1,b/a)$ has a [Hopf bifurcation](dynamical-systems.md#hopf-bifurcation) at $b=1+a$. Coordinates $x=u-1$, $y=-\sqrt a[(u-1)+(v-b/a)]$ give the threshold equations $x'=-\sqrt a\,y+(1-a)x^2-2\sqrt a\,xy-ax^3-\sqrt a\,x^2y$, $y'=\sqrt a\,x$. In the usual planar radial normalization the cubic coefficient is $-(a+2)/8<0$, proving a nondegenerate supercritical bifurcation. The leading small-amplitude angular frequency is $\sqrt a$.

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

## ← Incoming links (42)

- [Complex Ginzburg–Landau equation](partial-differential-equation.md#complex-ginzburg-landau-equation)
- [Diffusion](thermodynamics.md#diffusion)
- [Diffusion-controlled solute gravity current](reduced-gravity.md#diffusion-controlled-solute-gravity-current)
- [Diffusion image processing](computer-science.md#diffusion-image-processing)
- [Diffusive flux](physics.md#diffusive-flux)
- [Diffusive time scale](#diffusive-time-scale)
- [Ekman spin-down in a shallow-water layer](geophysical-fluid-dynamics.md#ekman-spin-down-in-a-shallow-water-layer)
- [Fick's laws](physics.md#fick-s-laws)
- [Isothermal diffusion with position-dependent drag](stochastic-calculus.md#isothermal-diffusion-with-position-dependent-drag)
- [Keplerian viscous diffusion equation](astrophysics.md#keplerian-viscous-diffusion-equation)
- [Molecular diffusion](thermodynamics.md#molecular-diffusion)
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
- [Saline Stefan problem](geophysics.md#saline-stefan-problem)
- [Scalar transport](fluid-mechanics.md#scalar-transport)
- [Scalar variance](fluid-mechanics.md#scalar-variance)
- [Solutal diffusivity](brownian-motion.md#solutal-diffusivity)
- [Variable-coefficient conservative diffusion equation](#variable-coefficient-conservative-diffusion-equation)
