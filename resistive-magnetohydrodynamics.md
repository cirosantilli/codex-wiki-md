# Resistive magnetohydrodynamics

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

Resistive magnetohydrodynamics retains finite [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity) in the coupled evolution of a conducting fluid and its [magnetic field](magnetic-field.md). The [resistive induction equation](#resistive-induction-equation) allows field diffusion relative to the fluid, while the [magnetohydrodynamic momentum equation](magnetohydrodynamics.md#magnetohydrodynamic-momentum-equation) includes the [Lorentz force density](relativistic-electromagnetism.md#lorentz-force-density). It contrasts with the zero-diffusivity limit of [ideal magnetohydrodynamics](ideal-magnetohydrodynamics.md).

**Table of contents**

- [Magnetic reconnection](#magnetic-reconnection)
- [Magnetic skin layer](#magnetic-skin-layer)
  - [Magnetic skin-layer streaming slip](#magnetic-skin-layer-streaming-slip)
  - [Mean Lorentz force in a magnetic skin layer](#mean-lorentz-force-in-a-magnetic-skin-layer)
- [Flux expulsion](#flux-expulsion)
  - [Phase mixing in magnetic flux expulsion](#phase-mixing-in-magnetic-flux-expulsion)
    - [Cubic-time resistive damping in a differentially rotating cell](#cubic-time-resistive-damping-in-a-differentially-rotating-cell)
- [Dynamo action](#dynamo-action)
  - [Homopolar disc dynamo](#homopolar-disc-dynamo)
    - [Torque-controlled homopolar dynamo equilibrium](#torque-controlled-homopolar-dynamo-equilibrium)
  - [Radial-flow dynamo energy bound](#radial-flow-dynamo-energy-bound)
  - [Dynamo quenching](#dynamo-quenching)
    - [Algebraic alpha quenching](#algebraic-alpha-quenching)
      - [Alpha-quenching rotating wave](#alpha-quenching-rotating-wave)
        - [Unequal-hemisphere dynamo rotating wave](#unequal-hemisphere-dynamo-rotating-wave)
  - [Equivariant three-mode dynamo normal form](#equivariant-three-mode-dynamo-normal-form)
    - [Magnetic onset on a rotating velocity branch](#magnetic-onset-on-a-rotating-velocity-branch)
    - [Normalization of nonzero dynamo coupling coefficients](#normalization-of-nonzero-dynamo-coupling-coefficients)
  - [Anti-dynamo theorem](#anti-dynamo-theorem)
    - [Periodic two-coordinate anti-dynamo energy bound](#periodic-two-coordinate-anti-dynamo-energy-bound)
    - [Planar anti-dynamo theorem](#planar-anti-dynamo-theorem)
      - [Zeldovich planar flux balance](#zeldovich-planar-flux-balance)
    - [Toroidal-velocity anti-dynamo theorem](#toroidal-velocity-anti-dynamo-theorem)
    - [Cowling anti-dynamo theorem](#cowling-anti-dynamo-theorem)
  - [Magnetic concentration by an incompressible stagnation flow](#magnetic-concentration-by-an-incompressible-stagnation-flow)
    - [Self-similar magnetic mode in a stagnation flow](#self-similar-magnetic-mode-in-a-stagnation-flow)
  - [Backus' necessary condition for dynamo action](#backus-necessary-condition-for-dynamo-action)
    - [Maximum-strain bound on dynamo growth](#maximum-strain-bound-on-dynamo-growth)
  - [Mean-field dynamo](#mean-field-dynamo)
    - [Mean-field shearing-wave transient amplification](#mean-field-shearing-wave-transient-amplification)
    - [Dipole and quadrupole parity in a mean-field dynamo](#dipole-and-quadrupole-parity-in-a-mean-field-dynamo)
      - [Coupled-hemisphere dynamo parity threshold](#coupled-hemisphere-dynamo-parity-threshold)
      - [Parity splitting of a mean-field dynamo threshold](#parity-splitting-of-a-mean-field-dynamo-threshold)
    - [Alpha-Omega dynamo](#alpha-omega-dynamo)
      - [Plane-layer alpha-Omega dynamo threshold](#plane-layer-alpha-omega-dynamo-threshold)
      - [Alpha-squared Omega dynamo threshold](#alpha-squared-omega-dynamo-threshold)
      - [Bounded-modulation alpha-Omega growth estimate](#bounded-modulation-alpha-omega-growth-estimate)
    - [Omega effect](#omega-effect)
    - [First-order smoothing approximation](#first-order-smoothing-approximation)
      - [Isotropic alpha effect of three helical traveling waves](#isotropic-alpha-effect-of-three-helical-traveling-waves)
      - [Helicity formula for isotropic first-order smoothing](#helicity-formula-for-isotropic-first-order-smoothing)
      - [Quasistatic magnetic response of a helical shearing wave](#quasistatic-magnetic-response-of-a-helical-shearing-wave)
      - [Monochromatic coupled magnetic and velocity response](#monochromatic-coupled-magnetic-and-velocity-response)
      - [Oscillatory magnetic response in first-order smoothing](#oscillatory-magnetic-response-in-first-order-smoothing)
    - [Parker dynamo wave](#parker-dynamo-wave)
      - [Local alpha-Omega dynamo wave dispersion](#local-alpha-omega-dynamo-wave-dispersion)
      - [Periodically reversing Parker dynamo coupling](#periodically-reversing-parker-dynamo-coupling)
    - [Alpha effect](#alpha-effect)
      - [Rapidly fluctuating alpha effect](#rapidly-fluctuating-alpha-effect)
      - [Strong-field quenching of an isotropic electromotive force](#strong-field-quenching-of-an-isotropic-electromotive-force)
      - [Alpha-squared dynamo](#alpha-squared-dynamo)
        - [Homogeneous alpha-squared dynamo growth criterion](#homogeneous-alpha-squared-dynamo-growth-criterion)
        - [Anisotropic alpha-squared dynamo](#anisotropic-alpha-squared-dynamo)
          - [Uniaxial alpha dynamo threshold](#uniaxial-alpha-dynamo-threshold)
      - [Alpha tensor](#alpha-tensor)
    - [Mean-field electromotive force](#mean-field-electromotive-force)
      - [Monochromatic small-Reynolds-number mean electromotive force](#monochromatic-small-reynolds-number-mean-electromotive-force)
        - [Antisymmetry of the second-order monochromatic alpha tensor](#antisymmetry-of-the-second-order-monochromatic-alpha-tensor)
        - [Symmetry of the first-order monochromatic alpha tensor](#symmetry-of-the-first-order-monochromatic-alpha-tensor)
      - [Turbulent magnetic pumping](#turbulent-magnetic-pumping)
      - [Integrated electromotive response of a finite cyclonic event](#integrated-electromotive-response-of-a-finite-cyclonic-event)
      - [Space-time average of periodic modes](#space-time-average-of-periodic-modes)
- [Hartmann flow](#hartmann-flow)
  - [Hartmann flow rate with normal-field walls](#hartmann-flow-rate-with-normal-field-walls)
  - [Hartmann layer](#hartmann-layer)
  - [Hartmann number](#hartmann-number)
- [Normal magnetic field boundary condition](#normal-magnetic-field-boundary-condition)
- [Resistive induction equation](#resistive-induction-equation)
  - [Conductivity-gradient term in magnetic induction](#conductivity-gradient-term-in-magnetic-induction)
  - [Shearing-coordinate magnetic flux equation](#shearing-coordinate-magnetic-flux-equation)
  - [Radial magnetic induction scalar](#radial-magnetic-induction-scalar)
    - [Insulating boundary condition for the radial magnetic scalar](#insulating-boundary-condition-for-the-radial-magnetic-scalar)

## Magnetic reconnection

↑ **Parent:** [Resistive magnetohydrodynamics](resistive-magnetohydrodynamics.md)

Magnetic reconnection changes connectivity between [magnetic field lines](magnetic-field.md#magnetic-field-line). It requires departure from smooth [magnetic flux freezing](ideal-magnetohydrodynamics.md#magnetic-flux-freezing), for example through finite resistivity or other nonideal terms concentrated in a [current sheet](electric-charge.md#current-sheet). Ideal viscous [magnetic relaxation](ideal-magnetohydrodynamics.md#magnetic-relaxation) dissipates mechanical energy while retaining frozen connectivity, so viscosity alone does not provide reconnection.

## Magnetic skin layer

↑ **Parent:** [Resistive magnetohydrodynamics](resistive-magnetohydrodynamics.md)

A magnetic skin layer is the thin region penetrated by an oscillating [magnetic field](magnetic-field.md) in a conductor. For locally tangential boundary amplitude $C(x)$, negligible material motion and variations along the boundary much slower than those across it, the [resistive induction equation](#resistive-induction-equation) gives $B_x=C(x)e^{-(1+i)y/\delta}$ with time convention $e^{i\omega t}$. The [solenoidal magnetic-field constraint](magnetic-field.md#solenoidal-magnetic-field-constraint) requires the smaller component $B_y=C'(x)e^{-(1+i)y/\delta}\delta/(1+i)$ to leading order. The tangential-field approximation therefore does not mean that the normal component is exactly zero at finite [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity).

### Magnetic skin-layer streaming slip

↑ **Parent:** [Magnetic skin layer](#magnetic-skin-layer)

In a thin [magnetic skin layer](#magnetic-skin-layer) next to a rigid [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition), vertical [pressure](pressure.md) balance gives $p=P-C^2e^{-2y/\delta}/(4\mu_0)$. With negligible inertia in the layer, the tangential [Stokes flow](stokes-flow.md) balance is $\rho\nu u_{yy}=p_x$. Matching zero leading shear outside the layer gives $u=U(1-e^{-2y/\delta})$ and the displayed effective tangential slip. The physical wall still has zero [velocity](classical-mechanics.md#velocity); the slip is a boundary condition for the outer flow extrapolated through the unresolved layer. It points toward larger squared boundary-field amplitude.

### Mean Lorentz force in a magnetic skin layer

↑ **Parent:** [Magnetic skin layer](#magnetic-skin-layer)

For real boundary amplitude $C$ and $q=(1+i)/\delta$, the leading [electric current density](electric-charge.md#current-density) is $j_z=qCe^{-qy}/\mu_0$. Averaging products of real harmonic fields gives $\overline{\mathbf F}=\operatorname{Re}[(\nabla\times\mathbf B)\times\mathbf B^*]/(2\mu_0)$. Its leading normal component is the displayed positive force. The first candidate tangential contribution is proportional to $\operatorname{Re}(q/q^*)CC'=0$, so retaining the small normal field does not introduce a tangential force of that order.

## Flux expulsion

↑ **Parent:** [Resistive magnetohydrodynamics](resistive-magnetohydrodynamics.md)

Flux expulsion is redistribution of [magnetic flux](magnetic-field.md#magnetic-flux) out of the interiors of persistent circulating flows into their edges and surrounding regions. In two-dimensional [incompressible flow](fluid-mechanics.md#incompressible-flow), a magnetic flux function obeys $\partial_t A+\mathbf u\cdot\nabla A=\eta\nabla^2 A$. At large but finite [magnetic Reynolds number](magnetohydrodynamics.md#magnetic-reynolds-number), circulation stretches gradients of $A$, enabling resistive smoothing and weak interior [magnetic field](magnetic-field.md) with strong field near the circulation boundary. Finite [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity) is essential to the eventual rearrangement; exact ideal [magnetic flux freezing](ideal-magnetohydrodynamics.md#magnetic-flux-freezing) alone does not justify a flux-free steady cell. Magnetic back reaction can limit the process.

### Phase mixing in magnetic flux expulsion

↑ **Parent:** [Flux expulsion](#flux-expulsion)

Differential circulation of a weak [magnetic field](magnetic-field.md) winds its flux function into progressively smaller radial scales. In a smooth eddy with angular-velocity gradient of order $U/L^2$, its radial wavenumber grows as $k_r\sim Ut/L^2$. Resistive damping becomes substantial when $\eta\int_0^t k_r^2dt\sim1$, giving $t\sim(L^4/(\eta U^2))^{1/3}=(L/U)\mathrm{Rm}^{1/3}$. This estimate presumes differential rotation and negligible magnetic feedback; a rigidly rotating eddy does not create this phase mixing. Finite [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity) then permits weak interior field and boundary concentration, unlike exact ideal flux freezing.

#### Cubic-time resistive damping in a differentially rotating cell

↑ **Parent:** [Phase mixing in magnetic flux expulsion](#phase-mixing-in-magnetic-flux-expulsion)

In a smooth interior region with locally constant shear $\Omega'$, a wound azimuthal [Fourier mode](fourier-analysis.md#fourier-mode) has radial [wavenumber](wave-equation.md#wavenumber) $k_s\simeq-m\Omega't$. Integrating its resistive damping rate $\eta k_s^2$ gives the [exponential decay](analysis.md#exponential-decay) in the title. The characteristic time is $\tau_c=[3/(\eta m^2\Omega'^2)]^{1/3}$. For $m=1$ and $\Omega'=-\Omega_0/d$, $\Omega_0\tau_c=(3\mathrm{Rm})^{1/3}$, where $\mathrm{Rm}=\Omega_0d^2/\eta$. This is a high-[magnetic Reynolds number](magnetohydrodynamics.md#magnetic-reynolds-number) interior transient on a time long compared with the rotation time but short compared with $d^2/\eta$. Physical [magnetic field](magnetic-field.md) components may have additional algebraic factors from taking [derivatives](calculus.md#derivative) of the wound [magnetic vector potential](electromagnetism.md#magnetic-vector-potential). A maintained exterior field, an axial core and a circulation-edge [boundary layer](continuum-mechanics.md#boundary-layer) prevent interpreting this estimate as an exact, uniform, infinite-time solution.

## Dynamo action

↑ **Parent:** [Resistive magnetohydrodynamics](resistive-magnetohydrodynamics.md)

Dynamo action is growth or sustained maintenance of a [magnetic field](magnetic-field.md) by conducting-fluid motion despite magnetic diffusion. In the kinematic problem the velocity is prescribed and the [resistive induction equation](#resistive-induction-equation) is linear in the [magnetic field](magnetic-field.md). Magnetic feedback through the [Lorentz force density](relativistic-electromagnetism.md#lorentz-force-density) matters once the field becomes dynamically important.

### Homopolar disc dynamo

↑ **Parent:** [Dynamo action](#dynamo-action)

Connect a [homopolar generator](electromagnetism.md#homopolar-generator) to a [solenoid](magnetic-field.md#solenoid) producing its own axial field. Reinforcing winding and rotation give $C=\mu_0Na^2/(2l)$ and $L\dot I=(C\omega-R)I$. A seed field grows for $\omega>R/C$, is marginal at equality, and decays below threshold. An identically zero initial field remains zero in this homogeneous ideal model; startup requires a seed or perturbation.

#### Torque-controlled homopolar dynamo equilibrium

↑ **Parent:** [Homopolar disc dynamo](#homopolar-disc-dynamo)

For steady rotation at nonzero current, the electromagnetic braking [torque](momentum.md#torque) is $CI^2$ and balances applied [torque](momentum.md#torque) $G$. Thus $I^2=G/C$, while the circuit requires $\omega=R/C$. With $H=NI/l$, these give the displayed field and $G\omega=I^2R$. This is a steady [energy](energy.md) balance, not a general nonlinear stability claim.

### Radial-flow dynamo energy bound

↑ **Parent:** [Dynamo action](#dynamo-action)

Let a [solenoidal](multivariable-calculus.md#solenoidal-vector-field) flow be confined to a sphere $V$, with the [insulating boundary condition for the radial magnetic scalar](#insulating-boundary-condition-for-the-radial-magnetic-scalar). Define $N=\int_VP^2$, $D=\int_{\mathbb R^3}|\nabla P|^2$, $M=\int_{\mathbb R^3}|\mathbf B|^2$ and $q=\max_V|\mathbf u\cdot\mathbf x|$. [Integration by parts](calculus.md#integration-by-parts) inside and outside the sphere gives

$$
\frac12N'=-\int_VQ\,\mathbf B\cdot\nabla P-\eta D\leq q\sqrt{MD}-\eta D.
$$

The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) therefore makes $q^2\geq\eta^2D/M$ necessary whenever $N'\geq0$ and $D>0$. A uniform strict violation with a positive gap forces decay, using a [Sobolev inequality](sobolev-space.md#sobolev-inequality) to bound $N$ by a constant times $D$. A bounded statistically steady field instead requires $q_*^2\geq\eta^2\langle D\rangle/\langle M\rangle$, with $q_*=\sup_tq(t)$. This is a necessary condition for [dynamo action](#dynamo-action), not a sufficient criterion or a pointwise assertion at every instant of an arbitrary time-dependent solution.

// Target: analysis.bigb

### Dynamo quenching

↑ **Parent:** [Dynamo action](#dynamo-action)

[Dynamo quenching](#dynamo-quenching) is the reduction or modification of magnetic-field generation by magnetic feedback on the generating flow and its correlations. The [Lorentz force](relativistic-electromagnetism.md#lorentz-force) can change shear or turbulence, while [magnetic helicity](electromagnetism.md#magnetic-helicity) affects mean-field regeneration. A phenomenological [scalar](vector-space.md#scalar) example is $\alpha(B)=\alpha_0/(1+B^2/B_*^2)$. In the illustrative amplitude equation $\dot B=[c\alpha(B)-d]B$ with $c,d>0$, a growing field saturates at $B^2=B_*^2(c\alpha_0/d-1)$ when $c\alpha_0>d$. This demonstrates the negative feedback mechanism without claiming that algebraic quenching is a complete solar closure.

#### Algebraic alpha quenching

↑ **Parent:** [Dynamo quenching](#dynamo-quenching)

Algebraic alpha quenching prescribes a field-dependent [alpha effect](#alpha-effect) as a closure for nonlinear [mean-field dynamo](#mean-field-dynamo) feedback. The polynomial law $\alpha=\alpha_0-p|B|^2$ with $p>0$ decreases alpha, so it can saturate positive alpha but makes negative alpha more negative. It therefore differs importantly from the sign-preserving rational law $\alpha_0/(1+|B|^2/B_*^2)$. Its solutions must satisfy nonnegative squared-amplitude conditions; an assertion based only on large $|\alpha_0|$ need not hold for both signs.

##### Alpha-quenching rotating wave

↑ **Parent:** [Algebraic alpha quenching](#algebraic-alpha-quenching)

A rotating wave in a complex [dynamo quenching](#dynamo-quenching) model has constant amplitude and a common phase factor $e^{i\omega t}$. In the two-hemisphere model with toroidal coupling parameter $\epsilon_2=0$, eliminating the poloidal amplitudes gives

$$
\frac{2\omega-i(1-\omega^2)}{\Omega}\begin{pmatrix}B_1\\B_2\end{pmatrix}=\begin{pmatrix}\alpha_0-p|B_1|^2&\epsilon_1\\\epsilon_1&\alpha_0-p|B_2|^2\end{pmatrix}\begin{pmatrix}B_1\\B_2\end{pmatrix}.
$$

The matrix is [Hermitian](hilbert-space.md#hermitian-operator), so its [eigenvalue](linear-operator-theory.md#eigenvalue) is real and a nonzero rotating wave with $\Omega\ne0$ has $\omega=\pm1$. Writing $a=\alpha_0-2\omega/\Omega$, pure dipole and quadrupole waves have $|B_j|^2=(a-\epsilon_1)/p$ and $(a+\epsilon_1)/p$, respectively, when those quantities are positive.

###### Unequal-hemisphere dynamo rotating wave

↑ **Parent:** [Alpha-quenching rotating wave](#alpha-quenching-rotating-wave)

For nonzero coupling $\epsilon_1$, an [alpha-quenching rotating wave](#alpha-quenching-rotating-wave) can be made real in its toroidal amplitudes by a common phase rotation. Set $a=\alpha_0-2\omega/\Omega$. The amplitude equations are $(a-pB_1^2)B_1+\epsilon_1B_2=0$ and $(a-pB_2^2)B_2+\epsilon_1B_1=0$. Subtracting after cross multiplication gives $(B_1^2-B_2^2)(pB_1B_2+\epsilon_1)=0$. Unequal magnitudes therefore require $B_1B_2=-\epsilon_1/p$ and $B_1^2+B_2^2=a/p$. They exist exactly when $a>2|\epsilon_1|$ and have the displayed squared amplitudes. Exchanging hemispheres yields the companion solution. This breaks equatorial reflection symmetry and combines both [dipole and quadrupole parity in a mean-field dynamo](#dipole-and-quadrupole-parity-in-a-mean-field-dynamo). Existence does not alone prove nonlinear stability.

### Equivariant three-mode dynamo normal form

↑ **Parent:** [Dynamo action](#dynamo-action)

An axisymmetric magnetic mode is unchanged by axial rotations, while an equatorial magnetic mode and a corresponding velocity mode transform as $A,V\mapsto e^{i\theta}(A,V)$. Magnetic reversal sends $(B,A,V)$ to $(-B,-A,V)$. For magnetic evolution linear in magnetic amplitudes, rotational [equivariance](group-action.md#equivariant-map) requires $\dot B=Bf(|V|^2)+2\operatorname{Re}[A^*Vg(|V|^2)]$ and $\dot A=Ah(|V|^2)+BVj(|V|^2)+A^*V^2\ell(|V|^2)$, with $f$ real and the other functions complex. Velocity monomials $B^pA^q(A^*)^rV^s(V^*)^t$ must have even $p+q+r$ and weight $q-r+s-t=1$. These conditions enumerate the cubic [normal form](bifurcation-theory.md#normal-form-dynamical-systems) without assuming reflection symmetry or nonlinear magnetic self-interactions.

#### Magnetic onset on a rotating velocity branch

↑ **Parent:** [Equivariant three-mode dynamo normal form](#equivariant-three-mode-dynamo-normal-form)

For real $c_2,d_4$ and the simplified magnetic amplitude equations, the pure-velocity branch is $V=se^{i\omega_3t}$ with $A=B=0$. In its rotating frame the magnetic linearization on $(B,\operatorname{Re}A,\operatorname{Im}A)$ has rows $(\mu_1-es^2,2s,0)$, $(c_2s,\mu_2,-\Delta)$ and $(0,\Delta,\mu_2)$, where $\Delta=\omega_2-\omega_3$. Its zero determinant gives the displayed onset relation. A nonzero magnetic branch needs a kernel involving both magnetic amplitudes, a transverse parameter crossing and nondegenerate nonlinear saturation; determinant zero alone is insufficient in degenerate cases.

#### Normalization of nonzero dynamo coupling coefficients

↑ **Parent:** [Equivariant three-mode dynamo normal form](#equivariant-three-mode-dynamo-normal-form)

For nonzero coefficients of $A^*V$ in $\dot B$ and $AB$ in $\dot V$, a relative phase rotation makes $c_1$ real positive. Positive rescalings of $A,V,B$ then normalize both magnitudes to one. The phase of $c_1c_3$ is invariant under these rescalings and remains as the phase of normalized $c_3$. Zero couplings cannot be normalized to one; they are degenerate parameter cases.

### Anti-dynamo theorem

↑ **Parent:** [Dynamo action](#dynamo-action)

An anti-dynamo theorem gives a geometric or analytic restriction excluding self-sustained [dynamo action](#dynamo-action) under stated [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity), domain and boundary conditions. It excludes regeneration against resistive decay, not all transient amplification or field induced by an external source. Important restrictions include [Cowling anti-dynamo theorem](#cowling-anti-dynamo-theorem), the [toroidal-velocity anti-dynamo theorem](#toroidal-velocity-anti-dynamo-theorem), and the [planar anti-dynamo theorem](#planar-anti-dynamo-theorem). [Backus' necessary condition for dynamo action](#backus-necessary-condition-for-dynamo-action) instead bounds the stretching required for possible regeneration.

#### Periodic two-coordinate anti-dynamo energy bound

↑ **Parent:** [Anti-dynamo theorem](#anti-dynamo-theorem)

For a solenoidal three-component velocity depending on two periodic coordinates and a zero-mean magnetic field with the same dependence, the in-plane flux potential satisfies a homogeneous [advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation). The [Poincaré inequality](sobolev-space.md#poincare-inequality) gives $\langle A^2\rangle\leq\langle A_0^2\rangle e^{-2\eta k^2t}$. Integrating the vertical stretching term by parts bounds it by $Q\sqrt{\langle A^2\rangle\langle|\nabla B_z|^2\rangle}$, where $Q=\|\nabla u_z\|_\infty$. Maximizing against resistive dissipation and integrating gives the displayed transient bound. Splitting off half the dissipation instead gives $E'+\eta k^2E\leq(Q^2/\eta)\langle A_0^2\rangle e^{-2\eta k^2t}$, proving vertical energy decays. This permits transient generation by a nonzero vertical velocity while excluding sustained fields in this zero-mean, z-independent periodic class.

#### Planar anti-dynamo theorem

↑ **Parent:** [Anti-dynamo theorem](#anti-dynamo-theorem)

In the standard two-dimensional setting, with planar [velocity](classical-mechanics.md#velocity) and [magnetic field](magnetic-field.md) independent of the third coordinate and homogeneous energy-closed boundary conditions, the in-plane magnetic potential is an advected diffusing scalar. Its quadratic integral decreases, preventing regeneration of a dynamo field. A third field component independent of that coordinate also obeys a passive advection-diffusion equation. A flow depending on two coordinates but possessing a third velocity component is not covered by this strictly planar formulation.

##### Zeldovich planar flux balance

↑ **Parent:** [Planar anti-dynamo theorem](#planar-anti-dynamo-theorem)

For a stationary planar advected magnetic flux potential, average its [advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation) horizontally and split it into mean and fluctuation. The mean transport is $\overline{wa'}=\eta\bar a_z+C$, with $C=\langle wa'\rangle$. Multiplying the fluctuation equation by $a'$ and applying [integration by parts](calculus.md#integration-by-parts) gives $\langle\overline{wa'}\bar a_z\rangle+B_0C=-\eta\langle|\nabla a'|^2\rangle$. A vanishing mean derivative removes the constant term in the first correlation, yielding the displayed dissipative identity. The boundary assumptions must eliminate surface terms; a periodic layer replaces, rather than accompanies, decay at vertical infinity.

#### Toroidal-velocity anti-dynamo theorem

↑ **Parent:** [Anti-dynamo theorem](#anti-dynamo-theorem)

For a bounded conducting sphere with uniform [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity) and an insulating exterior, an [incompressible flow](fluid-mechanics.md#incompressible-flow) tangent to concentric spheres cannot sustain [dynamo action](#dynamo-action). Neither the [velocity](classical-mechanics.md#velocity) nor the [magnetic field](magnetic-field.md) needs to be axisymmetric. The radial magnetic scalar has a homogeneous advection-diffusion equation, so the poloidal field decays. Once it is absent, the toroidal magnetic potential also has a homogeneous scalar advection-diffusion equation. This is a theorem about spherical flow geometry, not about a general cylindrical flow with an axial component.

#### Cowling anti-dynamo theorem

↑ **Parent:** [Anti-dynamo theorem](#anti-dynamo-theorem)

An isolated axisymmetric [magnetic field](magnetic-field.md) cannot be sustained by ordinary resistive [dynamo action](#dynamo-action) with scalar positive [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity). Its [poloidal magnetic flux function](ideal-magnetohydrodynamics.md#poloidal-magnetic-flux-function) satisfies a homogeneous scalar advection-diffusion equation with no toroidal-to-poloidal source. The maximum principle excludes regeneration of that flux; after it decays the toroidal field has no lasting source either. This constrains the symmetry of the field. An [axisymmetric flow](fluid-mechanics.md#axisymmetric-flow) may still generate a nonaxisymmetric field, and a turbulent mean-field electromotive force is not covered by the unmodified scalar-induction proof.

### Magnetic concentration by an incompressible stagnation flow

↑ **Parent:** [Dynamo action](#dynamo-action)

The linear [incompressible flow](fluid-mechanics.md#incompressible-flow) $\mathbf u=(-\omega x,-\omega y,2\omega z)$ compresses the transverse plane and stretches the axial direction. An axial [magnetic field](magnetic-field.md) obeys $B_t-\omega rB_r=2\omega B+\eta\Delta_\perp B$. In [ideal magnetohydrodynamics](ideal-magnetohydrodynamics.md), its amplitude grows as $e^{2\omega t}$ while its transverse width decreases as $e^{-\omega t}$. Thus its [magnetic energy](electromagnetic-wave.md#magnetic-energy) per unit axial length grows as $e^{2\omega t}$, even when opposite-polarity angular sectors give zero signed [magnetic flux](magnetic-field.md#magnetic-flux). Finite [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity) limits the amplification of localized finite-flux Gaussian fields.

#### Self-similar magnetic mode in a stagnation flow

↑ **Parent:** [Magnetic concentration by an incompressible stagnation flow](#magnetic-concentration-by-an-incompressible-stagnation-flow)

For [magnetic concentration by an incompressible stagnation flow](#magnetic-concentration-by-an-incompressible-stagnation-flow), one possible normalization gives $(g^2)'=2\eta-2\omega g^2$, $f'/f=2\omega-\lambda\eta/g^2$, and $b''+(q^{-1}+q)b'+(\lambda-m^2/q^2)b=0$. The mode parameter $\lambda$ is not fixed by decay at infinity alone. The regular axisymmetric Gaussian has $\lambda=2$, $b=e^{-q^2/2}$ and conserved axial [magnetic flux](magnetic-field.md#magnetic-flux), with energy proportional to $g^{-2}$. The radial equation also has regular algebraic-tail solutions.

### Backus' necessary condition for dynamo action

↑ **Parent:** [Dynamo action](#dynamo-action)

For an isolated bounded conductor of uniform [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity) $\eta>0$, contained in a sphere of radius $R$ and matched to a decaying potential field in an insulating exterior, [dynamo action](#dynamo-action) requires maximum stretching rate $S\geq\eta\pi^2/R^2$. Here $S$ bounds the largest [eigenvalue](linear-operator-theory.md#eigenvalue) of the [rate-of-strain tensor](viscous-fluid-flow.md#strain-rate-tensor) throughout the flow and time. Use fluid boundary conditions eliminating the stretching boundary term, for example a [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition), and no imposed energy input. The proof combines the [magnetic free-decay spectral bound](magnetohydrodynamics.md#magnetic-free-decay-spectral-bound) with the [magnetic energy](electromagnetic-wave.md#magnetic-energy) equation. This is a necessary condition, not a sufficiency criterion; changing magnetic boundary conditions changes the spectral constant.

#### Maximum-strain bound on dynamo growth

↑ **Parent:** [Backus' necessary condition for dynamo action](#backus-necessary-condition-for-dynamo-action)

Under the energy-closed boundary assumptions of [Backus' necessary condition for dynamo action](#backus-necessary-condition-for-dynamo-action), the [magnetic energy](electromagnetic-wave.md#magnetic-energy) equation gives $\dot E_B\leq2s(t)E_B$ after discarding nonnegative resistive dissipation. Integrating gives an upper bound by the time average of the largest spatial [eigenvalue](linear-operator-theory.md#eigenvalue) of the [rate-of-strain tensor](viscous-fluid-flow.md#strain-rate-tensor). Thus the field-amplitude exponent is at most its space-time supremum. The exponent of squared energy is twice the field-amplitude exponent.

### Mean-field dynamo

↑ **Parent:** [Dynamo action](#dynamo-action)

A mean-field dynamo evolves a slowly varying spatially averaged [magnetic field](magnetic-field.md). Correlations of fluctuating velocity and magnetic field supply a [mean-field electromotive force](#mean-field-electromotive-force). Its local linear response includes the [alpha effect](#alpha-effect); gradients of the mean field can contribute additional transport terms. The distinction between a uniform test field used to measure a response coefficient and a spatially varying mean field used to obtain growth is essential.

#### Mean-field shearing-wave transient amplification

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

For $k(t)=k_0\sqrt{1+(t/T)^2}$, factor resistive damping out of the shearing-mode equations by $R=e^{-D}G$, $S=e^{-D}H$, $D=\eta\int k^2dt$. They imply $G''=\alpha^2k^2G$, so a growing [WKB approximation](analysis.md#wkb-approximation) has $G\propto k^{-1/2}e^{|\alpha|\int kdt}$ and $H\simeq i\operatorname{sgn}(\alpha)kG$. Its [magnetic energy](electromagnetic-wave.md#magnetic-energy) is proportional to $k\exp[2|\alpha|\int kdt-2\eta\int k^2dt]$. At long times the positive quadratic exponent is overtaken by negative cubic resistive damping. A well-separated growing interval exists for sufficiently small positive [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity), with $\eta k_0/|\alpha|\ll1$ at fixed nonzero $|\alpha|k_0T$, and the displayed leading peak time. This is transient amplification, not an asymptotically self-sustaining dynamo.

#### Dipole and quadrupole parity in a mean-field dynamo

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

In a reflection-symmetric [mean-field dynamo](#mean-field-dynamo) model, dipole parity can be represented by an even poloidal-potential amplitude and an odd toroidal-field amplitude; quadrupole parity reverses these assignments. The names describe the reflection classes appropriate to the model, not arbitrary electric multipoles. A complex amplitude $P=A+iB$ allows a phase rotation by $i$ to interchange the two classes when the unperturbed equations have that phase symmetry.

##### Coupled-hemisphere dynamo parity threshold

↑ **Parent:** [Dipole and quadrupole parity in a mean-field dynamo](#dipole-and-quadrupole-parity-in-a-mean-field-dynamo)

In a two-hemisphere [mean-field dynamo](#mean-field-dynamo), dipole and quadrupole subspaces can reduce to $\dot A=aB-A$, $\dot B=bA-B$, with $(a,b)=(\alpha_0-\epsilon_1,i\Omega-\epsilon_2)$ and $(\alpha_0+\epsilon_1,i\Omega+\epsilon_2)$ respectively. Their [eigenvalues](linear-operator-theory.md#eigenvalue) satisfy $(\lambda+1)^2=ab$. Strict decay is equivalent to $\operatorname{Re}(ab)+[\operatorname{Im}(ab)]^2/4<1$. Thus dipole decay requires $F_d<1$, while quadrupole decay requires $F_q=\Omega^2(\alpha_0+\epsilon_1)^2/4+\epsilon_2(\alpha_0+\epsilon_1)<1$. Their difference is $F_q-F_d=\alpha_0(\Omega^2\epsilon_1+2\epsilon_2)$, which selects the first unstable parity when starting from a state stable in both subspaces.

##### Parity splitting of a mean-field dynamo threshold

↑ **Parent:** [Dipole and quadrupole parity in a mean-field dynamo](#dipole-and-quadrupole-parity-in-a-mean-field-dynamo)

An antisymmetric perturbation can split the thresholds of two degenerate [mean-field dynamo](#mean-field-dynamo) parity classes. At first order, project the perturbation equation onto the adjoint null mode using the [Fredholm alternative](compact-operator.md#fredholm-alternative). If multiplying the unperturbed complex mode by $i$ leaves the parameter-derivative matrix element unchanged but reverses the perturbation matrix element, the two first-order threshold shifts are equal and opposite.

#### Alpha-Omega dynamo

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

An alpha-Omega [mean-field dynamo](#mean-field-dynamo) couples toroidal-field generation by the [Omega effect](#omega-effect) to poloidal-field regeneration by the [alpha effect](#alpha-effect). A simple Fourier model is $\dot A=\alpha_0 f(t)B-\eta k^2A$, $\dot B=ik\Omega A-\eta k^2B$, where $A$ is a component of the [vector potential](multivariable-calculus.md#vector-potential) for the poloidal field and $B$ is a toroidal-field amplitude. For bounded $|f|\leq1$, the [bounded-modulation alpha-Omega growth estimate](#bounded-modulation-alpha-omega-growth-estimate) controls the maximum amplification.

##### Plane-layer alpha-Omega dynamo threshold

↑ **Parent:** [Alpha-Omega dynamo](#alpha-omega-dynamo)

For a [mean-field dynamo](#mean-field-dynamo) with uniform alpha, shear $\pi V/d$, diffusivity $\eta>0$ and fixed vertical wavenumber $\pi/d$, a horizontal Fourier mode obeys $(s+\eta(k^2+\pi^2/d^2))^2=i\alpha\pi Vk/d$. With $D=\alpha Vd^2/(\pi^2\eta^2)$ and $h=|k|d/\pi$, the growing branch has positive real part exactly when $|D|>2(1+h^2)^2/h$. Differentiation gives $3h^4+2h^2-1=0$, hence $h=1/\sqrt3$. Equality is a neutral oscillation, not exponential growth. The sign of $D$ reverses wave propagation without changing the growth threshold.

##### Alpha-squared Omega dynamo threshold

↑ **Parent:** [Alpha-Omega dynamo](#alpha-omega-dynamo)

For constant coefficients and a transverse wavenumber $\ell\ne0$, a planar [mean-field dynamo](#mean-field-dynamo) retaining both alpha feedback and shear has dispersion $(\sigma+\eta p)^2=\alpha^2p+i\alpha\Omega k$, $p=k^2+\ell^2$. Marginal stability gives $\alpha_m^2=4\eta^4p^4/(4\eta^2p^3+\Omega^2k^2)$. Differentiate with respect to $k^2$: an interior minimum solves $4\eta^2p^3+\Omega^2(3k^2-\ell^2)=0$. Its derivative with respect to $k^2$ is positive, so a unique positive minimizing $k^2$ exists only above the displayed shear threshold. Below it the minimum is at $k=0$. The sign of the marginal oscillation frequency is fixed by $2\eta p\omega=\alpha\Omega k$.

##### Bounded-modulation alpha-Omega growth estimate

↑ **Parent:** [Alpha-Omega dynamo](#alpha-omega-dynamo)

In the two-component [alpha-Omega dynamo](#alpha-omega-dynamo) with $|f(t)|\leq1$, apply the [weighted energy estimate for two coupled modes](linear-ordinary-differential-equation.md#weighted-energy-estimate-for-two-coupled-modes) with $a=|\alpha_0|$, $c=|k\Omega|$, and $d=\eta k^2$. The field-amplitude growth rate is at most $\sqrt{|\alpha_0\Omega k|}-\eta k^2$. Optimizing over $k$ gives the upper constant $3/2^{8/3}$ multiplying $(\alpha_0^2\Omega^2/\eta)^{1/3}$. The admissible choice $f=1$ gives a lower constant $3/2^{10/3}$, so the maximum possible growth has the displayed scaling. An arbitrary chosen modulation need not grow. The statement concerns the model with freely adjustable wavenumber; physical scale-separation restrictions can constrain that optimization.

#### Omega effect

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

Differential rotation or shear stretches a [poloidal magnetic field](magnetohydrodynamics.md#poloidal-magnetic-field) into a [toroidal magnetic field](magnetohydrodynamics.md#toroidal-magnetic-field). This is the Omega effect. By itself it need not regenerate the poloidal component; the [alpha effect](#alpha-effect) provides one possible feedback mechanism in an [alpha-Omega dynamo](#alpha-omega-dynamo). Without feedback, shear amplification can be transient or algebraic rather than sustained exponential [dynamo action](#dynamo-action).

#### First-order smoothing approximation

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

First-order smoothing neglects the fluctuating nonlinear velocity-magnetic-field product in the fluctuation [resistive induction equation](#resistive-induction-equation), but retains $\langle\mathbf u\times\mathbf b\rangle$ in the [mean-field electromotive force](#mean-field-electromotive-force). For a constant test field it gives $\partial_t\mathbf b-\eta\nabla^2\mathbf b=(\mathbf B_0\cdot\nabla)\mathbf u$. Its validity requires the omitted terms to be small compared with the retained forcing and diffusion terms.

##### Isotropic alpha effect of three helical traveling waves

↑ **Parent:** [First-order smoothing approximation](#first-order-smoothing-approximation)

Three equal-amplitude transverse waves along orthogonal axes, with the same [circular polarization](electromagnetic-wave.md#circular-polarization), each satisfy $\nabla\times\mathbf u_j=\sigma k\mathbf u_j$, $\sigma=\pm1$. Distinct spatial phases have zero cross averages. The periodic [first-order smoothing](#first-order-smoothing-approximation) response to a uniform test field satisfies $(\partial_t-\eta\Delta)\mathbf b_j=(\overline{\mathbf B}\cdot\nabla)\mathbf u_j$. Writing $a=\eta k^2$, the response is $\mathbf b_j=k\overline B_j[a\partial_\phi\mathbf u_j-\Omega\mathbf u_j]/(a^2+\Omega^2)$. Since $\mathbf u_j\times\partial_\phi\mathbf u_j=-\sigma U^2\mathbf e_j$, summing yields the displayed isotropic [alpha effect](#alpha-effect). It includes the resistive and temporal weighting absent from an unqualified instantaneous helicity rule.

##### Helicity formula for isotropic first-order smoothing

↑ **Parent:** [First-order smoothing approximation](#first-order-smoothing-approximation)

For a locally uniform mean [magnetic field](magnetic-field.md), [first-order smoothing](#first-order-smoothing-approximation) solves $\partial_t\mathbf b-\eta\Delta\mathbf b=(\overline{\mathbf B}\cdot\nabla)\mathbf u$. Inserting its causal diffusion propagator into the [mean-field electromotive force](#mean-field-electromotive-force) and taking the [trace](linear-algebra.md#matrix-trace) of the isotropic response tensor gives the displayed relation to [kinetic helicity](vorticity.md#hydrodynamical-helicity). When diffusion during a [correlation time](time-series.md#correlation-time) is negligible, it reduces to $\alpha=-\tau_H\langle\mathbf u\cdot\nabla\times\mathbf u\rangle/3$. At small [magnetic Reynolds number](magnetohydrodynamics.md#magnetic-reynolds-number), a quasistatic monochromatic velocity instead gives $\alpha=-\langle\mathbf u\cdot\nabla\times\mathbf u\rangle/(3\eta k_0^2)$. The effective [correlation time](time-series.md#correlation-time) and diffusion weighting should not be silently discarded.

##### Quasistatic magnetic response of a helical shearing wave

↑ **Parent:** [First-order smoothing approximation](#first-order-smoothing-approximation)

For background shear $\Omega y\widehat{\mathbf x}$ and uniform field $B_0\widehat{\mathbf x}$, [first-order smoothing](#first-order-smoothing-approximation) gives the magnetic shearing-wave amplitude equation

$$
\dot{\mathbf c}=\Omega c_y\widehat{\mathbf x}+ik_xB_0\mathbf v-\eta K^2\mathbf c.
$$

If magnetic relaxation is fast compared with shear, $c_y,c_z\simeq ik_xB_0(v_y,v_z)/(\eta K^2)$ after free transients decay. Thus the doubled Fourier-mode electromotive quantity $\mathcal E=\operatorname{Re}(v_yc_z^*-v_zc_y^*)$ is $-B_0H/(\eta K^2)$, where $H=ik_x(v_yv_z^*-v_zv_y^*)$. The spatially averaged [mean-field electromotive force](#mean-field-electromotive-force) of real waves has an extra factor $1/2$. Using the [helicity invariant of an inviscid shearing wave](gravitational-instability-of-an-astrophysical-disk.md#helicity-invariant-of-an-inviscid-shearing-wave), and assuming the approximation holds uniformly in time with $\Omega k_x\ne0$, gives

$$
\int_{-\infty}^{\infty}\mathcal E\,dt\simeq-\frac{\pi B_0H(0)}{2\eta|\Omega k_x|\sqrt{k_x^2+k_z^2}}.
$$

Indeed $K^2=A+\Omega^2k_x^2t^2$, $A=k_x^2+k_z^2$, and substitution $z=|\Omega k_x|t/\sqrt A$ uses $\int_{-\infty}^{\infty}(1+z^2)^{-2}dz=\pi/2$.

##### Monochromatic coupled magnetic and velocity response

↑ **Parent:** [First-order smoothing approximation](#first-order-smoothing-approximation)

For a steady forced [Fourier mode](fourier-analysis.md#fourier-mode) with $|\mathbf q|=k$, coupled viscous and magnetic response gives $\widehat{\mathbf u}=[\eta k^2\widehat{\mathbf f}+i(\mathbf B\cdot\mathbf q)\widehat{\mathbf g}/(\mu_0\rho)]/D$ and $\widehat{\mathbf b}=[\nu k^2\widehat{\mathbf g}+i(\mathbf B\cdot\mathbf q)\widehat{\mathbf f}]/D$. Their [mean-field electromotive force](#mean-field-electromotive-force) contains both forcing helicities and a possible weighted cross-forcing correlation. Jointly isotropic forcing removes the latter; its vanishing at zero mean field alone is insufficient for anisotropic forcing.

##### Oscillatory magnetic response in first-order smoothing

↑ **Parent:** [First-order smoothing approximation](#first-order-smoothing-approximation)

For a velocity [Fourier mode](fourier-analysis.md#fourier-mode) with wavenumber $k$, define $a=\eta k^2$, $d=a^2+\Omega^2$ and $\mathbf C=i(\mathbf B_0\cdot\mathbf k)\hat{\mathbf u}$. A cosine-forced mode has periodic response coefficients $(\mathbf p,\mathbf q)=(a\mathbf C,\Omega\mathbf C)/d$, while a sine-forced mode has $(-\Omega\mathbf C,a\mathbf C)/d$. Homogeneous transients decay as $e^{-at}$. The periodic response is a particular solution, not arbitrary initial data.

#### Parker dynamo wave

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

A Parker dynamo wave is a traveling or oscillatory mode of a mean-field dynamo coupling poloidal and toroidal magnetic-field components through an [alpha effect](#alpha-effect) and shear. A reduced complex-amplitude model can represent fluctuating alpha by a time-dependent coupling. Its periodically switched growth must be calculated from the [monodromy matrix of a periodic linear system](differential-equation.md#monodromy-matrix-of-a-periodic-linear-system), rather than by averaging noncommuting generators.

##### Local alpha-Omega dynamo wave dispersion

↑ **Parent:** [Parker dynamo wave](#parker-dynamo-wave)

Take a right-handed local Cartesian frame with $x$ towards the equator, $y$ azimuthal and $z$ radially outwards in the northern hemisphere. A local radial shear $U_y=Sz$ and a [poloidal magnetic field](magnetohydrodynamics.md#poloidal-magnetic-field) represented by $A\widehat{\mathbf y}$ give the [alpha-Omega dynamo](#alpha-omega-dynamo) equations $A_t=\alpha B+\eta_T A_{xx}$ and $B_t=S A_x+\eta_T B_{xx}$. Substitution of a [Fourier mode](fourier-analysis.md#fourier-mode) proportional to $e^{pt+ikx}$ gives the displayed [dispersion relation](dispersion-relation.md). The growing branch has $\operatorname{Re}p=-\eta_Tk^2+\sqrt{|\alpha Sk|/2}$ and $\operatorname{Im}p=\operatorname{sgn}(\alpha Sk)\sqrt{|\alpha Sk|/2}$. Its phase velocity is $-\operatorname{Im}p/k$: it propagates equatorwards when $\alpha S<0$, polewards when $\alpha S>0$. The result assumes local constant coefficients and no [meridional circulation in a star](stellar-structure.md#meridional-circulation-in-a-star); advection and spatially separated field regeneration can alter migration.

##### Periodically reversing Parker dynamo coupling

↑ **Parent:** [Parker dynamo wave](#parker-dynamo-wave)

For $\dot A=D^2f(t)B$ and $\dot B=iA$, with $f$ alternating between $+1$ and $-1$ for intervals of length $T$, the [monodromy matrix of a periodic linear system](differential-equation.md#monodromy-matrix-of-a-periodic-linear-system) has determinant one and trace $\cosh(\sqrt2DT)+\cos(\sqrt2DT)>2$. Its reciprocal [Floquet multipliers](dynamical-systems.md#floquet-multiplier) give positive dominant [Floquet growth rate](differential-equation.md#floquet-growth-rate) for $D,T>0$, despite the zero mean of $f$. An exceptional initial state in the stable [eigenspace](linear-operator-theory.md#eigenspace) decays.

#### Alpha effect

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

The alpha effect is the part of a [mean-field electromotive force](#mean-field-electromotive-force) linear in the mean [magnetic field](magnetic-field.md) itself, $\boldsymbol{\mathcal E}=\boldsymbol\alpha\overline{\mathbf B}+\cdots$. The [alpha tensor](#alpha-tensor) can be anisotropic; it need not be a scalar multiple of the identity. Its [curl](multivariable-calculus.md#curl) can couple transverse mean-field components and produce an [alpha-squared dynamo](#alpha-squared-dynamo).

##### Rapidly fluctuating alpha effect

↑ **Parent:** [Alpha effect](#alpha-effect)

In a [Parker dynamo wave](#parker-dynamo-wave) model, an [alpha effect](#alpha-effect) of the form $\alpha=\epsilon^{-1}\alpha_0\sin(\omega t/\epsilon)$ has zero time average but can generate a finite averaged coupling. The [method of multiple scales](singular-perturbation.md#method-of-multiple-scales) gives $\widetilde A=-(\alpha_0/\omega)\cos(\omega\tau)\overline B$ and $\widetilde B=-(\Omega\alpha_0/\omega^2)\sin(\omega\tau)\partial_x\overline B$, where $\tau=t/\epsilon$. Consequently $C=\Omega\alpha_0^2/(2\omega^2)$. With diffusion operator $\partial_x^2-\ell^2$, the averaged [Fourier mode](fourier-analysis.md#fourier-mode) growth exponents are $-k^2-\ell^2\pm|k|\sqrt{\Omega C}$. For freely adjustable real $k$, growth requires $\Omega C>4\ell^2$. The result is an asymptotic averaged model for fixed nonzero $\omega$, not an exact replacement at finite $\epsilon$.

##### Strong-field quenching of an isotropic electromotive force

↑ **Parent:** [Alpha effect](#alpha-effect)

For isotropic monochromatic forcing, the longitudinal coefficient in a [mean-field electromotive force](#mean-field-electromotive-force) is proportional to $\int_0^1\mu^2(1+h^2\mu^2)^{-2}d\mu=[\arctan h-h/(1+h^2)]/(2h^3)$, where $h$ is proportional to mean-field strength. This gives generic $|B|^{-3}$ quenching. The natural angular [alpha tensor](#alpha-tensor) is anisotropic in a nonzero mean field: its transverse coefficient instead contains $\int_0^1(1-\mu^2)(1+h^2\mu^2)^{-2}d\mu$ and scales as $|B|^{-1}$. Only the longitudinal contraction enters $\boldsymbol{\mathcal E}=\boldsymbol\alpha\mathbf B$. An effective scalar representation may therefore have every diagonal entry equal to the longitudinal coefficient without being the unique natural response tensor.

##### Alpha-squared dynamo

↑ **Parent:** [Alpha effect](#alpha-effect)

An alpha-squared dynamo generates a mean [magnetic field](magnetic-field.md) using an [alpha effect](#alpha-effect) without requiring an additional large-scale shear coupling. For $\boldsymbol\alpha=\alpha_0\operatorname{diag}(1,1,0)$ and a transverse mean field varying as $e^{iKz}$, the growth rates are $-\eta K^2\pm\alpha_0K$. A nonzero $\alpha_0$ therefore allows growth for sufficiently long wavelengths, provided the domain and scale separation permit them.

###### Homogeneous alpha-squared dynamo growth criterion

↑ **Parent:** [Alpha-squared dynamo](#alpha-squared-dynamo)

For constant isotropic transport coefficients and zero mean flow, a divergence-free [Fourier mode](fourier-analysis.md#fourier-mode) has two [circular polarizations](electromagnetic-wave.md#circular-polarization) that diagonalize [curl](multivariable-calculus.md#curl) with eigenvalues $\pm k$. The mean induction equation therefore has the displayed [growth rates](dispersion-relation.md#growth-rate). Growth requires an admissible $k$ with $|\alpha|>(\eta+\beta)k$. Freely variable wavenumber gives $k_*=|\alpha|/[2(\eta+\beta)]$, provided it respects mean-field scale separation. A uniform field has zero [curl](multivariable-calculus.md#curl) and cannot grow by constant alpha alone; boundaries fix the longest available spatial mode.

###### Anisotropic alpha-squared dynamo

↑ **Parent:** [Alpha-squared dynamo](#alpha-squared-dynamo)

An [alpha-squared dynamo](#alpha-squared-dynamo) may use a tensorial [alpha effect](#alpha-effect) rather than an isotropic coefficient. For constant [alpha tensor](#alpha-tensor) $\boldsymbol\alpha$ and [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity) $\eta>0$, a steady nonzero [Fourier mode](fourier-analysis.md#fourier-mode) with wavevector $\mathbf K$ satisfies $\eta K^2\mathbf B=i\mathbf K\times(\boldsymbol\alpha\mathbf B)$ and $\mathbf K\cdot\mathbf B=0$. Anisotropy can change both the critical alpha magnitude and the preferred wavevector direction.

###### Uniaxial alpha dynamo threshold

↑ **Parent:** [Anisotropic alpha-squared dynamo](#anisotropic-alpha-squared-dynamo)

For $\boldsymbol\alpha=\operatorname{diag}(\alpha_0,\alpha_0,\alpha_1)$, set $\gamma=\alpha_0/\eta$, $\delta=\alpha_1/\alpha_0$, and $q^2=k^2+l^2$. A steady nonzero [Fourier mode](fourier-analysis.md#fourier-mode) obeys the displayed condition when the denominator is nonzero. At fixed $q>0$ and $0<\delta<1$, minimizing over $m^2\geq0$ gives $m_*^2=(1-2\delta)q^2$ and $\gamma_{\min}^2=4(1-\delta)q^2$ for $\delta<1/2$; for $\delta\geq1/2$ it gives $m_*^2=0$ and $\gamma_{\min}^2=q^2/\delta$. This is a boundary-constrained threshold of an [anisotropic alpha-squared dynamo](#anisotropic-alpha-squared-dynamo).

##### Alpha tensor

↑ **Parent:** [Alpha effect](#alpha-effect)

The alpha tensor is the linear map from a uniform test [magnetic field](magnetic-field.md) to the corresponding [mean-field electromotive force](#mean-field-electromotive-force). Its components satisfy $\mathcal E_i=\alpha_{ij}B_{0j}$. Anisotropic helical flows can produce a real symmetric rank-two response, such as $\alpha_0\operatorname{diag}(1,1,0)$.

#### Mean-field electromotive force

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

The mean-field electromotive force is the vector correlation $\boldsymbol{\mathcal E}=\langle\mathbf u\times\mathbf b\rangle$. Its [curl](multivariable-calculus.md#curl) enters the mean [resistive induction equation](#resistive-induction-equation). It is a local vector with units of velocity times magnetic field, not the scalar circuit voltage called [electromotive force](electric-charge.md#electromotive-force). A [space-time average of periodic modes](#space-time-average-of-periodic-modes) is often used to measure its transport coefficients.

##### Monochromatic small-Reynolds-number mean electromotive force

↑ **Parent:** [Mean-field electromotive force](#mean-field-electromotive-force)

Suppose a steady [solenoidal](multivariable-calculus.md#solenoidal-vector-field) velocity satisfies $\Delta\mathbf u=-\mathbf u$, and spatial averaging permits [integration by parts](calculus.md#integration-by-parts) without boundary terms. For a uniform test [magnetic field](magnetic-field.md) $\mathbf B$, the small-[magnetic Reynolds number](magnetohydrodynamics.md#magnetic-reynolds-number) expansion gives $\mathbf b_1=(\mathbf B\cdot\nabla)\mathbf u$ and $\Delta\mathbf b_2=-\nabla\times(\mathbf u\times\mathbf b_1)$. Using the [self-adjointness](linear-operator-theory.md#self-adjoint-operator) of the [Laplacian](multivariable-calculus.md#laplacian) inside the average,

$$
\mathcal E^{(1)}=\langle\mathbf u\times(\mathbf B\cdot\nabla)\mathbf u\rangle,\qquad
\mathcal E^{(2)}=\langle\mathbf u\times\nabla\times[\mathbf u\times(\mathbf B\cdot\nabla)\mathbf u]\rangle.
$$

The second equality concerns the averaged [mean-field electromotive force](#mean-field-electromotive-force); it does not assert that the quadratic forcing itself is monochromatic.

// Target: fluid-mechanics.bigb

###### Antisymmetry of the second-order monochromatic alpha tensor

↑ **Parent:** [Monochromatic small-Reynolds-number mean electromotive force](#monochromatic-small-reynolds-number-mean-electromotive-force)

For $\mathbf C=\mathbf u\times(\mathbf B\cdot\nabla)\mathbf u$, the [cross product](vector-space.md#cross-product) identity $(\mathbf u\times\nabla\times\mathbf C)_i=u_j\partial_iC_j-u_j\partial_jC_i$ and [integration by parts](calculus.md#integration-by-parts) give $\mathcal E^{(2)}_i=-\langle\partial_i u_jC_j\rangle$. Its [alpha tensor](#alpha-tensor) is

$$
\alpha^{(2)}_{ij}=-\langle\partial_i\mathbf u\cdot(\mathbf u\times\partial_j\mathbf u)\rangle
=\langle\mathbf u\cdot(\partial_i\mathbf u\times\partial_j\mathbf u)\rangle.
$$

Interchanging $i,j$ reverses the [cross product](vector-space.md#cross-product), showing that the coefficient is an [antisymmetric matrix](linear-algebra.md#skew-symmetric-matrix). Such a coefficient represents a [turbulent magnetic pumping](#turbulent-magnetic-pumping) contribution rather than the symmetric part of the [alpha effect](#alpha-effect).

// Target: fluid-mechanics.bigb

###### Symmetry of the first-order monochromatic alpha tensor

↑ **Parent:** [Monochromatic small-Reynolds-number mean electromotive force](#monochromatic-small-reynolds-number-mean-electromotive-force)

The first coefficient of the [alpha tensor](#alpha-tensor) is $\alpha^{(1)}_{ij}=\epsilon_{ikl}\langle u_k\partial_j u_l\rangle$. Its contraction with the [Levi-Civita symbol](multivariable-calculus.md#levi-civita-symbol) is

$$
\epsilon_{pij}\alpha^{(1)}_{ij}=\langle u_j\partial_j u_p-u_p\partial_j u_j\rangle=0,
$$

by [incompressibility](fluid-mechanics.md#incompressible-flow) and vanishing averages of total derivatives. Every [antisymmetric second-rank tensor](multilinear-algebra.md#antisymmetric-second-rank-tensor) in three dimensions is detected by this contraction, so the coefficient is a [symmetric matrix](linear-algebra.md#symmetric-matrix). The proof needs no [Fourier analysis](fourier-analysis.md).

// Target: fluid-mechanics.bigb

##### Turbulent magnetic pumping

↑ **Parent:** [Mean-field electromotive force](#mean-field-electromotive-force)

[Turbulent magnetic pumping](#turbulent-magnetic-pumping) is an effective transport of the mean [magnetic field](magnetic-field.md) produced by correlations in inhomogeneous or anisotropic turbulence. Its contribution to the [mean-field electromotive force](#mean-field-electromotive-force) is $\boldsymbol{\mathcal E}_{\rm pump}=\boldsymbol\gamma\times\overline{\mathbf B}$. In the mean induction equation this enters as $\nabla\times(\boldsymbol\gamma\times\overline{\mathbf B})$, the same algebraic form as [advection](fluid-mechanics.md#advection) by a [velocity](classical-mechanics.md#velocity) $\boldsymbol\gamma$. Thus it supplements the mean material [velocity](classical-mechanics.md#velocity) without requiring an equal mean mass flow. Downward pumping can help retain or couple fields in a [solar dynamo](stellar-astrophysics.md#solar-dynamo).

##### Integrated electromotive response of a finite cyclonic event

↑ **Parent:** [Mean-field electromotive force](#mean-field-electromotive-force)

For the [ideal magnetic response to a cylindrical cyclonic event](ideal-magnetohydrodynamics.md#ideal-magnetic-response-to-a-cylindrical-cyclonic-event), the plane-integrated $x$-component of $\mathbf u\times\mathbf B$ at duration $t$ is

$$
\mathcal E_x(t)=\pi B_0\int_0^\infty\left[t r^2(fg'-gf')\cos(ft)-2rg\sin(ft)\right]dr.
$$

This follows from $(\mathbf u\times\mathbf B)_x=(rfB_z+gA_r)\cos\phi-(g/r)A_\phi\sin\phi$ and azimuthal integration. If boundary terms vanish, integration by parts gives the equivalent form $\pi B_0\int_0^\infty r^2g'[\sin(ft)+tf\cos(ft)]dr$. For $f=g=a^2-r^2$ on $r<a$, zero outside, the response is

$$
\mathcal E_x(t)=\pi B_0a^4\frac{x\cos x-\sin x}{x^2},\qquad x=a^2t.
$$

The value at zero is its continuous limit zero. It is initially $-\pi B_0a^6t/3$, but changes sign repeatedly at the nonzero roots of $\tan x=x$, with oscillatory envelope of order $t^{-1}$. The flow's [kinetic helicity density](vorticity.md#kinetic-helicity-density) is $2f^2\geq0$, showing that the sign of a finite-duration ideal response is not fixed by the instantaneous helicity sign.

##### Space-time average of periodic modes

↑ **Parent:** [Mean-field electromotive force](#mean-field-electromotive-force)

A space-time average over periodic modes integrates over the spatial periodic cell and one temporal period. For real spatial [Fourier modes](fourier-analysis.md#fourier-mode) sharing a [wavevector](elasticity-physics.md#wavevector), $\langle\operatorname{Re}(\mathbf v e^{i\mathbf k\cdot\mathbf x})\times\operatorname{Re}(\mathbf w e^{i\mathbf k\cdot\mathbf x})\rangle_x=\operatorname{Re}(\mathbf v^*\times\mathbf w)/2$. A matching sine or cosine temporal factor supplies another $1/2$. Opposite wavevectors can have nonzero spatial cross averages, so their temporal coefficients must be checked rather than discarded merely because the wavevectors are distinct.

## Hartmann flow

↑ **Parent:** [Resistive magnetohydrodynamics](resistive-magnetohydrodynamics.md)

Hartmann flow is a fully developed viscous conducting-fluid flow driven along a planar channel while a uniform [magnetic field](magnetic-field.md) crosses the walls. Induction and the [Lorentz force density](relativistic-electromagnetism.md#lorentz-force-density) couple its velocity and tangential induced field. For no-slip, normal-field walls separated by $2L$, the velocity is a [hyperbolic cosine](calculus.md#hyperbolic-cosine) profile that approaches [plane Poiseuille flow](viscous-fluid-flow.md#plane-poiseuille-flow) at zero imposed field and develops a uniform core with [Hartmann layers](#hartmann-layer) at large [Hartmann number](#hartmann-number).

### Hartmann flow rate with normal-field walls

↑ **Parent:** [Hartmann flow](#hartmann-flow)

For a streamwise pressure gradient $-\rho G$ and walls at $z=\pm L$ with zero tangential [magnetic field](magnetic-field.md), the [volumetric flow rate](fluid-mechanics.md#volumetric-flow-rate) per unit span is

$$
Q(H)=\frac{2GL^3}{\nu}\frac{H\coth H-1}{H^2}.
$$

Its zero-field value is $2GL^3/(3\nu)$; it decreases strictly for $H>0$ and is asymptotic to $2GL^3/(\nu H)$. The [partial-fraction expansion of the hyperbolic cotangent](calculus.md#partial-fraction-expansion-of-the-hyperbolic-cotangent) proves monotonicity directly.

### Hartmann layer

↑ **Parent:** [Hartmann flow](#hartmann-flow)

A Hartmann layer is the thin viscous-magnetic [boundary layer](continuum-mechanics.md#boundary-layer) next to a wall crossed by the applied [magnetic field](magnetic-field.md). For channel half-width $L$ and large [Hartmann number](#hartmann-number) $H$, its thickness is $\delta\sim L/H=\sqrt{\mu_0\rho\nu\eta}/|B_0|$. It restores the [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition) and the specified magnetic wall condition outside the nearly uniform [Hartmann flow](#hartmann-flow) core.

### Hartmann number

↑ **Parent:** [Hartmann flow](#hartmann-flow)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hartmann_number)

The Hartmann number measures the strength of magnetic coupling relative to viscous and resistive effects in a channel:

$$
H=\frac{|B_0|L}{\sqrt{\mu_0\rho\nu\eta}}=|B_0|L\sqrt{\frac{\sigma_c}{\rho\nu}}.
$$

Here $L$ is the channel half-width, $\nu$ the [kinematic viscosity](dynamic-viscosity.md#kinematic-viscosity), $\eta$ the [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity) and $\sigma_c$ the [electrical conductivity](electric-charge.md#electrical-conductivity). In [Hartmann flow](#hartmann-flow), large $H$ produces thin magnetic-viscous wall layers and a flatter, slower core for fixed [pressure gradient](fluid-mechanics.md#pressure-gradient).

## Normal magnetic field boundary condition

↑ **Parent:** [Resistive magnetohydrodynamics](resistive-magnetohydrodynamics.md)

A normal-field wall imposes zero tangential [magnetic field](magnetic-field.md): $\mathbf B\times\mathbf n=0$ for the wall [unit normal](differential-geometry.md#unit-normal) $\mathbf n$. In a channel with imposed normal field $B_0\hat{\mathbf z}$, an induced tangential component $b(z)\hat{\mathbf x}$ therefore satisfies $b=0$ on each wall. This condition is distinct from the [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition) on fluid velocity.

## Resistive induction equation

↑ **Parent:** [Resistive magnetohydrodynamics](resistive-magnetohydrodynamics.md)

For a [solenoidal vector field](multivariable-calculus.md#solenoidal-vector-field) $\mathbf B$ and constant [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity) $\eta$, the magnetic induction equation is

$$
\partial_t\mathbf B=\nabla\times(\mathbf u\times\mathbf B)+\eta\nabla^2\mathbf B,\qquad \nabla\cdot\mathbf B=0.
$$

It combines [Faraday's law](maxwell-equations.md#faraday-s-law-of-induction) with the moving-conductor relation for [electrical conductivity](electric-charge.md#electrical-conductivity), neglecting displacement current. With [incompressible flow](fluid-mechanics.md#incompressible-flow), its advective form is $\partial_t\mathbf B+(\mathbf u\cdot\nabla)\mathbf B=(\mathbf B\cdot\nabla)\mathbf u+\eta\nabla^2\mathbf B$.

### Conductivity-gradient term in magnetic induction

↑ **Parent:** [Resistive induction equation](#resistive-induction-equation)

For scalar [electrical conductivity](electric-charge.md#electrical-conductivity) $\sigma(\mathbf x)$ and constant permeability $\mu_0$, the moving-fluid Ohm law and the quasistatic [Ampere-Maxwell law](maxwell-equations.md#ampere-s-circuital-law) give $\mathbf E=-\mathbf u\times\mathbf B+\eta\nabla\times\mathbf B$, where $\eta=1/(\mu_0\sigma)$ is the [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity). Taking minus the [curl](multivariable-calculus.md#curl) and using [Faraday's law of induction](maxwell-equations.md#faraday-s-law-of-induction) gives $\partial_t\mathbf B=\nabla\times(\mathbf u\times\mathbf B)-\nabla\times(\eta\nabla\times\mathbf B)$. Expanding this expression and imposing $\nabla\cdot\mathbf B=0$ yields the title equation. The familiar constant-diffusivity [resistive induction equation](#resistive-induction-equation) omits the last term because $\nabla\eta=0$; nonrelativistic motion alone does not establish that simplification.

### Shearing-coordinate magnetic flux equation

↑ **Parent:** [Resistive induction equation](#resistive-induction-equation)

For a planar [magnetic field](magnetic-field.md) written as $\mathbf B=\nabla\times(A\widehat{\mathbf z})$ and a circular [velocity](classical-mechanics.md#velocity) $\mathbf u=s\Omega(s)\widehat{\boldsymbol\phi}$, the [resistive induction equation](#resistive-induction-equation) reduces, after choosing the additive [gauge transformation](electromagnetism.md#gauge-transformation), to $\partial_tA+\Omega\partial_\phi A=\eta\nabla^2A$. A [Fourier mode](fourier-analysis.md#fourier-mode) $A=a(s,t)e^{im[\phi-\Omega(s)t]}$ therefore obeys the equation in the title. Indeed, each radial [derivative](calculus.md#derivative) acting on the exponential replaces $\partial_s$ by $\partial_s-imt\Omega'$, while the azimuthal [Laplacian](multivariable-calculus.md#laplacian) contributes $-m^2/s^2$. At zero [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity), $a$ is constant in time, but the physical [magnetic field](magnetic-field.md) can still be amplified algebraically by [differential rotation](astrophysical-fluid-dynamics.md#differential-rotation).

### Radial magnetic induction scalar

↑ **Parent:** [Resistive induction equation](#resistive-induction-equation)

For [solenoidal](multivariable-calculus.md#solenoidal-vector-field) velocity and [magnetic field](magnetic-field.md), with constant [magnetic diffusivity](magnetohydrodynamics.md#magnetic-diffusivity) $\eta$, the [resistive induction equation](#resistive-induction-equation) implies

$$
\partial_tP+\mathbf u\cdot\nabla P=\mathbf B\cdot\nabla Q+\eta\Delta P,\qquad Q=\mathbf u\cdot\mathbf x.
$$

The [product rule](calculus.md#product-rule) gives $D_tP=\mathbf x\cdot D_t\mathbf B+\mathbf u\cdot\mathbf B$ and $\Delta P=\mathbf x\cdot\Delta\mathbf B+2\nabla\cdot\mathbf B$. Consequently the radial velocity, through $Q$, is the source term for the radial [magnetic field](magnetic-field.md).

// Target: fluid-mechanics.bigb

#### Insulating boundary condition for the radial magnetic scalar

↑ **Parent:** [Radial magnetic induction scalar](#radial-magnetic-induction-scalar)

At a spherical interface with an insulating exterior, equal [magnetic permeability](maxwell-equations.md#permeability-electromagnetism) on both sides and no surface current, all components of the [magnetic field](magnetic-field.md) are continuous. The [solenoidal magnetic-field constraint](magnetic-field.md#solenoidal-magnetic-field-constraint) then makes $P=\mathbf B\cdot\mathbf x$ and $\partial_rP$ continuous. A current-free exterior has $\Delta P=0$. For an isolated field decaying at infinity, its degree-$l$ [spherical harmonic](analysis.md#spherical-harmonic) satisfies $\partial_rP_{lm}=-(l+1)P_{lm}/a$ at a sphere of radius $a$. This [boundary condition](differential-equation.md#boundary-condition) incorporates the exterior field without setting the radial field to zero.

// Target: fluid-mechanics.bigb

## ↑ Ancestors (6)

1. [Magnetohydrodynamics](magnetohydrodynamics.md)
2. [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)
3. [Fluid mechanics](fluid-mechanics.md)
4. [Branches of physics](physics.md#branches-of-physics)
5. [Physics](physics.md)
6. [Codex Wiki](README.md)
