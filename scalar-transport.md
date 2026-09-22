# Scalar transport

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[Scalar transport](scalar-transport.md) follows a material quantity through [advection](fluid-mechanics.md#advection) and [diffusion equation](diffusion-equation.md) terms, for example $\Theta_t+\mathbf U\cdot\nabla\Theta=\kappa\Delta\Theta$. A [passive scalar](#passive-scalar) does not affect the [velocity field](fluid-mechanics.md#velocity-field); an [active scalar](#active-scalar) feeds back through forces such as [buoyancy](fluid-mechanics.md#buoyancy). With [incompressible flow](fluid-mechanics.md#incompressible-flow) bounded by impermeable walls and homogeneous [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition), the spatial mean is conserved.

**Table of contents**

- [Active scalar](#active-scalar)
- [Passive scalar](#passive-scalar)
  - [Gaussian scalar packet in a linear incompressible flow](#gaussian-scalar-packet-in-a-linear-incompressible-flow)
    - [Diffusion arrest of Gaussian packet compression](#diffusion-arrest-of-gaussian-packet-compression)
      - [Large-deviation decay rates of a Gaussian scalar packet](#large-deviation-decay-rates-of-a-gaussian-scalar-packet)
  - [Schmidt number (fluid mechanics)](#schmidt-number-fluid-mechanics)
  - [Covector evolution of a material scalar gradient](#covector-evolution-of-a-material-scalar-gradient)
    - [Scalar-gradient inclination in a steady planar strain](#scalar-gradient-inclination-in-a-steady-planar-strain)
      - [White-noise vertical shear gives an Ornstein-Uhlenbeck inclination](#white-noise-vertical-shear-gives-an-ornstein-uhlenbeck-inclination)
      - [Gaussian-over-Rayleigh inclination distribution](#gaussian-over-rayleigh-inclination-distribution)
  - [Scalar structure function](#scalar-structure-function)
  - [Obukhov-Corrsin theory](#obukhov-corrsin-theory)
    - [Inertial-diffusive scalar range](#inertial-diffusive-scalar-range)
      - [Corrsin scalar microscale](#corrsin-scalar-microscale)
    - [Viscous-convective scalar range](#viscous-convective-scalar-range)
      - [Batchelor scalar microscale](#batchelor-scalar-microscale)
    - [Inertial-convective scalar range](#inertial-convective-scalar-range)
  - [Horizontally integrated plume concentration](#horizontally-integrated-plume-concentration)
    - [Horizontally averaged plume concentration](#horizontally-averaged-plume-concentration)
- [Adjoint equations for Boussinesq scalar mixing](#adjoint-equations-for-boussinesq-scalar-mixing)
- [Scalar variance](#scalar-variance)
  - [Scalar dissipation rate](#scalar-dissipation-rate)

## Active scalar

↑ **Parent:** [Scalar transport](scalar-transport.md)

An [active scalar](#active-scalar) is a transported [scalar field](classical-field-theory.md#scalar-field) that feeds back on the [velocity field](fluid-mechanics.md#velocity-field), for example a density anomaly producing [buoyancy](fluid-mechanics.md#buoyancy). In an [adjoint equations for Boussinesq scalar mixing](#adjoint-equations-for-boussinesq-scalar-mixing) calculation its dynamical coupling must also be transposed; a passive-scalar sensitivity equation generally omits that feedback.

## Passive scalar

↑ **Parent:** [Scalar transport](scalar-transport.md)

A [passive scalar](#passive-scalar) is an advected and diffusing [scalar field](classical-field-theory.md#scalar-field) whose value has no dynamical effect on the transporting [velocity field](fluid-mechanics.md#velocity-field). Concentration of a dilute nonreacting dye is a common example. Its transport can depend on the flow while the flow equations remain independent of it.

### Gaussian scalar packet in a linear incompressible flow

↑ **Parent:** [Passive scalar](#passive-scalar)

For $\chi=f\exp(-\boldsymbol x^TB\boldsymbol x)$ in two dimensions, take $B$ positive definite, $\operatorname{tr}C=0$ and positive conserved mass $Q=\int\chi\,dA$. The [Gaussian integral](integral.md#gaussian-integral) gives $Q=\pi f/\sqrt{\det B}$, $J=(Q/2)B^{-1}$ and $f=Q^2/(2\pi\sqrt{\det J})$. Substitution in the [advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation) gives $\dot B=-C^TB-BC-4\kappa B^2$ and $\dot f/f=-2\kappa\operatorname{tr}B$, equivalently the displayed moment equation. If $\dot F=CF$, its solution is $J=F[J_0+2\kappa Q\int_0^tF^{-1}(s)F^{-T}(s)ds]F^T$, with $\det F=1$.

#### Diffusion arrest of Gaussian packet compression

↑ **Parent:** [Gaussian scalar packet in a linear incompressible flow](#gaussian-scalar-packet-in-a-linear-incompressible-flow)

For a chaotic incompressible planar flow with [Lyapunov exponent](dynamical-systems.md#lyapunov-exponent) pair $\lambda,-\lambda$, an initially broad [Gaussian scalar packet in a linear incompressible flow](#gaussian-scalar-packet-in-a-linear-incompressible-flow) stretches and compresses exponentially while diffusion is negligible. Its compressed variance stops decreasing around $\kappa/\lambda$, the [Batchelor scalar microscale](#batchelor-scalar-microscale) balance, while the larger variance continues to grow. In a constant principal strain, the normalized covariance eigenvalues obey $\dot j_\pm=\pm2\lambda j_\pm+2\kappa$, proving that the compressed one approaches $\kappa/\lambda$. Random finite-correlation strain instead gives a fluctuating compressed width; stationarity and integrability assumptions are required to turn this into exponential statistics of the packet amplitude.

##### Large-deviation decay rates of a Gaussian scalar packet

↑ **Parent:** [Diffusion arrest of Gaussian packet compression](#diffusion-arrest-of-gaussian-packet-compression)

After [diffusion arrest of Gaussian packet compression](#diffusion-arrest-of-gaussian-packet-compression), define the logarithmic area increase $A_t=\tfrac12\log[\det J(t)/\det J(0)]$. It is nonnegative. Assume $A_t/t$ has a [large deviation principle](convergence-of-random-variables.md#large-deviation-principle) with convex [rate function](convergence-of-random-variables.md#rate-function) $\mathcal I$, minimized at $\lambda>0$. The exact amplitude relation $f(t)=f(0)e^{-A_t}$ and the [Laplace principle for probability measures](convergence-of-random-variables.md#laplace-principle-for-probability-measures) give the displayed moment decay rate. The rate function refers to area, so rare width fluctuations are included rather than discarded without justification. For differentiable strictly convex $\mathcal I$, the interior minimizer satisfies $\mathcal I'(s_\mu)=-\mu$. If $\mu_*=-\mathcal I'(0)$ is finite, then $\gamma_\mu=\mathcal I(0)$ for $\mu\ge\mu_*$: rare nearly unstretched packets dominate high moments. Below the threshold, $d(\gamma_\mu/\mu)/d\mu=-\mathcal I(s_\mu)/\mu^2<0$. These statements concern a positive Gaussian packet with flow-only averaging; a homogeneous signed random initial scalar requires a different averaging kernel. Arbitrary random $C(t)$ alone does not imply this statistical model.

### Schmidt number (fluid mechanics)

↑ **Parent:** [Passive scalar](#passive-scalar)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schmidt_number)

The molecular Schmidt number is the ratio of [kinematic viscosity](dynamic-viscosity.md#kinematic-viscosity) to scalar [diffusivity](brownian-motion.md#diffusion-coefficient). A large value allows a [passive scalar](#passive-scalar) to develop structure below the viscous smoothing scale of the [velocity field](fluid-mechanics.md#velocity-field). It is distinct from the [turbulent Schmidt number](turbulence.md#turbulent-schmidt-number), which compares effective turbulent transport coefficients, and from the [Schmidt number](von-neumann-entropy.md#schmidt-number) used for quantum entanglement.

### Covector evolution of a material scalar gradient

↑ **Parent:** [Passive scalar](#passive-scalar)

Differentiate the [advection equation](transport-equation.md) componentwise: $D_t(\partial_i\theta)=-(\partial_i u_j)\partial_j\theta$. Along a [Lagrangian trajectory](continuum-mechanics.md#lagrangian-trajectory), the scalar [gradient](multivariable-calculus.md#gradient) therefore evolves by the negative transpose of the [velocity gradient tensor](fluid-mechanics.md#velocity-gradient-tensor). If $F$ is the [deformation gradient](continuum-mechanics.md#deformation-gradient), this says $\boldsymbol k(t)=F(t)^{-T}\boldsymbol k(0)$, as expected for a [covector](dual-space.md#covector). Fluid material vectors and scalar gradients transform oppositely under stretching.

#### Scalar-gradient inclination in a steady planar strain

↑ **Parent:** [Covector evolution of a material scalar gradient](#covector-evolution-of-a-material-scalar-gradient)

For horizontal strain matrix $S=\bigl(\begin{smallmatrix}a&b\\b&-a\end{smallmatrix}\bigr)$ and zero vertical velocity, horizontal scalar gradients obey $\dot k_h=-Sk_h$. Since $S^2=c^2I$ with $c=\sqrt{a^2+b^2}$, the growing projection is $(I-S/c)k_h(0)/2$. If nonzero it equals $k_0(\cos\phi,\sin\phi)$ and grows as $e^{ct}$. Fixed vertical shears give $\dot k_3=-\sigma_{13}k_1-\sigma_{23}k_2$, so $k_3\sim-k_0D e^{ct}/c$ with $D=\sigma_{13}\cos\phi+\sigma_{23}\sin\phi$. The ratio $\alpha=|k_3|/|k_h|$ tends to the displayed value. It measures scalar-isosurface orientation; zero growing projection or $D=0$ must not be described as generic exponential vertical-gradient growth.

##### White-noise vertical shear gives an Ornstein-Uhlenbeck inclination

↑ **Parent:** [Scalar-gradient inclination in a steady planar strain](#scalar-gradient-inclination-in-a-steady-planar-strain)

In the long-time growing horizontal-gradient branch, independent vertical shear noises combine as $\cos\phi\,dW_1+\sin\phi\,dW_2=dW$. The signed inclination $\beta=k_3e^{-ct}/k_0$ satisfies the displayed [Ornstein-Uhlenbeck stochastic differential equation](gaussian-process.md#ornstein-uhlenbeck-stochastic-differential-equation). For $c>0$ its stationary density is $\sqrt{c/(\pi g^2)}e^{-cB^2/g^2}$, with variance $g^2/(2c)$. The [Fokker-Planck probability current](probability-theory.md#fokker-planck-probability-current) vanishes at infinity and gives this Gaussian by one integration. At $c=0$ and nonzero noise there is no normalizable stationary density.

##### Gaussian-over-Rayleigh inclination distribution

↑ **Parent:** [Scalar-gradient inclination in a steady planar strain](#scalar-gradient-inclination-in-a-steady-planar-strain)

Let $c=\sqrt{a^2+b^2}$ with independent $a,b\sim N(0,\Gamma^2)$, and let $D\sim N(0,\Lambda^2)$ be independent of them. Then $c$ has [Rayleigh distribution](continuous-probability-distribution.md#rayleigh-distribution) and $\alpha=|D|/c$ has the displayed [cumulative distribution function](probability-distribution.md#cumulative-distribution-function) for $A\ge0$ and density $\Lambda^2\Gamma(\Gamma^2A^2+\Lambda^2)^{-3/2}$. Indeed, conditioning on $D$ gives $\mathbb P(c\ge|D|/A)=\exp[-D^2/(2\Gamma^2A^2)]$, and a [Gaussian integral](integral.md#gaussian-integral) completes the calculation. Independence is essential: choosing $D=(\Lambda/\Gamma)a$ has the same Gaussian marginal but makes the ratio bounded by $\Lambda/\Gamma$.

### Scalar structure function

↑ **Parent:** [Passive scalar](#passive-scalar)

For a homogeneous scalar, $S_C(r)=2[\langle C^2\rangle-\langle CC'\rangle]$. Decorrelation at large separation gives saturation at twice the variance. If the scalar is mean-square differentiable and isotropic, $S_C(r)=r^2\langle|\nabla C|^2\rangle/3+o(r^2)$ at small separation. Statistical isotropy and zero mean alone do not imply decorrelation at infinity.

### Obukhov-Corrsin theory

↑ **Parent:** [Passive scalar](#passive-scalar)

Obukhov-Corrsin theory concerns transfer of [scalar variance](#scalar-variance) across scales in turbulent mixing. In the inertial-convective range, a constant scalar-variance flux and an eddy turnover time $\epsilon^{-1/3}r^{2/3}$ predict the displayed second-order [scalar structure function](#scalar-structure-function). It assumes a passive scalar, local transfer, approximate statistical equilibrium and separation from the molecular diffusion and forcing scales.

#### Inertial-diffusive scalar range

↑ **Parent:** [Obukhov-Corrsin theory](#obukhov-corrsin-theory)

For scalar diffusivity much larger than [kinematic viscosity](dynamic-viscosity.md#kinematic-viscosity), scalar diffusion dominates at lengths between the Kolmogorov and scalar cutoff scales. The velocity may still have inertial-range variations, but the scalar is smooth to leading order. The leading isotropic [scalar structure function](#scalar-structure-function) is quadratic, with coefficient fixed by the mean-square gradient and the [scalar dissipation rate](#scalar-dissipation-rate), rather than by a continuing inertial-convective two-thirds law.

##### Corrsin scalar microscale

↑ **Parent:** [Inertial-diffusive scalar range](#inertial-diffusive-scalar-range)

In the large-diffusivity regime, equate diffusion rate $\alpha/r^2$ with inertial eddy rate $\epsilon^{1/3}r^{-2/3}$. This gives the Corrsin scalar microscale, which exceeds the [Kolmogorov length scale](turbulence.md#kolmogorov-length-scale) when $\alpha\gg\nu$.

#### Viscous-convective scalar range

↑ **Parent:** [Obukhov-Corrsin theory](#obukhov-corrsin-theory)

For scalar diffusivity much smaller than [kinematic viscosity](dynamic-viscosity.md#kinematic-viscosity), a scalar has structure below the [Kolmogorov length scale](turbulence.md#kolmogorov-length-scale) while the velocity is smooth. The strain rate $s\sim(\epsilon/\nu)^{1/2}$ transfers scalar variance, giving $dS_C/dr\sim\epsilon_c/(sr)$. Integration produces a logarithm plus an additive matching constant.

##### Batchelor scalar microscale

↑ **Parent:** [Viscous-convective scalar range](#viscous-convective-scalar-range)

At the Batchelor scalar microscale, molecular diffusion rate $\alpha/r^2$ balances the smooth Kolmogorov strain rate $(\epsilon/\nu)^{1/2}$. For $\alpha\ll\nu$ this scale is much smaller than the [Kolmogorov length scale](turbulence.md#kolmogorov-length-scale).

#### Inertial-convective scalar range

↑ **Parent:** [Obukhov-Corrsin theory](#obukhov-corrsin-theory)

This range lies above both the [Kolmogorov length scale](turbulence.md#kolmogorov-length-scale) and the scalar diffusion cutoff, but below the forcing scale. Molecular viscosity and scalar diffusion have negligible direct influence on transfer at those scales. The [Obukhov-Corrsin theory](#obukhov-corrsin-theory) predicts a two-thirds [scalar structure function](#scalar-structure-function) there.

### Horizontally integrated plume concentration

↑ **Parent:** [Passive scalar](#passive-scalar)

The horizontally integrated plume concentration is the [integral](integral.md) of a local [concentration](mathematical-physics.md#concentration) $C$ across the plume. It measures scalar amount per unit vertical length and unit span, and its vertical [integral](integral.md) is total scalar amount per unit span. Unlike a local [concentration](mathematical-physics.md#concentration), its dimensions include one horizontal length. It must be distinguished from [horizontally averaged plume concentration](#horizontally-averaged-plume-concentration) when a plume's width varies with height.

#### Horizontally averaged plume concentration

↑ **Parent:** [Horizontally integrated plume concentration](#horizontally-integrated-plume-concentration)

For a plume of full width $w(z)$, its horizontally averaged [concentration](mathematical-physics.md#concentration) is $\overline C(z,t)=c(z,t)/w(z)$, where $c$ is [horizontally integrated plume concentration](#horizontally-integrated-plume-concentration). In a [line plume](turbulent-plume.md#line-plume) with $w=\mu z$, division by $z$ generally changes the location of maximum [concentration](mathematical-physics.md#concentration). A gradient closure for $c$ differs from one for $\overline C$: $w\partial_z\overline C=c_z-c/z$, so integrated diffusive flux $-Kw\partial_z\overline C$ equals $-K(c_z-c/z)$.

## Adjoint equations for Boussinesq scalar mixing

↑ **Parent:** [Scalar transport](scalar-transport.md)

For a smooth incompressible direct trajectory with total [velocity field](fluid-mechanics.md#velocity-field) $\mathbf U$ and [active scalar](#active-scalar) $\Theta$, the negative-constraint [Lagrangian function in constrained optimization](calculus-of-variations.md#lagrangian-function-in-constrained-optimization) convention gives

$$
\partial_t\mathbf u^\dagger+\mathbf U\cdot\nabla\mathbf u^\dagger-(\nabla\mathbf U)^T\mathbf u^\dagger+\nabla p^\dagger+\nu\Delta\mathbf u^\dagger-\theta^\dagger\nabla\Theta=0,\qquad \nabla\cdot\mathbf u^\dagger=0,
$$



$$
\partial_t\theta^\dagger+\mathbf U\cdot\nabla\theta^\dagger+\kappa\Delta\theta^\dagger-\mathrm{Ri}_B u_y^\dagger=0.
$$

The transpose term is the [formal adjoint](hilbert-space.md#formal-adjoint) of $\delta\mathbf u\cdot\nabla\mathbf U$; the two couplings transpose [scalar transport](scalar-transport.md) by [advection](fluid-mechanics.md#advection) and [buoyancy](fluid-mechanics.md#buoyancy). For terminal cost $\int\Theta(T)^2$, the terminal data are $\mathbf u^\dagger(T)=0$, $\theta^\dagger(T)=2\Theta(T)$. They are integrated backward along the stored direct trajectory. [No-slip boundary conditions](viscous-fluid-flow.md#no-slip-boundary-condition) and [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) for the adjoint [velocity](classical-mechanics.md#velocity) and homogeneous [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) for the adjoint scalar remove the spatial boundary terms.

## Scalar variance

↑ **Parent:** [Scalar transport](scalar-transport.md)

[Scalar variance](#scalar-variance) measures spatial departure from the conserved mean. For zero mean, [incompressible flow](fluid-mechanics.md#incompressible-flow) bounded by impermeable walls and homogeneous scalar [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition), [integration by parts](calculus.md#integration-by-parts) gives $d\int\Theta^2/dt=-2\kappa\int|\nabla\Theta|^2$. [Advection](fluid-mechanics.md#advection) preserves the instantaneous quadratic integral but can sharpen [gradients](multivariable-calculus.md#gradient), allowing the [diffusion equation](diffusion-equation.md) to remove [scalar variance](#scalar-variance) faster.

### Scalar dissipation rate

↑ **Parent:** [Scalar variance](#scalar-variance)

With this half-variance convention, the unforced scalar equation gives $d\langle C^2/2\rangle/dt=-\epsilon_c$ in a homogeneous incompressible flow. Authors defining dissipation of the full variance instead use $2\alpha\langle|\nabla C|^2\rangle$. Stating the convention is necessary when relating the dissipation rate to a [scalar structure function](#scalar-structure-function).

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Adjoint equations for Boussinesq scalar mixing](#adjoint-equations-for-boussinesq-scalar-mixing)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-69.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-331.md#4/a/solution)
- [Scalar transport](scalar-transport.md)
