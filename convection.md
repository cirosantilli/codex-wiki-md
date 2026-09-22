# Convection

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convection)

Convection transports properties such as [energy](energy.md) or composition through bulk fluid motion. [Thermal convection](#thermal-convection) is driven by temperature-dependent [buoyancy](fluid-mechanics.md#buoyancy).

**Table of contents**

- [Convection cell](#convection-cell)
- [Convection zone](#convection-zone)
- [Compositional convection](#compositional-convection)
- [Long-wave convection equation with broken Boussinesq symmetry](#long-wave-convection-equation-with-broken-boussinesq-symmetry)
  - [Second-harmonic feedback in a long-wave convection amplitude equation](#second-harmonic-feedback-in-a-long-wave-convection-amplitude-equation)
  - [Energy square completion for long-wave convection](#energy-square-completion-for-long-wave-convection)
- [Thermal convection](#thermal-convection)
  - [Horizontal convection](#horizontal-convection)
    - [Shallow horizontal convection with an insulated bottom](#shallow-horizontal-convection-with-an-insulated-bottom)
      - [Advection correction in shallow horizontal convection](#advection-correction-in-shallow-horizontal-convection)
  - [Forced convection](#forced-convection)
  - [Natural convection](#natural-convection)
    - [Free-convection surface-layer scaling](#free-convection-surface-layer-scaling)
  - [Hexagonal convection amplitude equations](#hexagonal-convection-amplitude-equations)
    - [Rotational hexagon amplitude equations](#rotational-hexagon-amplitude-equations)
      - [Roll and hexagon spectra without reflection symmetry](#roll-and-hexagon-spectra-without-reflection-symmetry)
      - [Axial isotropy of rolls and hexagons](#axial-isotropy-of-rolls-and-hexagons)
    - [Roll instability from broken up-down symmetry](#roll-instability-from-broken-up-down-symmetry)
  - [Convection roll](#convection-roll)
  - [Oscillatory convection](#oscillatory-convection)
    - [Travelling and standing convection rolls](#travelling-and-standing-convection-rolls)
  - [Stationary convection](#stationary-convection)
  - [Convective stability](#convective-stability)
  - [Convective overshoot](#convective-overshoot)
  - [Double-diffusive convection](#double-diffusive-convection)
    - [Thermosolutal convection](#thermosolutal-convection)
      - [Double-diffusive overflow reservoir](#double-diffusive-overflow-reservoir)
        - [Post-shutdown double-diffusive reservoir cooling](#post-shutdown-double-diffusive-reservoir-cooling)
      - [Lorenz model of thermosolutal convection](#lorenz-model-of-thermosolutal-convection)
        - [Oscillatory threshold of a thermosolutal Lorenz model](#oscillatory-threshold-of-a-thermosolutal-lorenz-model)
        - [Steady fold of a thermosolutal Lorenz model](#steady-fold-of-a-thermosolutal-lorenz-model)
    - [Layered convection](#layered-convection)

## Convection cell

↑ **Parent:** [Convection](convection.md)

An organized region of buoyant rising fluid and compensating descending flow that transports heat or composition. [Convection rolls](#convection-roll) are a simple planar example; [solar granules](stellar-astrophysics.md#solar-granule) are evolving compressible examples. A cellular pattern does not require every material trajectory to form a closed streamline, especially near a radiating free surface.

## Convection zone

↑ **Parent:** [Convection](convection.md)

A stellar [convection zone](#convection-zone) is a region where buoyant fluid motion transports a significant part of the stellar heat flux. Rising and sinking parcels carry enthalpy, so heat transport is not entirely radiative. The [Sun](stellar-astrophysics.md#sun)'s outer [convection zone](#convection-zone) extends from near $0.7R_\odot$ to the surface and overlies its radiative interior. The [tachocline](stellar-astrophysics.md#tachocline) lies near this transition, and the [convection](convection.md) helps power the [solar dynamo](stellar-astrophysics.md#solar-dynamo).

## Compositional convection

↑ **Parent:** [Convection](convection.md)

Compositional convection is buoyancy-driven motion caused by composition-dependent density variations. In a planetary core, freezing can expel light elements into the surrounding liquid, making that liquid buoyant and supplying mechanical power for a [planetary dynamo](planetary-science.md#planetary-dynamo). It can operate alongside thermally driven [convection](convection.md) and release of [latent heat](thermodynamic-potential.md#latent-heat).

## Long-wave convection equation with broken Boussinesq symmetry

↑ **Parent:** [Convection](convection.md)

A reduced long-wave [convection](convection.md) model can combine linear damping, destabilizing second derivatives, stabilizing fourth derivatives and gradient nonlinearities. In the displayed normalization the quadratic coefficient $s$ breaks [Boussinesq symmetry](geophysical-fluid-dynamics.md#boussinesq-up-down-symmetry), while the cubic gradient term dissipates the mean-square temperature. The linear [dispersion relation](dispersion-relation.md) is $\lambda(k)=-1+\mu k^2-k^4$, with critical [wavenumber](wave-equation.md#wavenumber) $k=1$ at $\mu=2$. Smoothness and spatial averaging hypotheses must be specified before applying the [energy method](numerical-analysis.md#energy-method) on an infinite interval.

### Second-harmonic feedback in a long-wave convection amplitude equation

↑ **Parent:** [Long-wave convection equation with broken Boussinesq symmetry](#long-wave-convection-equation-with-broken-boussinesq-symmetry)

In a [weakly nonlinear expansion](singular-perturbation.md#weakly-nonlinear-expansion) of the [long-wave convection equation with broken Boussinesq symmetry](#long-wave-convection-equation-with-broken-boussinesq-symmetry) at $\mu=2$, a critical [Fourier mode](fourier-analysis.md#fourier-mode) $\Theta_1=Ae^{ix}+\mathrm{c.c.}$ generates $\Theta_2=(2is/9)A^2e^{2ix}+\mathrm{c.c.}$. The quadratic interaction of these first and second harmonics feeds back $8s^2|A|^2A/9$ into the critical [Fourier mode](fourier-analysis.md#fourier-mode), while the cubic gradient nonlinearity contributes $-3|A|^2A$. The [Fredholm solvability condition](sturm-liouville-theory.md#fredholm-solvability-condition) is consequently $\mu_2A-g|A|^2A=0$. The sign of $g$ distinguishes supercritical and subcritical branches; $g=0$ requires a higher-order [amplitude equation](bifurcation-theory.md#amplitude-equation).

### Energy square completion for long-wave convection

↑ **Parent:** [Long-wave convection equation with broken Boussinesq symmetry](#long-wave-convection-equation-with-broken-boussinesq-symmetry)

For a real smooth solution of the [long-wave convection equation with broken Boussinesq symmetry](#long-wave-convection-equation-with-broken-boussinesq-symmetry), assume a periodic spatial average or an existing long-interval average with vanishing endpoint fluxes. [Integration by parts](calculus.md#integration-by-parts) gives the exact [energy method](numerical-analysis.md#energy-method) identity

$$
\frac12\partial_t\langle\Theta^2\rangle
=-\langle(\Theta+\Theta_{xx})^2\rangle
-\langle\Theta_x^2(\Theta_x-s/2)^2\rangle
+(\mu-2+s^2/4)\langle\Theta_x^2\rangle.
$$

Thus $\mu<\mu_E$ prevents growth of the mean-square temperature at arbitrary amplitude in this averaging class. This sufficient nonlinear bound need not equal the linear instability threshold, and it does not imply pointwise monotonicity of the temperature.

## Thermal convection

↑ **Parent:** [Convection](convection.md)

Thermal convection is fluid motion driven by temperature-dependent [buoyancy](fluid-mechanics.md#buoyancy). It transports [heat](heat.md) by bulk motion in addition to [thermal conduction](heat.md#thermal-conduction).

### Horizontal convection

↑ **Parent:** [Thermal convection](#thermal-convection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Horizontal_convection)

Horizontal convection is [buoyancy](fluid-mechanics.md#buoyancy)-driven circulation forced by lateral variations of [temperature](temperature.md) along one horizontal boundary. Hot and cold surface regions drive a circulation even though all thermal forcing is applied at the same height. An insulated bottom and sides require zero net heat exchange through the remaining surface in steady state, but permit heat to enter its warmer region and leave its colder region.

#### Shallow horizontal convection with an insulated bottom

↑ **Parent:** [Horizontal convection](#horizontal-convection)

For downward depth $z=\epsilon y$, take $(u,w)=(\psi_z,-\psi_x)$, surface temperature $T=x$, a flat impermeable stress-free upper boundary and a no-slip insulated bottom. In the steady infinite-[Prandtl number](heat.md#prandtl-number) thin-layer interior, $\psi_{zzzz}=-\operatorname{Ra}$ with $\psi=\psi_{zz}=0$ at the surface and $\psi=\psi_z=0$ at the bottom. The displayed profile follows. Sidewall end layers close the circulation; the interior profile must not be imposed unchanged at those walls.

##### Advection correction in shallow horizontal convection

↑ **Parent:** [Shallow horizontal convection with an insulated bottom](#shallow-horizontal-convection-with-an-insulated-bottom)

The interior first temperature correction obeys $\Theta_{zz}=u=\psi_z$, $\Theta(0)=0$ and $\Theta_z(\epsilon)=0$. Hence $\Theta_z=\psi$, which integrates to the displayed polynomial. Its contribution to depth-integrated horizontal advective [heat flux](heat.md#heat-flux-density) is $\int u\Theta\,dz=-\int\psi^2dz=-19\operatorname{Ra}^2\epsilon^9/1451520$. The leading conductive flux is $-\epsilon$. These statements apply away from the sidewall end layers at fixed Rayleigh number as the layer becomes shallow.

### Forced convection

↑ **Parent:** [Thermal convection](#thermal-convection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Forced_convection)

Heat-carrying fluid motion dominated by an externally imposed flow or shear. Buoyancy may still influence it; forced and free contributions can coexist. In surface-layer scaling, $z\ll|\ell_O|$ is predominantly shear-driven, while $z\gg|\ell_O|$ is predominantly buoyancy-driven for lower-boundary heating.

### Natural convection

↑ **Parent:** [Thermal convection](#thermal-convection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Natural_convection)

Convection driven primarily by buoyancy generated by heating or cooling, rather than an externally imposed mean flow. In a constant-flux unstable surface layer, the local speed scales as $(B_0z)^{1/3}$.

#### Free-convection surface-layer scaling

↑ **Parent:** [Natural convection](#natural-convection)

For a positive approximately constant [vertical turbulent buoyancy flux](turbulence.md#vertical-turbulent-buoyancy-flux), dimensional turnover scaling gives $K_b\sim B_0^{1/3}z^{4/3}$ and $N^2\sim-B_0^{2/3}z^{-4/3}$. The negative squared frequency describes unstable overturning, not a real restoring oscillation. The leading dissipation is height-independent, unlike neutral wall turbulence.

### Hexagonal convection amplitude equations

↑ **Parent:** [Thermal convection](#thermal-convection)

A finite-[wavenumber](wave-equation.md#wavenumber) convection instability with a [resonant three-wave triad](singular-perturbation.md#resonant-three-wave-triad) can yield three coupled [amplitude equations](bifurcation-theory.md#amplitude-equation). For the gradient nonlinearity $\nabla\cdot(|\nabla\Theta|^2\nabla\Theta)$ and weak quadratic asymmetry $-\epsilon\gamma\nabla\cdot(\Theta\nabla\Theta)$, projection onto a triad of length squared $K$ gives the stated equation and its cyclic copies. The quadratic coefficient is $+\gamma K$, while both self and cross cubic coefficients are $-3K^2$ for angles of $120$ degrees. The finite critical mode requires positive linear damping in the underlying long-wave equation.

#### Rotational hexagon amplitude equations

↑ **Parent:** [Hexagonal convection amplitude equations](#hexagonal-convection-amplitude-equations)

For a [resonant three-wave triad](singular-perturbation.md#resonant-three-wave-triad) with rotational and translational [symmetry](physics.md#symmetry-physics) but no spatial [reflection](linear-algebra.md#reflection-mathematics), the cubic [amplitude equations](bifurcation-theory.md#amplitude-equation) have the cyclic form $\dot A=\mu A+\overline B\,\overline C-\nu_1|A|^2A-(\nu_2+\delta)|B|^2A-(\nu_2-\delta)|C|^2A$. A half-turn induces [complex conjugation](complex-analysis.md#complex-conjugation), so all coefficients are real. The coefficient $\delta$ distinguishes the two cyclic cross-couplings that a [reflection](linear-algebra.md#reflection-mathematics) would interchange.

##### Roll and hexagon spectra without reflection symmetry

↑ **Parent:** [Rotational hexagon amplitude equations](#rotational-hexagon-amplitude-equations)

For the [rotational hexagon amplitude equations](#rotational-hexagon-amplitude-equations), put $d=\nu_2-\nu_1$ and $N=\nu_1+2\nu_2$. A roll with $r^2=\mu/\nu_1$ has transverse [eigenvalues](linear-operator-theory.md#eigenvalue) $-dr^2\pm\sqrt{\delta^2r^4+r^2}$, each twice, radial [eigenvalue](linear-operator-theory.md#eigenvalue) $-2\mu$, and one neutral translation. A hexagon with $\mu=Nh^2-h$ has real-amplitude [eigenvalues](linear-operator-theory.md#eigenvalue) $h-2Nh^2$ and $-2h+2dh^2\pm2i\sqrt3\delta h^2$; its imaginary-amplitude [eigenvalues](linear-operator-theory.md#eigenvalue) are $-3h,0,0$. These follow by diagonalizing the cyclic [Jacobian matrix](multivariable-calculus.md#jacobian-matrix). Stability is understood modulo translations. If $\nu_2>\nu_1>0$ and $\delta\ne0$, the upper positive hexagon branch reaches a [Hopf bifurcation](bifurcation-theory.md#hopf-bifurcation) at $h=1/d$, $\mu=(2\nu_1+\nu_2)/d^2$.

##### Axial isotropy of rolls and hexagons

↑ **Parent:** [Rotational hexagon amplitude equations](#rotational-hexagon-amplitude-equations)

Write the translation [group action](group-action.md) as $(A,B,C)\mapsto(e^{i\theta_1}A,e^{i\theta_2}B,e^{-i(\theta_1+\theta_2)}C)$. Modulo lattice translations, the [stabilizer subgroup](group-action.md#stabilizer-subgroup) of $(h,h,h)$, with nonzero real $h$, is the sixfold rotation group. Its [fixed-point subspace of a group action](representation-theory.md#fixed-point-subspace-of-a-group-action) is the real line $(a,a,a)$. The [stabilizer subgroup](group-action.md#stabilizer-subgroup) of $(r,0,0)$, with nonzero real $r$, consists of the circle $\theta_1=0$ together with a half-turn; its [fixed-point subspace of a group action](representation-theory.md#fixed-point-subspace-of-a-group-action) is the real line $(a,0,0)$. The [equivariant branching lemma](dynamical-systems.md#equivariant-branching-lemma) therefore supplies generic branches of both axial types.

#### Roll instability from broken up-down symmetry

↑ **Parent:** [Hexagonal convection amplitude equations](#hexagonal-convection-amplitude-equations)

In the [hexagonal convection amplitude equations](#hexagonal-convection-amplitude-equations), a pure [convection roll](#convection-roll) has $|A|^2=\mu_2/(3K)$ and $B=C=0$. The transverse diagonal linear growth cancels because self and cross cubic coefficients coincide. Broken up-down symmetry leaves the off-diagonal coupling $\gamma K A$, giving eigenvalues $\pm|\gamma|K|A|$ and an unstable orientation perturbation whenever $\gamma\ne0$. With zero quadratic coupling these directions are neutral at the retained order, so that degenerate case cannot be declared strictly unstable by this calculation.

### Convection roll

↑ **Parent:** [Thermal convection](#thermal-convection)

A [convection roll](#convection-roll) is a circulating cell pattern whose ideal [velocity](classical-mechanics.md#velocity) and [temperature](temperature.md) fields are periodic across a chosen horizontal direction and independent of the coordinate along the [convection roll](#convection-roll) axis. In a two-dimensional [stream function](fluid-mechanics.md#stream-function) representation, its [velocity field](fluid-mechanics.md#velocity-field) is $(-\psi_z,0,\psi_x)$. [Rayleigh-Bénard convection](viscous-fluid-flow.md#rayleigh-benard-convection) can select stationary or oscillatory [convection rolls](#convection-roll); a two-dimensional [convection roll](#convection-roll) may be unstable to three-dimensional disturbances, a different [convection roll](#convection-roll) orientation, or slow amplitude and phase modulations. Existence of a saturated [Landau amplitude equation](bifurcation-theory.md#landau-amplitude-equation) branch does not alone establish its stability.

### Oscillatory convection

↑ **Parent:** [Thermal convection](#thermal-convection)

[oscillatory convection](#oscillatory-convection) is time-dependent convection emerging through nonzero-frequency [overstability](dynamical-systems.md#overstability) or a [Hopf bifurcation](bifurcation-theory.md#hopf-bifurcation). At onset a complex-conjugate growth-rate pair crosses the imaginary axis. Travelling and standing [convection rolls](#convection-roll) are distinct nonlinear possibilities, and their stability cannot be decided from the linear [angular frequency](lagrangian-mechanics.md#angular-frequency) alone.

#### Travelling and standing convection rolls

↑ **Parent:** [Oscillatory convection](#oscillatory-convection)

At fixed orientation, opposite travelling amplitudes can obey $\dot Z_\pm=(r+i\omega_0)Z_\pm-(g|Z_\pm|^2+h|Z_\mp|^2)Z_\pm$. For $r>0$ and $g_r=\operatorname{Re}g>0$, a travelling branch has one nonzero intensity $r/g_r$ and is stable to its counter-propagating amplitude when $h_r>g_r$. A standing branch has both intensities $r/(g_r+h_r)$ and is stable within the pair when $g_r>h_r$ and $g_r+h_r>0$. These follow by linearizing the real intensity equations. Spatial modulation and other orientations remain separate stability tests.

### Stationary convection

↑ **Parent:** [Thermal convection](#thermal-convection)

[stationary convection](#stationary-convection) has a time-independent [velocity](classical-mechanics.md#velocity) and [temperature](temperature.md) field, in the chosen fixed frame. Its onset from a conduction state corresponds to a real growth rate passing through zero. Stability of a resulting steady [convection roll](#convection-roll) is a separate nonlinear question.

### Convective stability

↑ **Parent:** [Thermal convection](#thermal-convection)

A stable stratification gives a restoring [buoyancy](fluid-mechanics.md#buoyancy) force and positive squared [buoyancy frequency](gravity-wave.md#buoyancy-frequency) for an adiabatically displaced parcel. An adverse [specific entropy](entropy.md#specific-entropy) gradient can instead drive [convection](convection.md); other forces such as rotation can modify the full stability criterion.

### Convective overshoot

↑ **Parent:** [Thermal convection](#thermal-convection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convective_overshoot)

Convective overshoot carries material from an unstable convecting region into an adjacent stably stratified region because its [momentum](momentum.md) does not vanish at the stability boundary. In stars this mixes material beyond the boundary determined by a local [stellar convective stability](stellar-structure.md#stellar-convective-stability) criterion, changing stellar core masses and nuclear lifetimes.

### Double-diffusive convection

↑ **Parent:** [Thermal convection](#thermal-convection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Double-diffusive_convection)

Double-diffusive convection occurs when two properties, such as [temperature](temperature.md) and composition, affect [buoyancy](fluid-mechanics.md#buoyancy) but diffuse at different rates. A stabilizing composition gradient can oppose a destabilizing thermal gradient and change the form of heat transport.

#### Thermosolutal convection

↑ **Parent:** [Double-diffusive convection](#double-diffusive-convection)

[Thermosolutal convection](#thermosolutal-convection) is [double-diffusive convection](#double-diffusive-convection) driven by temperature and concentration gradients. Their buoyancy contributions can oppose one another, while unequal [thermal diffusivity](heat.md#thermal-diffusivity) and [solutal diffusivity](brownian-motion.md#solutal-diffusivity) allow steady, oscillatory and finite-amplitude states. For a layer heated from below with a stabilizing concentration gradient, thermal buoyancy is destabilizing and solutal buoyancy restoring.

##### Double-diffusive overflow reservoir

↑ **Parent:** [Thermosolutal convection](#thermosolutal-convection)

A steady well-mixed hot salty reservoir receives volume flux $Q$ and loses the same flux over a weir. Heat and salt balances are $Q(T_i-T)=AF_T$ and $Q(S_i-S)=AF_S$. If $\beta F_S/(\alpha F_T)=R_F$ and $\alpha F_T=b(\alpha\Delta T)^{4/3}/R_\rho^2$, define $R_0=\beta(S_i-S_\infty)/[\alpha(T_i-T_\infty)]$. Then $\eta_s=(R_F/R_0)\theta_s$ and $C=Ab[\alpha(T_i-T_\infty)]^{1/3}/(Q R_0^2)$. For $R_0>1$ and $0\leq R_F<1$ the interface is statically stable while preferential heat transfer can drive [double-diffusive convection](#double-diffusive-convection).

###### Post-shutdown double-diffusive reservoir cooling

↑ **Parent:** [Double-diffusive overflow reservoir](#double-diffusive-overflow-reservoir)

After inflow and overflow cease, a fixed-volume reservoir initially in the preceding steady state obeys $\eta=q\theta$ and $\dot\theta=k(1-\theta)^{10/3}/(1-q\theta)^2$, with $k=Ab[\alpha(T_i-T_\infty)]^{1/3}/(V R_0^2)$. Integrating gives $k(t-t_0)=G(\theta)-G(\theta_s)$, where $G=3(1-q)^2(1-\theta)^{-7/3}/7+3q(1-q)(1-\theta)^{-4/3}/2+3q^2(1-\theta)^{-1/3}$. For $q<1$, heat contrast tends to zero only at infinite time, while a nonzero salt contrast remains.

##### Lorenz model of thermosolutal convection

↑ **Parent:** [Thermosolutal convection](#thermosolutal-convection)

A five-mode [Galerkin method](partial-differential-equation.md#galerkin-method) model retains the roll velocity $a$, its correlated temperature and concentration modes $b,d$, and the mean-profile distortions $c,e$. Its parameters include the [Prandtl number](heat.md#prandtl-number) $\sigma$, diffusivity ratio $\tau$, thermal forcing $r$, stabilizing solutal forcing $r_s$, and a positive geometric decay ratio $\varpi$. The velocity equation is $\dot a=\sigma(-a+rb-r_sd)$, while the scalar equations are $\dot b=-b+a(1-c)$, $\dot c=\varpi(-c+ab)$, $\dot d=-\tau d+a(1-e)$ and $\dot e=\varpi(-\tau e+ad)$. The solutal forcing is normalized using the thermal diffusion scale, so its steady stabilizing effect is $r_s/\tau$.

###### Oscillatory threshold of a thermosolutal Lorenz model

↑ **Parent:** [Lorenz model of thermosolutal convection](#lorenz-model-of-thermosolutal-convection)

Linearization of the [Lorenz model of thermosolutal convection](#lorenz-model-of-thermosolutal-convection) at conduction yields $(\lambda+\sigma)(\lambda+1)(\lambda+\tau)-\sigma r(\lambda+\tau)+\sigma r_s(\lambda+1)=0$. A [Hopf bifurcation](bifurcation-theory.md#hopf-bifurcation) requires the cubic coefficient identity $a_3=a_1a_2$ and positive frequency squared. Its threshold is the stated $r_H$, with $\omega^2=\sigma r_s(1-\tau)/(\sigma+1)-\tau^2>0$. If $r_s=\beta^2\tau$ and $\delta=\sigma/(1+\sigma)$, then $r_H=1+\tau/\delta+\beta^2\tau\delta+O(\tau^2)$. Comparing with the [steady fold of a thermosolutal Lorenz model](#steady-fold-of-a-thermosolutal-lorenz-model) gives a leading nonnegative difference $\tau(\beta\delta-1)^2/\delta$ for $\beta\ge0$.

###### Steady fold of a thermosolutal Lorenz model

↑ **Parent:** [Lorenz model of thermosolutal convection](#lorenz-model-of-thermosolutal-convection)

A nonzero steady [Lorenz model of thermosolutal convection](#lorenz-model-of-thermosolutal-convection) branch obeys $r(x)=(1+x)+r_s\tau(1+x)/(\tau^2+x)$, with $x=a^2$. For $0<\tau<1$, it has an interior [saddle-node bifurcation](bifurcation-theory.md#saddle-node-bifurcation) precisely when $r_s>\tau^3/(1-\tau^2)$. Differentiating gives $x_*=-\tau^2+\sqrt{r_s\tau(1-\tau^2)}$ and the stated minimum. The weaker-versus-stronger threshold distinction matters: a sufficient bound need not be the sharp subcriticality condition. Steady-branch existence alone does not decide oscillatory stability.

#### Layered convection

↑ **Parent:** [Double-diffusive convection](#double-diffusive-convection)

Layered convection consists of mixed convecting layers separated by more weakly transporting interfaces. In a giant planet, composition gradients can support such interfaces and reduce heat loss, contributing to [delayed cooling of an inflated giant planet](exoplanet.md#delayed-cooling-of-an-inflated-giant-planet).

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (88)

- [Boundary layer turbulence by Massachusetts Institute of Technology](physics-bibliography.md#boundary-layer-turbulence-by-massachusetts-institute-of-technology)
- [Boussinesq up-down symmetry](geophysical-fluid-dynamics.md#boussinesq-up-down-symmetry)
- [Climate model](geophysics.md#climate-model)
- [Comparing surface emission at equal temperature](heat.md#comparing-surface-emission-at-equal-temperature)
- [Compositional convection](#compositional-convection)
- [Convection zone](#convection-zone)
- [Convective adjustment](geophysics.md#convective-adjustment)
- [Convective envelope](stellar-structure.md#convective-envelope)
- [Convective instability of a square-root exponential atmospheric profile](exoplanet.md#convective-instability-of-a-square-root-exponential-atmospheric-profile)
- [Convective stability](#convective-stability)
- [Cooling-controlled planetary envelope growth](planetary-science.md#cooling-controlled-planetary-envelope-growth)
- [Deep radiative boundary beneath a power-law-opacity convective envelope](stellar-structure.md#deep-radiative-boundary-beneath-a-power-law-opacity-convective-envelope)
- [Delayed cooling of an inflated giant planet](exoplanet.md#delayed-cooling-of-an-inflated-giant-planet)
- [Electrolyte](electrochemistry.md#electrolyte)
- [Fully convective star](stellar-structure.md#fully-convective-star)
- [Geodynamo](planetary-science.md#geodynamo)
- [Heat transfer](heat.md#heat-transfer)
- [Infrared](optics.md#infrared)
- [Long-wave convection equation with broken Boussinesq symmetry](#long-wave-convection-equation-with-broken-boussinesq-symmetry)
- [Magnetic flux separation](magnetohydrodynamics.md#magnetic-flux-separation)
- [Magnetoconvection](magnetohydrodynamics.md#magnetoconvection)
- [Meridional circulation in a star](stellar-structure.md#meridional-circulation-in-a-star)
- [Net radiative heat exchange](heat.md#net-radiative-heat-exchange)
- [Nondiffusive convective angular momentum transport](turbulence.md#nondiffusive-convective-angular-momentum-transport)
- [Oil drop charge readout and calibration](electric-charge.md#oil-drop-charge-readout-and-calibration)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-4.md#51/a/i/solution)
- [Solution](past-exam-of-the-exoplanets-and-planetary-systems-course-of-the-university-of-cambridge/2015/paper-1.md#1/solution)
- [Solution](past-exam-of-the-exoplanets-and-planetary-systems-course-of-the-university-of-cambridge/2015/paper-1.md#2/solution)
- [Solution](past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2016/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-35.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-38.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-38.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-43.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-43.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-63.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-63.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-62.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-70.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-76.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-66.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-68.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-74.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-67.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-63.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-63.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-55.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-59.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-59.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-59.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-59.md#4/g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-315.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-315.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-315.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-332.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#1/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#1/a/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#2/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#4/h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-317.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-337.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-315.md#2/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-315.md#2/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-315.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-317.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-321.md#2/d/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2010/paper-2.md#section-d/d12/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-1.md#section-d/d13/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1.md#section-d/d13/b/solution)
- [Solution](past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2012/paper-1.md#1/b/solution)
- [Solution](past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2012/paper-1.md#1/c/solution)
- [Solution](past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2013/paper-1.md#2/a/solution)
- [Peltier current-reversal experiment](thermoelectric-effect.md#peltier-current-reversal-experiment)
- [Perfectly conducting thermal boundary condition](differential-equation.md#perfectly-conducting-thermal-boundary-condition)
- [Planetary dynamo](planetary-science.md#planetary-dynamo)
- [Planetary stratosphere](exoplanet.md#planetary-stratosphere)
- [Planetary troposphere](exoplanet.md#planetary-troposphere)
- [Power-law opacity radiative envelope](stellar-structure.md#power-law-opacity-radiative-envelope)
- [Radiative-convective climate column](geophysics.md#radiative-convective-climate-column)
- [Radiative core](stellar-structure.md#radiative-core)
- [Radius sensitivity in the Perrin sedimentation experiment](brownian-motion.md#radius-sensitivity-in-the-perrin-sedimentation-experiment)
- [Stefan–Boltzmann law](heat.md#stefan-boltzmann-law)
- [Stellar activity Rossby number](geophysical-fluid-dynamics.md#stellar-activity-rossby-number)
- [Stellar rotation-activity feedback](stellar-astrophysics.md#stellar-rotation-activity-feedback)
- [Subcritical magnetoconvection](magnetohydrodynamics.md#subcritical-magnetoconvection)
- [Thermal diffusivity](heat.md#thermal-diffusivity)
- [Thermal insulation](heat.md#thermal-insulation)
- [Tropopause](exoplanet.md#tropopause)
