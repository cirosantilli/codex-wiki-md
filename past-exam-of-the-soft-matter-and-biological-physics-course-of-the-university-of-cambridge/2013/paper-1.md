# Paper 1

↑ **Parent:** [2013](../2013.md)

Original paper: [Public original, physical PDF pages 567–569](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=567).

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For the generic instrument, [magnetic tweezers](../../electromagnetism.md#magnetic-tweezers) combine a magnetically responsive bead, a controllable [magnetic field gradient](../../magnetic-field.md#magnetic-field-gradient), a tether attached to a fixed support, and optical tracking of bead coordinates. For a fixed [magnetic dipole moment](../../electromagnetism.md#magnetic-dipole-moment), the [force](../../force.md) is $\nabla(\mathbf m\cdot\mathbf B)$; an induced linear isotropic moment instead gives $\mathbf F=V\Delta\chi\nabla B^2/(2\mu_0)$. A uniform [magnetic field](../../magnetic-field.md) can orient an anisotropic bead, but a gradient is needed for translation. Magnet height sets the load, while field rotation can impose [torque](../../momentum.md#torque) if bead orientation is coupled to the field. Tracking uses lateral images and a calibrated axial image/defocus response; a fixed reference removes stage drift. A sufficiently slowly varying gradient approximates a [force clamp](../../molecule.md#force-clamp) over the bead's displacement. TODO: **user-deferred biomolecular implementation**; DNA-specific attachment, preparation and response are not treated.

For [transverse-fluctuation calibration of a tensioned tether](../../electromagnetism.md#transverse-fluctuation-calibration-of-a-tensioned-tether), use an ideal tether of vertical extension $h$ whose endpoint is displaced by small $x,y$. Keeping its [length](../../physics.md#length) fixed to quadratic order lowers its vertical coordinate by $(x^2+y^2)/(2h)$, increasing load potential by $F_z(x^2+y^2)/(2h)$. The [equipartition theorem](../../canonical-ensemble.md#equipartition-theorem) therefore gives

$$
\boxed{F_z=\frac{k_BTh}{\langle\delta x^2\rangle}
=\frac{k_BTh}{\langle\delta y^2\rangle}
=\frac{2k_BTh}{\langle\delta x^2+\delta y^2\rangle}.}
$$

Here fluctuations are about the mean. The height is the effective pendulum [length](../../physics.md#length) of the measured coordinate, not automatically the [polymer contour length](../../polymer.md#polymer-contour-length). The displayed $h$ formula uses the point-endpoint or fixed-bead-orientation idealization; freely rotating large beads can require a bead-radius correction to that lever arm. The [finite-exposure correction to fluctuation force calibration](../../electromagnetism.md#finite-exposure-correction-to-fluctuation-force-calibration) restores variance lost through exposure averaging; ignoring it would overestimate [force](../../force.md); localization noise increases it and would underestimate [force](../../force.md). Drift, wall coupling, finite observation time and magnetic lateral stiffness must be checked. Vertical fluctuations measure longitudinal stiffness and do not obey the same geometrical formula.

For the [stretch and twist coefficients of an elastic filament](../../mathematical-biology.md#stretch-and-twist-coefficients-of-an-elastic-filament), take $s$ as reference contour [length](../../physics.md#length) and $\epsilon$ as local axial [strain](../../continuum-mechanics.md#strain). The three positive quadratic costs represent bending of the tangent, stretching of the material and excess twist about its relaxed orientation. With the paper's coefficient convention,

$$
K_b=k_BTA,\qquad S=k_BTB,\qquad K_t=k_BTC.
$$

$K_b,K_t$ are bending and torsional rigidities with units of [energy](../../energy.md) times [length](../../physics.md#length); $S$ is an axial [force](../../force.md) modulus. Thus $A,C$ have units of [length](../../physics.md#length) and $B$ inverse [length](../../physics.md#length). Positive quadratic forms describe a stable relaxed filament; odd terms vanish when expansion is about its zero-stress, zero-torque reference configuration.

At weak and intermediate [tension](../../force.md#tension), changing thermal bending conformations can extend the filament without appreciably stretching the backbone. Axial [strain](../../continuum-mechanics.md#strain) is $\epsilon\simeq F_z/S$, so material stretching must be included when this is no longer negligible. For a long strongly aligned but nearly inextensible three-dimensional [worm-like chain](../../mathematical-biology.md#worm-like-chain), the thermal extension deficit is approximately $\tfrac12\sqrt{k_BT/(AF_z)}$; stretch adds approximately $F_z/S$ to fractional extension. Twist matters whenever [torque](../../momentum.md#torque) or imposed end rotation is present, at any [tension](../../force.md#tension). A freely swivelling, [torque-free](../../stokes-flow.md#torque-free) tether need not store excess twist. There is no universal force-only threshold for switching on torsional [energy](../../energy.md).

The [circular bending energy of an elastic filament](../../mathematical-biology.md#circular-bending-energy-of-an-elastic-filament) follows because curvature is $1/R$ over contour [length](../../physics.md#length) $2\pi R$. Integrating the bending term gives

$$
\boxed{E_{\rm loop}=\frac{k_BTA}{2R^2}(2\pi R)=\frac{\pi k_BTA}{R}.}
$$

This is bending [energy](../../energy.md) alone: imposed [tension](../../force.md#tension), stretching and twist would add costs. The dimensionless bending action is $(A/2)\int|\partial_s\mathbf t|^2ds$. Its tangent propagator in three dimensions obeys [rotational diffusion](../../thermodynamics.md#rotational-diffusion) on the unit sphere, $\partial_sP=(2A)^{-1}\nabla_{S^2}^2P$. The vector [spherical harmonic](../../analysis.md#spherical-harmonic) has angular [eigenvalue](../../linear-operator-theory.md#eigenvalue) $-2$, giving

$$
\boxed{\langle\mathbf t(s)\cdot\mathbf t(0)\rangle=e^{-s/A}.}
$$

Hence $A$ is the [persistence length](../../mathematical-biology.md#persistence-length) in this three-dimensional convention. A strictly planar filament instead has tangent-correlation [length](../../physics.md#length) $2A$; one cannot infer the factor merely by setting a loop's [energy](../../energy.md) equal to $k_BT$.

TODO: **user-deferred biomolecular applications**. Both enzyme-driven unwinding experiments, their experimental sketches, the requested numerical [force](../../force.md) and plectoneme [radius](../../topology.md#radius), [energy](../../energy.md) loss per turn and enzyme-specific dissipation mechanisms remain unsolved. None of their biomolecular parameters has been used in a calculation.

<a id="1/image-original-generic-magnetic-tether-instrument-and-its-transverse-fluctuation-calibration"></a>
![](../../past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2013/paper-1-generic-magnetic-calibration.png)

**[Figure 1](#1/image-original-generic-magnetic-tether-instrument-and-its-transverse-fluctuation-calibration). Original generic magnetic-tether instrument and its transverse fluctuation calibration**.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use a [force-tilted activation barrier](../../chemical-kinetics.md#force-tilted-activation-barrier) for a generic one-coordinate escape model. A tensile [force](../../force.md) tilts a [free-energy landscape](../../statistical-physics.md#free-energy-landscape) to $G_F(x)=G_0(x)-Fx$. If $x_b$ is the initial [minimum](../../set.md#minimum-of-a-subset-of-a-total-order) and $x_s$ the saddle, define $\Delta x=x_s-x_b>0$ and the zero-force barrier $\Delta G_0^\ddagger=G_0(x_s)-G_0(x_b)$. The relevant activation barrier is measured relative to the initial [minimum](../../set.md#minimum-of-a-subset-of-a-total-order), not an arbitrary absolute transition-state [energy](../../energy.md). To first order in [force](../../force.md),

$$
\Delta G^\ddagger(F)=\Delta G_0^\ddagger-F\Delta x,
\qquad
\boxed{k(F)=k_0e^{F/F_0},\quad F_0=\frac{k_BT}{\Delta x},\quad
k_0=\nu e^{-\Delta G_0^\ddagger/(k_BT)}.}
$$

The attempt prefactor $\nu$ is assumed [force](../../force.md) independent, and the saddle displacement is approximated as constant. This single-barrier approximation need not survive large landscape deformations or a change of escape pathway. TODO: **user-deferred biomolecular implementation**; the protein-specific shear-force arrangement and attachment chemistry are not solved.

For a generic force-ramp measurement, a calibrated [atomic force microscope](../../engineering.md#atomic-force-microscope) [cantilever](../../elasticity-physics.md#cantilever) pulls an attachment while a stage changes separation. [cantilever](../../elasticity-physics.md#cantilever) deflection $d$ gives [force](../../force.md) $k_cd$, and the [cantilever compliance correction](../../molecule.md#cantilever-compliance-correction) subtracts $d$ from imposed separation to give tether extension, with further corrections for other apparatus compliance. A prescribed stage speed does not automatically produce constant [force](../../force.md) loading rate when tether stiffness varies; the assumed $F(t)=ft$ must be measured or controlled. The original schematic below illustrates a generic nonbiological bond/tether geometry. Protein-specific construction is deferred.

The no-rebinding approximation is a physical escape assumption: after the link breaks, separation removes the partners from the capture region before appreciable reassociation. It requires the integrated return/association probability during that separation to be small. If the separated state stays nearby or the [force](../../force.md) is held without separation, setting $k_+=0$ can fail. Under the stipulated approximation, with the link initially intact,

$$
\frac{dp}{dF}=-\frac{k_0}{f}e^{F/F_0}p,
\qquad
\boxed{p(F)=\exp\left[-\frac{k_0F_0}{f}(e^{F/F_0}-1)\right],\quad F\geq0.}
$$

This [survival under a linear force ramp](../../markov-chain.md#survival-under-a-linear-force-ramp) differs from the [probability density](../../wave-function.md#probability-density) for rupture. It starts at one, decreases to zero and shifts to larger [force](../../force.md) as the loading rate increases. For small $F/F_0$, $p\simeq e^{-k_0F/f}$; a slow ramp allows much escape before substantial [force](../../force.md) is reached.

The [median rupture force under a linear ramp](../../markov-chain.md#median-rupture-force-under-a-linear-ramp) satisfies $p=1/2$, giving

$$
\boxed{F_{1/2}=F_0\ln\left(1+\frac{f\ln2}{k_0F_0}\right).}
$$

At high loading rate, the slope of $F_{1/2}$ against $\ln f$ tends to $F_0$; it is not exactly $F_0$ for a slow ramp. Fit the full expression across loading rates to recover $F_0$ and $k_0$. The rupture-force [probability density](../../wave-function.md#probability-density) is $\rho(F)=k(F)p(F)/f$, whose [most probable rupture force under a linear ramp](../../markov-chain.md#most-probable-rupture-force-under-a-linear-ramp) is $F_*=F_0\ln[f/(k_0F_0)]$ if $f>k_0F_0$, and zero otherwise. [median](../../probability-distribution.md#median) and [mode](../../probability-and-statistics.md#mode-statistics) are different observables and must not be interchanged when fitting.

At known [temperature](../../temperature.md), $F_0$ yields the activation distance $\Delta x=k_BT/F_0$; $1/k_0$ gives the zero-force mean lifetime in this exponential model. Absolute barrier height additionally requires the attempt prefactor, and neither equilibrium binding [free energy](../../thermodynamic-potential.md#thermodynamic-free-energy) nor an association rate follows from dissociation-only data. A loading-rate-dependent rupture [force](../../force.md) is a kinetic readout, not an intrinsic equilibrium strength. TODO: **user-deferred biological conclusions**. The protein-specific stability interpretation and cell-adhesion strategy are left unsolved.

<a id="2/image-original-generic-pulling-arrangement-tilted-energy-landscape-and-calculated-survival-under-a-force-ramp"></a>
![](../../past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2013/paper-1-generic-force-ramp.png)

**[Figure 2](#2/image-original-generic-pulling-arrangement-tilted-energy-landscape-and-calculated-survival-under-a-force-ramp). Original generic pulling arrangement, tilted energy landscape and calculated survival under a force ramp**.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

In [gel sieving of synthetic polymers](../../physical-chemistry.md#gel-sieving-of-synthetic-polymers), [gel electrophoresis](../../biology.md#gel-electrophoresis) combines drift under an [electric field](../../electric-field.md) with size- and conformation-dependent obstruction by a porous matrix. In weak-field free solution, [force](../../force.md) balance gives $v=\mu E$ and, in a simple effective-charge/effective-friction model, $\mu=q_{\rm eff}/\zeta$. The [mobility](../../critical-phenomenon.md#order-parameter-mobility) is motion relative to the medium, so fluid motion from [electro-osmosis](../../electrostatics.md#electro-osmosis) must be accounted for separately. This is the operational [mobility](../../critical-phenomenon.md#order-parameter-mobility) convention, not a claim that the bare structural charge is always the effective driving charge.[entry E02024, electrophoretic mobility: migration speed divided by electric field strength](../../chemistry-bibliography.md#iupac-compendium-of-chemical-terminology-fifth-edition-gold-book-by-international-union-of-pure-and-applied-chemistry)

For a chain with [free-draining polymer friction](../../polymer.md#free-draining-polymer-friction) with approximately constant effective [electric charge](../../electric-charge.md) per segment, both charge and friction scale with $N$. The free-solution [mobility](../../critical-phenomenon.md#order-parameter-mobility) can therefore become nearly independent of [length](../../physics.md#length), making size separation poor. A gel adds steric constraints. Coils smaller than the mesh can pass relatively easily; larger coils require deformation and pore-to-pore rearrangement. A schematic weak-sieving law is $\mu(c_g)\simeq\mu(0)e^{-K_rc_g}$, where matrix [concentration](../../mathematical-physics.md#concentration) $c_g$ and retardation coefficient $K_r$ are defined by a calibration; it is not a universal size law.

When a long flexible charged [polymer](../../polymer.md) is confined to a tube of available paths, [reptation](../../polymer.md#reptation) supplies another regime. An additive-friction model gives contour [diffusion](../../thermodynamics.md#diffusion) $D_c\propto N^{-1}$ and renewal time $\tau\sim N^2/D_c\propto N^3$. For ideal large-scale chain statistics, $R^2\propto N$, so centre-of-mass [diffusion](../../thermodynamics.md#diffusion) scales as $N^{-2}$. With total effective driving charge proportional to $N$, weak-field [mobility](../../critical-phenomenon.md#order-parameter-mobility) can then scale as $N^{-1}$. This assumes screened/ideal large-scale conformations and [linear response](../../statistical-physics.md#linear-response-theory); strong-field alignment, trapping and nonideal matrices can alter the scaling.

Operationally, load narrow zones of independently characterized synthetic standards and sample into a controlled gel, apply a known field and detect migration positions after a measured time. Compare with a free-solution measurement, vary matrix [concentration](../../mathematical-physics.md#concentration) and field, and control [temperature](../../temperature.md), [ionic strength](../../mixture.md#ionic-strength), [pH](../../acid-base-chemistry.md#ph) and matrix charge. Larger gel pores or lower matrix [concentration](../../mathematical-physics.md#concentration) usually reduce sieving within a given calibrated material system. Excessive field causes [Joule heating](../../electric-charge.md#joule-heating) and can change conformation and [mobility](../../critical-phenomenon.md#order-parameter-mobility). [adsorption](../../physical-chemistry.md#adsorption) or electro-osmotic drift can mimic a size effect; standards should match charge chemistry and [topology](../../topology.md) as well as nominal mass.

Band centres move as $\mu Et$ while ordinary [diffusion](../../thermodynamics.md#diffusion) gives $\sigma_x^2(t)=\sigma_x^2(0)+2Dt$. Resolution depends on separation of centres relative to band widths, not travel distance alone. A neutral tracer helps identify bulk flow, and multiple [concentrations](../../mathematical-physics.md#concentration) test [adsorption](../../physical-chemistry.md#adsorption) or overloading. **A [mobility](../../critical-phenomenon.md#order-parameter-mobility) or band position does not uniquely determine size without a regime-specific calibration.** TODO: biomolecular examples, sample preparation and biological applications are user deferred; the account here concerns synthetic charged [polymers](../../polymer.md) only.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use SI units, uniform absolute [permittivity](../../permittivity.md) $\varepsilon$ and a neutral bulk reservoir. Local equilibrium of ideal mobile [ions](../../chemistry.md#ion) gives $n_i=n_{i,\infty}e^{-z_ie\psi/(k_BT)}$. Combining their charge with the [Poisson equation](../../partial-differential-equation.md#poisson-s-equation) yields

$$
\boxed{\nabla^2\psi=-\frac1\varepsilon\left[\rho_f+\sum_i z_ie n_{i,\infty}e^{-z_ie\psi/(k_BT)}\right].}
$$

The reference is $\psi=0$ in the bulk. Boundary data specify fixed charge, fixed potential or a surface reaction/[charge regulation](../../electrostatics.md#charge-regulation) law. These are physically different problems. The [mean-field theory](../../statistical-physics.md#mean-field-theory) assumes point [ions](../../chemistry.md#ion), [thermal equilibrium](../../thermal-equilibrium.md) and a continuum [solvent](../../mixture.md#solvent); ion-size packing, dielectric structure and strong electrostatic correlations can invalidate it.

For a symmetric monovalent electrolyte let $n_\infty$ count each sign and define $u=e\psi/(k_BT)$, $\kappa_D^2=2e^2n_\infty/(\varepsilon k_BT)$. Outside fixed sources,

$$
\nabla^2u=\kappa_D^2\sinh u.
$$

For $|u|\ll1$, the Debye-Hückel approximation is $\nabla^2u=\kappa_D^2u$. A planar wall bounding electrolyte in $z>0$ has $\psi=\psi_0e^{-\kappa_Dz}$; assuming zero field on the other side, its charge is $\sigma=\varepsilon\kappa_D\psi_0$. A sphere of [radius](../../topology.md#radius) $a$ and total charge $Q$ instead gives

$$
\psi(r)=\frac{Qe^{-\kappa_D(r-a)}}{4\pi\varepsilon r(1+\kappa_Da)},\qquad r\geq a.
$$

The factors arise from geometry and [boundary conditions](../../differential-equation.md#boundary-condition); planar screening cannot be substituted unchanged for a small sphere. The weak-potential condition must hold where the potential is largest, particularly at the surface.

The [nonlinear planar Poisson-Boltzmann profile](../../electrostatics.md#nonlinear-planar-poisson-boltzmann-profile) is also exactly integrable. Multiply $u''=\kappa_D^2\sinh u$ by $u'$ and use $u,u'\to0$ at infinity:

$$
(u')^2=2\kappa_D^2(\cosh u-1),\qquad
u'=-2\kappa_D\sinh(u/2).
$$

The sign selects a profile decaying to the bulk for either sign of surface potential. Integration gives

$$
\boxed{u(z)=4\operatorname{artanh}\left[\gamma e^{-\kappa_Dz}\right],\qquad
\gamma=\tanh(u_0/4).}
$$

For weak $u_0$ this reduces to the linear solution. Strong surface potentials have a bounded far-field amplitude $4\gamma$, while the near-wall [ion](../../chemistry.md#ion) [density](../../fluid-mechanics.md#density) still grows strongly. There is no need to permit the negative [ion](../../chemistry.md#ion) [densities](../../fluid-mechanics.md#density) produced by an invalid extrapolation of a linearized [density](../../fluid-mechanics.md#density) formula.

The same first integral yields the [Grahame equation](../../electrostatics.md#grahame-equation) and its [diffuse-layer differential capacitance](../../electrostatics.md#diffuse-layer-differential-capacitance) per unit [area](../../differential-geometry.md#surface-area):

$$
\boxed{\sigma=\frac{2\varepsilon\kappa_Dk_BT}{e}\sinh(u_0/2),\qquad
C_D=\frac{d\sigma}{d\psi_0}=\varepsilon\kappa_D\cosh(u_0/2).}
$$

These describe the [diffuse layer](../../electrostatics.md#diffuse-layer). A compact interfacial layer adds a voltage drop and can place its [capacitance](../../electromagnetism.md#capacitance) in series with $C_D$; a measured electrode [capacitance](../../electromagnetism.md#capacitance) need not equal the ideal diffuse contribution.[section VI, printed pp. 470–474, especially equations (31)–(48); diffuse charge and differential versus integral capacitance](../../chemistry-bibliography.md#the-electrical-double-layer-and-the-theory-of-electrocapillarity-by-david-c-grahame)

For comparison, a [planar counterion-only double layer](../../electrostatics.md#planar-counterion-only-double-layer) next to a negative plane has positive [counterions](../../chemistry.md#counterion) and no salt reservoir. Its profile is algebraic:

$$
\psi(z)-\psi(0)=\frac{2k_BT}{e}\ln(1+z/b),\qquad
n(z)=\frac1{2\pi\ell_B(z+b)^2},\qquad
b=\frac{e}{2\pi\ell_B|\sigma|},\quad
\ell_B=\frac{e^2}{4\pi\varepsilon k_BT}.
$$

Integrating $en(z)$ over $z>0$ gives $|\sigma|$, checking charge neutrality. This problem cannot be obtained by putting a finite reservoir [density](../../fluid-mechanics.md#density) into the symmetric-electrolyte answer without changing its [boundary conditions](../../differential-equation.md#boundary-condition).

Applications include screening around synthetic [colloids](../../mixture.md#colloid), diffuse-layer electrode [capacitance](../../electromagnetism.md#capacitance) and [forces](../../force.md) between charged plates. In planar geometry, the bulk-subtracted normal [stress](../../continuum-mechanics.md#stress) is constant:

$$
\Pi=k_BT(n_++n_--2n_\infty)-\frac{\varepsilon E^2}{2}.
$$

At the midpoint of identical plates, symmetry sets $E=0$, so the remaining excess ionic [osmotic pressure](../../cell-membrane.md#osmotic-pressure) determines their repulsion. A comparison with [force](../../force.md) or [capacitance](../../electromagnetism.md#capacitance) measurements should vary salt and surface potential independently, test [charge regulation](../../electrostatics.md#charge-regulation) and [adsorption](../../physical-chemistry.md#adsorption), and distinguish compact-layer effects from failures of diffuse screening. Nonlinear Poisson-Boltzmann theory retains finite-potential Boltzmann populations, but still omits correlations and finite-ion-volume saturation.

<a id="3/b/image-original-linear-and-nonlinear-planar-screening-profiles-and-diffuse-layer-capacitance"></a>
![](../../past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2013/paper-1-planar-screening.png)

**[Figure 3](#3/b/image-original-linear-and-nonlinear-planar-screening-profiles-and-diffuse-layer-capacitance). Original linear and nonlinear planar screening profiles and diffuse-layer capacitance**.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

TODO: **user-deferred organism-specific biology**. The bacterial behaviour, mechanisms, experiments and biological applications are intentionally left unsolved.

## ↑ Ancestors (11)

1. [2013](../2013.md)
2. [Past exam of the soft matter and biological physics course of the University of Cambridge](../../past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge.md)
3. [Soft Matter and Biological Physics course of the University of Cambridge](../../university-of-cambridge.md#soft-matter-and-biological-physics-course-of-the-university-of-cambridge)
4. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
