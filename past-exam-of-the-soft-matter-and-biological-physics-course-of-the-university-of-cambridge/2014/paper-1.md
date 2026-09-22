# Paper 1

↑ **Parent:** [2014](../2014.md)

Original paper: [13 January 2014, physical PDF pages 658–660](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=658).

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

[velocity](../../classical-mechanics.md#velocity) $U$, [length](../../physics.md#length) $\ell$ and [diffusivity](../../brownian-motion.md#diffusion-coefficient) $D$ have dimensions $L/T$, $L$, and $L^2/T$. Their dimensionless [Péclet number](../../fluid-mechanics.md#peclet-number) is

$$
\boxed{\mathrm{Pe}=\frac{U\ell}{D}=\frac{\ell^2/D}{\ell/U}.}
$$

[diffusion](../../thermodynamics.md#diffusion) dominates for $\mathrm{Pe}\ll1$, [advection](../../fluid-mechanics.md#advection) for $\mathrm{Pe}\gg1$. At fixed $U,D$, the crossover [length](../../physics.md#length) is $D/U$; neglecting [advection](../../fluid-mechanics.md#advection) requires $\ell\ll D/U$.

TODO: user-deferred organism-specific swimming-speed and detection-scale estimates. No biological numerical substitution is made.

For the generic [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) transport derivation, let an external potential $V(x)$ give [force](../../force.md) $F=-V'$ and drift $u=F/\zeta$. Boltzmann [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) has $c\propto e^{-V/(k_BT)}$, hence $c'=Fc/(k_BT)$. Substituting in the zero-current condition gives

$$
J=Fc\left(\frac1\zeta-\frac{D}{k_BT}\right)=0,
\qquad\boxed{D=\frac{k_BT}{\zeta}=\frac{k_BT}{6\pi\eta a}.}
$$

The [Stokes–Einstein relation](../../stokes-flow.md#stokes-einstein-relation) in the final equality is for an isolated no-slip sphere in a Newtonian liquid at low [Reynolds number](../../dynamic-viscosity.md#reynolds-number). Zero flux alone is insufficient: the [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) distribution and mechanical mobility law are also needed.

TODO: user-deferred organism-specific absorbing-surface calculation and its biological flux interpretation.

TODO: user-deferred receptor-number, receptor-density and receptor-competition calculations. These continuations have not been solved.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Consider generic synthetic filaments and films. [buckling](../../elasticity-physics.md#buckling) occurs when compression makes a transverse deformation lower the energy. For a straight filament of bending rigidity $B=EI$ under compressive [force](../../force.md) $P$,

$$
\delta^2F=\frac12\int_0^L[B(y'')^2-P(y')^2]\,ds.
$$

Pinned ends admit $y=A\sin(\pi s/L)$, giving $\delta^2F=A^2L[B(\pi/L)^4-P(\pi/L)^2]/4$. The first instability is therefore **$P_c=\pi^2B/L^2$**. True clamping raises this to $4\pi^2B/L^2$; a clamped-free rod has $\pi^2B/(4L^2)$. [boundary conditions](../../differential-equation.md#boundary-condition) are part of the threshold, not a minor correction. Above threshold geometric nonlinearities and end constraints determine the buckled amplitude.

For [buckling of a synthetic film](../../elasticity-physics.md#buckling-of-a-synthetic-film), let the bending modulus be $\kappa$ and the isotropic in-plane [tension](../../force.md#tension) be $\sigma$. The small-slope quadratic energy is

$$
F_2=\tfrac12\int[\kappa(\nabla^2h)^2+\sigma|\nabla h|^2]\,dA.
$$

A mode of [wave number](../../wave-equation.md#wavenumber) $q$ has stiffness $\kappa q^4+\sigma q^2$. [tension](../../force.md#tension) stabilizes it; compression corresponds to $\sigma<0$ and makes modes with $q^2<|\sigma|/\kappa$ unstable. A finite sheet has a smallest allowed $q$, giving a finite threshold. A supporting foundation adds positive stiffness and can select a nonzero wrinkle wavelength.

Approaching either threshold softens a fluctuation mode: its thermal variance is proportional to $k_BT$ divided by modal stiffness. The apparent quadratic-theory divergence is rounded by nonlinear geometry, finite size and imperfections. Experimentally vary end shortening or load, measure the transverse profile, and control attachment stiffness and initial curvature. Load control and displacement control need not [trace](../../linear-algebra.md#matrix-trace) the same postbuckling response. Biological applications are outside this generic mechanics note.

<a id="2/a/image-original-pinned-filament-shapes-and-synthetic-film-modal-stiffness-under-tension-and-compression"></a>
![](../../past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2014/paper-1-buckling.png)

**[Figure 1](#2/a/image-original-pinned-filament-shapes-and-synthetic-film-modal-stiffness-under-tension-and-compression). Original pinned-filament shapes and synthetic-film modal stiffness under tension and compression**.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

[single-molecule force spectroscopy](../../molecule.md#single-molecule-force-spectroscopy) measures [force](../../force.md) and extension of an individual tether while controlling position or load. In an atomic-force arrangement, a synthetic chain connects a cantilever probe to a translated substrate. For the [cantilever compliance correction](../../molecule.md#cantilever-compliance-correction), a deflection sensor gives $d$, a calibrated spring constant gives **$F=k_cd$**, and substrate displacement $Z$ gives chain extension $x=Z-d$ after geometric offsets are removed. Additional linkers and instrument compliance must be included if appreciable. Thermal deflection calibration uses $k_c\langle d^2\rangle=k_BT$ only after isolating the cantilever's calibrated thermal contribution.

An optical-tweezers implementation detects a tethered bead's displacement from a calibrated trap centre, with $F=k_{\rm trap}\Delta x$ in the harmonic regime. Detector calibration, drag and trap linearity determine the usable [force](../../force.md) and frequency range. These instruments measure individual [force](../../force.md)–extension curves and distributions; averaging many curves can hide multiple tether populations.

For a synthetic [freely jointed chain](../../mathematical-biology.md#ideal-chain) with [Kuhn length](../../mathematical-biology.md#kuhn-length) $b$,

$$
\frac{x}{L}=\coth\frac{Fb}{k_BT}-\frac{k_BT}{Fb}.
$$

A strongly stretched [worm-like chain](../../mathematical-biology.md#worm-like-chain) instead has $1-x/L\simeq\sqrt{k_BT/(4F\ell_p)}$ before backbone stretching becomes important. Fits can estimate contour and [persistence lengths](../../mathematical-biology.md#persistence-length) only in their appropriate regimes. Hysteresis and pulling-rate dependence test whether an apparent mechanical transition is quasistatic or activated.

Control single versus multiple attachments, subtract nonspecific adhesion, vary pulling [speed](../../classical-mechanics.md#speed), calibrate [temperature](../../temperature.md) and stiffness, and correct drift. A rupture peak is not a universal bond strength independent of loading history. A primary nonbiological example measured individual [polydimethylsiloxane](../../polymer.md#polydimethylsiloxane) chains by atomic-force methods; its flexibility interpretation combines those measurements with molecular calculations.[abstract, synthetic PDMS single-chain mechanics](../../chemistry-bibliography.md#understanding-the-extraordinary-flexibility-of-polydimethylsiloxane-through-single-molecule-mechanics-by-song-lu-and-others)

<a id="2/b/image-original-single-tether-force-measurement-schematic-and-the-instrument-compliance-relation"></a>
![](../../past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2014/paper-1-force-spectroscopy.png)

**[Figure 2](#2/b/image-original-single-tether-force-measurement-schematic-and-the-instrument-compliance-relation). Original single-tether force-measurement schematic and the instrument-compliance relation**.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

TODO: user-deferred biological kinetic mechanism and its biochemical pattern-forming applications. The remainder treats generic two-field reaction-diffusion physics only.

Let $\mathbf u=(u,v)$ obey $\partial_t\mathbf u=\mathbf f(\mathbf u)+\operatorname{diag}(D_u,D_v)\nabla^2\mathbf u$. At a uniform steady state, write its reaction Jacobian as $J=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$. Without [diffusion](../../thermodynamics.md#diffusion) stability requires $a+d<0$ and $\Delta=ad-bc>0$. A Fourier perturbation evolves under $J-q^2\operatorname{diag}(D_u,D_v)$, whose [determinant](../../multilinear-algebra.md#determinant) is

$$
\Delta(q)=\Delta-(D_va+D_ud)q^2+D_uD_vq^4.
$$

Its [trace](../../linear-algebra.md#matrix-trace) becomes more negative with increasing $q$. A stationary diffusion-driven instability therefore requires

$$
\boxed{D_va+D_ud>0,\qquad (D_va+D_ud)^2>4D_uD_v\Delta,}
$$

with an allowed domain mode in the resulting negative-determinant band. Equal [diffusivities](../../brownian-motion.md#diffusion-coefficient) cannot satisfy this while $a+d<0$. The physical mechanism is that transport can destabilize coupled fields even when the local kinetics relaxes a spatially uniform perturbation. Faster [diffusion](../../thermodynamics.md#diffusion) of an inhibitory response is one possible realization.

The selected [wave numbers](../../wave-equation.md#wavenumber) depend on growth rates and boundaries; nonlinear saturation determines the final stripes, spots or other states. Linear instability alone neither supplies a biochemical mechanism nor uniquely predicts a final finite-amplitude pattern.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let the channel [length](../../physics.md#length) be $\ell_c\gg R$ and assume uniform solution conductivity. Its Ohmic resistance scales as $\ell_c/(\sigma R^2)$, whereas access resistance of a reservoir mouth scales as $1/(\sigma R)$. The fraction of voltage in the entrance regions is therefore of order $R/\ell_c$. Most of the potential drop lies inside the long channel; the small entrance field region is neglected in the model, not asserted identically zero.

Write $x$ for inserted contour [length](../../physics.md#length) and choose $qE>0$ to pull the chain inward. The charge already inside feels [force](../../force.md) $qEx$, giving

$$
\boxed{U_{\rm el}(x)=-\tfrac12qEx^2.}
$$

Confinement removes [polymer](../../polymer.md) configurations. In the stiff-chain regime, the [confinement deflection length](../../mathematical-biology.md#confinement-deflection-length) obeys $R^2\sim\lambda^3/\ell_p$, hence $\lambda\sim(R^2\ell_p)^{1/3}$. A free-energy cost of order $k_BT$ per deflection gives a roughly constant resisting [entropic force](../../force.md#entropic-force) $f\sim k_BT/\lambda$. The [insertion barrier of a charged polymer](../../polymer.md#insertion-barrier-of-a-charged-polymer) follows from $F(x)\simeq fx-qEx^2/2$, with an entry maximum at $x_*=f/(qE)$ when that point lies within the insertion interval. Its height is $f^2/(2qE)$. The field supplies work against this confinement [entropy](../../entropy.md).

Put $\zeta_\ell=2\pi\eta/\ln(R/a)$, so $\gamma(x)=\zeta_\ell x$. After capture, neglect the entry barrier, exterior-chain drag and thermal corrections to strong directed motion. Then

$$
\gamma(x)\dot x=qEx,\quad \dot x=\frac{qE}{\zeta_\ell},\qquad
\boxed{\tau_{\rm in}=\frac{\zeta_\ell L_0}{qE}=\frac{\gamma(L_0)}{qE}.}
$$

The [confined-polymer entry and recoil times](../../polymer.md#confined-polymer-entry-and-recoil-times) have different length dependence; this entry graph is linear through the origin. Charge and drag both grow with inserted [length](../../physics.md#length), leaving a constant [velocity](../../classical-mechanics.md#velocity). The same cancellation explains length-independent mobility in an ideal free-draining [electrophoresis](../../physical-chemistry.md#electrophoresis) model. It does not include a capture waiting time or claim that every free-solution chain has identical hydrodynamic drag.

A measured superlinear entry time can arise when exterior-coil drag, [tension](../../force.md#tension) propagation, wall adsorption or nonuniform friction adds [length](../../physics.md#length) dependence absent from this model. For example $\gamma(x)\propto x^p$ with the same $qEx$ drive gives $\tau\propto L_0^p$ for $p>0$. Under the assumptions of [uniform wall charge and polymer entry scaling](../../electrostatics.md#uniform-wall-charge-and-polymer-entry-scaling), a homogeneous thin-double-layer electro-osmotic model adds a length-independent fluid [velocity](../../classical-mechanics.md#velocity) $u_{\rm eo}=-\epsilon\zeta_wE/\eta$. It changes the drift coefficient, not its [length](../../physics.md#length) exponent. This does not rule out charge heterogeneity, adsorption or near-cancellation followed by [diffusion](../../thermodynamics.md#diffusion) in a real channel; those are additional mechanisms.

With the field off, the confinement [entropy](../../entropy.md) drives outward motion. Assuming the constant [force](../../force.md) $f$ and the same local friction,

$$
\zeta_\ell x\dot x=-f,\qquad
\boxed{\tau_{\rm out}=\int_0^{L_0}\frac{\zeta_\ell x}{f}\,dx
=\frac{\gamma(L_0)L_0}{2f}.}
$$

The small final end region lies outside the long-confined-segment approximation but gives only a small correction. Thus ideal insertion scales as $L_0$, while recoil scales as $L_0^2$.

TODO: user-deferred DNA-specific numerical stopping-voltage estimate and its biological parameter-based inference. No biological quantities are evaluated.

For [entropic-trap length separation](../../polymer.md#entropic-trap-length-separation), a reservoir/channel array can repeat length-dependent capture, confinement and relaxation delays, turning them into different mean residence times. The uniform inside-channel drift [speed](../../classical-mechanics.md#speed) derived above is itself [length](../../physics.md#length) independent, so that drift alone cannot separate [lengths](../../physics.md#length). Separation must retain [length](../../physics.md#length) dependence of the barrier or of the capture/recoil dynamics and can be tuned with a forward-biased time-dependent field. For large bulk throughput, pressure-driven [advection](../../fluid-mechanics.md#advection) is preferable to [diffusion](../../thermodynamics.md#diffusion) alone; a [pressure](../../pressure.md) gradient can be combined with electric capture control. In the unobstructed continuum limit $Q=\pi R^4\Delta P/(8\eta\ell_c)$. Excessive driving erases trapping differences, so throughput and resolution compete; the question supplies no geometry or adsorption law selecting a unique optimal drive.

<a id="3/image-original-dimensionless-insertion-barriers-and-the-distinct-insertion-and-recoil-length-scalings"></a>
![](../../past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2014/paper-1-polymer-channel.png)

**[Figure 3](#3/image-original-dimensionless-insertion-barriers-and-the-distinct-insertion-and-recoil-length-scalings). Original dimensionless insertion barriers and the distinct insertion and recoil length scalings**.

## ↑ Ancestors (11)

1. [2014](../2014.md)
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
