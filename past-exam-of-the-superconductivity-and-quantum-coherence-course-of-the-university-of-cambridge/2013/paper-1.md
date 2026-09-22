# Paper 1

↑ **Parent:** [2013](../2013.md)

Original public paper: [Physical PDF pages 589–591](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=589). All four optional notes and both long questions are covered.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A neutral [superfluid](../../statistical-physics.md#superfluid) has a complex [order parameter](../../critical-phenomenon.md#order-parameter) whose phase describes coherent particle transport. For a Bose condensate it is represented by a field amplitude; for a paired Fermi superfluid it is a pair amplitude. In a symmetry-breaking description, selecting its phase breaks the global particle-number $U(1)$ symmetry. A common [phase shift](../../wave.md#phase-shift) leaves the [energy](../../energy.md) unchanged, while a phase gradient costs [energy](../../energy.md) and produces [superfluid velocity](../../statistical-physics.md#superfluid-velocity). Long-wavelength phase oscillations give a gapless [Goldstone mode](../../critical-phenomenon.md#goldstone-boson), generally a sound wave when density fluctuations provide the conjugate dynamics. A finite isolated state with exact particle number need not have a nonzero field expectation: the phase-selected language describes the ordered limit and relative-phase coherence.

In a [superconductor](../../superconductivity.md#superconductor), the paired [order parameter](../../critical-phenomenon.md#order-parameter) carries charge of magnitude $2e$ and couples to the [electromagnetic field](../../electromagnetism.md#electromagnetic-field). The meaningful spatial phase combination is $\hbar\nabla\theta-q\mathbf A$, with signed pair charge $q$. [Gauge symmetry](../../relativistic-quantum-field.md#gauge-invariance) is a redundancy, so “breaking local gauge symmetry” is not a literal breaking of a measurable physical symmetry. The gauge-invariant electromagnetic response includes the [Meissner effect](../../magnetic-field.md#meissner-effect) and a finite [London penetration depth](../../magnetic-field.md#london-penetration-depth). Long-range Coulomb [forces](../../force.md) move the would-be neutral phase mode to a plasma scale through the [Anderson-Higgs mechanism in a superconductor](../../superconductivity.md#anderson-higgs-mechanism-in-a-superconductor).

Additional symmetries can be broken by particular pairing states. Conventional isotropic spin-singlet pairing need not break spatial rotations or time reversal. A [d-wave superconductor](../../superconductivity.md#d-wave-superconductor) has a gap transforming nontrivially under crystal symmetries, and some triplet or multicomponent states can also break spin-rotation or time-reversal symmetries. These additional choices are not required by superconductivity itself. A nonzero pairing amplitude, phase coherence and electromagnetic screening describe related but distinct aspects of the ordered state.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In [BCS theory](../../fermi-liquid.md#bcs-theory), pairing mixes an [electron](../../physics.md#electron) state with a hole in its opposite-momentum partner. For a uniform spin-singlet gap, the uniform [Bogoliubov--de Gennes Hamiltonian](../../topological-quantum-matter.md#bogoliubov-de-gennes-hamiltonian) gives the momentum-pair eigenproblem

$$
\begin{pmatrix}\xi_{\mathbf k}&\Delta\\\Delta^*&-\xi_{\mathbf k}\end{pmatrix}
\binom{u_{\mathbf k}}{v_{\mathbf k}}=E_{\mathbf k}\binom{u_{\mathbf k}}{v_{\mathbf k}},\qquad
\boxed{E_{\mathbf k}=\sqrt{\xi_{\mathbf k}^2+|\Delta|^2}.}
$$

Here $\xi_{\mathbf k}=\varepsilon_{\mathbf k}-\mu$. A [fermionic Bogoliubov quasiparticle](../../fermi-liquid.md#fermionic-bogoliubov-quasiparticle) is a coherent particle–hole combination, with

$$
|u_{\mathbf k}|^2=\frac12\left(1+\frac{\xi_{\mathbf k}}{E_{\mathbf k}}\right),\qquad
|v_{\mathbf k}|^2=\frac12\left(1-\frac{\xi_{\mathbf k}}{E_{\mathbf k}}\right).
$$

Far above the [Fermi surface](../../fermi-liquid.md#fermi-surface) the excitation is mostly particle-like; far below it is mostly hole-like; at $\xi_{\mathbf k}=0$ the two weights agree. The transformation preserves the fermionic [canonical anticommutation relations](../../supersymmetric-quantum-mechanics.md#canonical-anticommutation-relations). Its mean-field particle-number mixing does not mean that the full physical theory violates charge conservation.

For a fully gapped isotropic state, the minimum single-quasiparticle [energy](../../energy.md) is $|\Delta|$, while creating a pair of [quasiparticles](../../quantum-mechanics.md#quasiparticle) costs at least $2|\Delta|$. This produces suppressed low-temperature thermal populations, an activated electronic [heat capacity](../../heat.md#heat-capacity) and a gap feature in superconducting tunneling. Gap nodes in an unconventional state instead allow low-energy excitations, changing the [temperature](../../temperature.md) dependence. These fermionic excitations are distinct from collective phase and amplitude oscillations of the paired condensate.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

A neutral superfluid's broken global $U(1)$ phase symmetry produces a [Goldstone mode](../../critical-phenomenon.md#goldstone-boson). Coupling phase to density fluctuations generally gives a long-wavelength [phonon](../../quantum-ideal-gas-statistics.md#phonon) with $E(p)\simeq cp$, rather than the quadratic dispersion of a noninteracting condensate. In a dilute interacting Bose gas, the [Bogoliubov quasiparticle dispersion](../../quantum-ideal-gas-statistics.md#bogoliubov-quasiparticle-dispersion) is

$$
E(p)=\sqrt{\varepsilon_p(\varepsilon_p+2gn)},\qquad
\varepsilon_p=\frac{p^2}{2m},\qquad c=\sqrt{\frac{gn}{m}}.
$$

For a heavy weak obstacle moving at speed $v$, emitting an excitation of [momentum](../../momentum.md) $\mathbf p$ changes the available [energy](../../energy.md) by $E(p)-\mathbf v\cdot\mathbf p$. The [Landau criterion](../../statistical-physics.md#landau-criterion) therefore gives

$$
\boxed{v_L=\inf_{p>0}\frac{E(p)}p.}
$$

The dilute-gas spectrum has $v_L=c$. In liquid helium, a [roton](../../statistical-physics.md#roton) minimum can make the minimum ratio smaller than the sound speed; the slope of a line from the origin tangent to the full dispersion determines the kinematic bound. A neutral paired Fermi superfluid also has a fermionic pair-breaking bound of order $\Delta/p_F$ in weak coupling. The smallest relevant branch bound must be considered. Actual flow can fail earlier through vortex nucleation, surface defects or other instabilities: the excitation-energy criterion is not a complete dynamical guarantee of dissipation-free flow.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

In weak-coupling conventional [superconductivity](../../superconductivity.md), a useful guide is $k_BT_c\sim\hbar\omega_{\rm ph}\exp[-1/\lambda_{\rm eff}]$: an appreciable phonon scale and an effective attraction after Coulomb effects are favorable. A large [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) at the [Fermi level](../../quantum-ideal-gas-statistics.md#fermi-level) can strengthen pairing, while light constituent masses can raise relevant phonon frequencies. Increasing [electron](../../physics.md#electron)–phonon coupling without limit is not a general strategy: lattice instabilities, competing order and changes to the phonon spectrum constrain it, and stronger coupling requires treatment beyond the simple exponential expression.

For unconventional high-temperature superconductivity, strong electronic interactions and magnetic fluctuations can support sign-changing pairing, as in [d-wave superconductivity](../../superconductivity.md#d-wave-superconductivity). Layered structures and proximity to magnetic order may enhance useful correlations, but can also promote competing insulating or density-wave states. Sufficient mobile-carrier [phase stiffness](../../critical-phenomenon.md#phase-stiffness) is needed to turn pairing into coherent superconductivity; strong pairing alone does not guarantee a large transition [temperature](../../temperature.md). Disorder that is relatively harmless to an isotropic conventional pair state can be pair-breaking for sign-changing gaps. There is no universal recipe established by these qualitative conditions: the pairing interaction, symmetry, carrier density, competing phases and phase coherence must all be considered.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

In three dimensions an ideal Bose gas can saturate its excited-state population at [chemical potential](../../chemical-potential.md) zero, with the remaining particles forming a [Bose-Einstein condensate](../../quantum-ideal-gas-statistics.md#bose-einstein-condensate). The transition follows from the [Bose-Einstein distribution](../../quantum-ideal-gas-statistics.md#bose-einstein-distribution) integrated against its [density of states](../../quantum-ideal-gas-statistics.md#density-of-states); below the ideal-gas transition, $n_0/n=1-(T/T_c)^{3/2}$. Condensation alone does not supply the finite [Landau critical velocity](../../statistical-physics.md#landau-critical-velocity) of an interacting superfluid: the ideal quadratic spectrum has $\inf_pE(p)/p=0$.

By contrast, a weak attractive interaction near a [Fermi surface](../../fermi-liquid.md#fermi-surface) produces the Cooper instability and the [BCS gap equation](../../fermi-liquid.md#bcs-gap-equation). Its logarithmic enhancement permits pairing at arbitrarily weak attraction in the ideal model. The low-temperature excitations have $E=\sqrt{\xi^2+\Delta^2}$, and in weak coupling $k_BT_c=(e^{\gamma_E}/\pi)\Delta(0)\simeq0.567\Delta(0)$. This transition is controlled by pair formation when phase fluctuations are small; deeply bound pairs instead motivate a Bose-condensation description with their own density and effective [mass](../../classical-mechanics.md#mass).

For the given ellipsoidal dispersion, set $q_x=k_x$, $q_y=k_y$ and $q_z=k_z/\sqrt\gamma$. Then $\varepsilon=\hbar^2q^2/(2m)$ while the integration measure is $d^3k=\sqrt\gamma\,d^3q$. Thus the [anisotropic ideal-gas density of states](../../quantum-ideal-gas-statistics.md#anisotropic-ideal-gas-density-of-states) per unit [volume](../../geometry-and-topology.md#volume) and per internal state is

$$
\boxed{N(\varepsilon,\gamma)=\sqrt\gamma\,N(\varepsilon)
=\frac{\sqrt\gamma}{4\pi^2}\left(\frac{2m}{\hbar^2}\right)^{3/2}\sqrt\varepsilon.}
$$

The full continuum [momentum](../../momentum.md) range is assumed; this is an anisotropic three-dimensional gas, not yet a discrete stack of two-dimensional bands.

At the Bose transition, substitute $x=\varepsilon/(k_BT)$:

$$
n_B=\frac{\sqrt\gamma}{4\pi^2}\left(\frac{2m}{\hbar^2}\right)^{3/2}(k_BT)^{3/2}
\int_0^\infty\frac{x^{1/2}\,dx}{e^x-1}.
$$

The integral is $\Gamma(3/2)\zeta(3/2)\simeq2.315$. Solving for the [Bose-Einstein condensation temperature for an anisotropic effective mass](../../quantum-ideal-gas-statistics.md#bose-einstein-condensation-temperature-for-an-anisotropic-effective-mass) gives

$$
\boxed{k_BT^{\rm BEC}=\frac{2\pi\hbar^2}{m}\left[\frac{n_B}{\sqrt\gamma\,\zeta(3/2)}\right]^{2/3}
\simeq\frac{3.31\hbar^2n_B^{2/3}}{m\gamma^{1/3}}.}
$$

The heavier $z$-direction effective [mass](../../classical-mechanics.md#mass) increases the available excited-state count and lowers the condensation [temperature](../../temperature.md) at fixed number density.

For a balanced two-spin Fermi gas, let $n_F$ denote total [fermion](../../tensor-product-of-quantum-systems.md#fermion) number density and take $N_s$ to be the [single-spin density of states](../../quantum-ideal-gas-statistics.md#single-spin-density-of-states) used in the conventional gap equation. Counting the filled ellipsoid gives

$$
\varepsilon_F(\gamma)=\frac{\hbar^2}{2m}(3\pi^2n_F)^{2/3}\gamma^{-1/3}
\equiv\varepsilon_{F0}\gamma^{-1/3},
$$



$$
N_s(\varepsilon_F,\gamma)=\frac{m(3\pi^2n_F)^{1/3}}{2\pi^2\hbar^2}\gamma^{1/3}
\equiv N_{s0}\gamma^{1/3}.
$$

If a spin-summed [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) is used instead, the coupling convention in the supplied integral must change accordingly; inserting a factor two into only one side would change the exponent incorrectly.

For $\varepsilon_c\ll\varepsilon_F$, replace the [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) across the interaction window by $N_s(\varepsilon_F,\gamma)$. Writing $\lambda_0=|g|N_{s0}$, the zero-temperature integral becomes

$$
1=\lambda_0\gamma^{1/3}\operatorname{arsinh}\left(\frac{\varepsilon_c}{\Delta}\right),
$$

and therefore

$$
\boxed{\Delta(\gamma)=\frac{\varepsilon_c}{\sinh[1/(\lambda_0\gamma^{1/3})]}
\simeq2\varepsilon_c\exp\left[-\frac1{\lambda_0\gamma^{1/3}}\right].}
$$

The second expression additionally requires $\lambda_0\gamma^{1/3}\ll1$. The explicit density dependence is $\lambda_0=|g|m(3\pi^2n_F)^{1/3}/(2\pi^2\hbar^2)$. This [mass-anisotropy enhancement of a weak-coupling BCS gap](../../fermi-liquid.md#mass-anisotropy-enhancement-of-a-weak-coupling-bcs-gap) initially raises the pairing scale, while the ideal Bose condensation scale decreases as $\gamma^{-1/3}$.

<a id="2/image-formal-anisotropy-dependent-gap-and-bose-scales-with-a-schematic-coherence-limited-transition"></a>
![](../../past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2013/paper-1-anisotropy-scales.png)

**[Figure 1](#2/image-formal-anisotropy-dependent-gap-and-bose-scales-with-a-schematic-coherence-limited-transition). Formal anisotropy-dependent gap and Bose scales, with a schematic coherence-limited transition**.

Large anisotropy weakens transport and coherence in the heavy direction. The separation of [pair formation and phase ordering](../../superconductivity.md#pair-formation-and-phase-ordering) then matters, so a large mean-field gap need not imply a large actual $T_c$. A qualitative sketch has $T_c$ initially rising with the pairing scale and eventually turning down when coherence is the smaller scale. If preformed [fermion](../../tensor-product-of-quantum-systems.md#fermion) pairs behave as [bosons](../../tensor-product-of-quantum-systems.md#boson), use $n_B=n_F/2$ and pair [mass](../../classical-mechanics.md#mass) about $2m$; in this continuum model this gives $k_BT^{\rm BEC}\simeq0.218\varepsilon_{F0}\gamma^{-1/3}$.

The turnover cannot be located reliably by taking the weak-coupling formulas to $\gamma\to\infty$: $\varepsilon_F$ falls, $\lambda_0\gamma^{1/3}$ grows, the narrow-window assumption fails and the pair [chemical potential](../../chemical-potential.md) and [mass](../../classical-mechanics.md#mass) require a self-consistent treatment. The smooth curve in the figure is explicitly an illustrative interpolation of two extrapolated scales, not such a calculation. If actual decoupled two-dimensional layers are approached, ordinary ideal-gas finite-temperature condensation is absent and interacting phase order requires a different analysis, including the [Berezinskii–Kosterlitz–Thouless transition](../../critical-phenomenon.md#berezinskii-kosterlitz-thouless-transition) when appropriate.

The cuprates make the distinction between pairing and phase coherence relevant: they are layered and have anisotropic motion, but their strong correlations, lattice band structure and predominantly [d-wave superconductivity](../../superconductivity.md#d-wave-superconductivity) are outside this attractive continuum $s$-wave model. Anisotropy by itself is therefore not an explanation or quantitative fit of cuprate transition [temperatures](../../temperature.md).

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use a complex pair [order parameter](../../critical-phenomenon.md#order-parameter) $\Psi=|\Psi|e^{i\theta}$ with signed charge $q$, $|q|=2e$. A local isotropic [Ginzburg-Landau theory of superconductivity](../../superconductivity.md#ginzburg-landau-theory-of-superconductivity) has free [energy](../../energy.md)

$$
F=\int d^3x\left[\alpha|\Psi|^2+\frac\beta2|\Psi|^4+
\frac{|(-i\hbar\nabla-q\mathbf A)\Psi|^2}{2m_*}+\frac{B^2}{2\mu_0}\right].
$$

For $\alpha<0$, $\beta>0$, the uniform amplitude is $|\Psi_0|^2=-\alpha/\beta$. Variation gives the static field equation and [supercurrent](../../supersymmetry.md#supercurrent)

$$
\frac{(-i\hbar\nabla-q\mathbf A)^2}{2m_*}\Psi+\alpha\Psi+\beta|\Psi|^2\Psi=0,
\qquad
\mathbf j_s=\frac{q}{m_*}\operatorname{Re}\left[\Psi^*(-i\hbar\nabla-q\mathbf A)\Psi\right].
$$

The [vector potential](../../multivariable-calculus.md#vector-potential) obeys Maxwell's equations, including $\nabla\times\mathbf B=\mu_0(\mathbf j_s+\mathbf j_n)+\mu_0\epsilon_0\partial_t\mathbf E$ and $\nabla\times\mathbf E=-\partial_t\mathbf B$, with $\mathbf B=\nabla\times\mathbf A$ and $\mathbf E=-\nabla\phi-\partial_t\mathbf A$. The static approximation drops the displacement current. A common dissipative near-transition dynamical extension is the [time-dependent Ginzburg-Landau equation](../../superconductivity.md#time-dependent-ginzburg-landau-equation)

$$
\Gamma\left(\partial_t+\frac{iq\phi}{\hbar}\right)\Psi=-\frac{\delta F}{\delta\Psi^*},\qquad\Gamma>0.
$$

It is a phenomenological relaxation law in its applicable regime, not a universal microscopic Schrödinger equation for every superconductor. Its covariant time derivative and the covariant spatial derivative ensure consistent phase and electromagnetic gauge transformations.

The amplitude and screening lengths are

$$
\xi=\frac{\hbar}{\sqrt{2m_*|\alpha|}},\qquad
\lambda=\sqrt{\frac{m_*}{\mu_0q^2|\Psi_0|^2}},\qquad\kappa=\lambda/\xi.
$$

For $\kappa>1/\sqrt2$ the ideal model is type II. An [Abrikosov vortex](../../superconductivity.md#abrikosov-vortex) has a $2\pi n$ phase winding, a core with suppressed $|\Psi|$ of size $\xi$, and circulating screening currents over $\lambda$. Single-valuedness implies [fluxoid and flux quantization in a superconductor](../../quantum-theory.md#fluxoid-and-flux-quantization-in-a-superconductor):

$$
\Phi+\mu_0\lambda^2\oint\mathbf j_s\cdot d\boldsymbol\ell=n\Phi_0,
\qquad\boxed{\Phi_0=\frac{h}{2e}.}
$$

The sign of $n$ depends on the chosen circulation and charge convention. Far from the core, where the contour current term is negligible, each singly wound vortex carries one flux quantum in magnitude.

The equilibrium [lower critical magnetic field](../../superconductivity.md#lower-critical-magnetic-field) marks favorable entry of the first vortex; for $\kappa\gg1$, $\mu_0H_{c1}\simeq[\Phi_0/(4\pi\lambda^2)](\ln\kappa+C)$ with an order-one core correction $C$. The [upper critical magnetic field](../../superconductivity.md#upper-critical-magnetic-field) follows by linearizing the order-parameter equation in the field:

$$
\boxed{\mu_0H_{c2}=\frac{\Phi_0}{2\pi\xi^2}.}
$$

Between these fields lies the superconducting mixed state, often with an [Abrikosov vortex lattice](../../superconductivity.md#abrikosov-vortex-lattice). The ideal equilibrium entry and exit fields need not yield large irreversible loops. [Flux pinning](../../superconductivity.md#flux-pinning) and surface barriers impede vortex motion; field sweeps then retain history-dependent flux and produce [magnetic hysteresis](../../critical-phenomenon.md#magnetic-hysteresis) and dissipative losses.

A [superconducting weak link](../../superconductivity.md#superconducting-weak-link), such as a tunnel junction or narrow constriction, couples the phases of two superconductors. With consistent choices of phase and voltage orientation, the [Josephson effect](../../superconductivity.md#josephson-effect) gives

$$
\boxed{I_s=I_c\sin\delta,\qquad\hbar\dot\delta=2eV,\qquad f_J=\frac{2e|V|}{h}.}
$$

The [Gauge-invariant Josephson phase](../../superconductivity.md#gauge-invariant-josephson-phase) includes the line integral of $\mathbf A$ across the link. A zero voltage can sustain a phase-dependent steady current; a constant nonzero voltage makes that contribution oscillate. Microwave irradiation can lock this oscillation to an applied [frequency](../../wave.md#frequency), giving voltage steps at $V_n=nhf/(2e)$, an experimental test of coherent pair transport rather than an ordinary resistive current law.

A [DC SQUID](../../superconductivity.md#dc-squid) places two weak links in a loop. For identical junction critical currents $I_0$ and negligible self-inductance, flux quantization fixes their relative phase difference to $2\pi\Phi_{\rm ext}/\Phi_0$. Adding the two sinusoidal currents and maximizing over their common phase gives

$$
\boxed{I_{c,\rm SQUID}=2I_0\left|\cos\left(\frac{\pi\Phi_{\rm ext}}{\Phi_0}\right)\right|.}
$$

The flux-periodic response provides sensitive magnetic measurements. Junction asymmetry or appreciable loop inductance changes the ideal contrast and can introduce additional hysteresis; the phase-coherent [interference](../../physical-optics.md#interference-wave-propagation) principle remains. The [Jaklevic Josephson interference experiment](../../superconductivity.md#jaklevic-josephson-interference-experiment) is a motivating experimental realization of this link between a superconducting loop, weak links and [magnetic flux](../../magnetic-field.md#magnetic-flux).

## ↑ Ancestors (11)

1. [2013](../2013.md)
2. [Past exam of the superconductivity and Quantum Coherence course of the University of Cambridge](../../past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge.md)
3. [Superconductivity and Quantum Coherence course of the University of Cambridge](../../university-of-cambridge.md#superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge)
4. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
