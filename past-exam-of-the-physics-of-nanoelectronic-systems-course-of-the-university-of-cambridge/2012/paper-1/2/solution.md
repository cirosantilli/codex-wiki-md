<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [Landau quasiparticle](../../../../landau-quasiparticle.md) is an electron-like excitation dressed by the interacting medium. Adiabatic continuity connects low-energy states of an ordinary [Fermi liquid](../../../../fermi-liquid-split.md) to those of a free [Fermi gas](../../../../fermi-gas.md) without changing their particle statistics or conserved quantum numbers. The excitation has a renormalized dispersion, [effective mass](../../../../band-effective-mass.md), magnetic response and finite lifetime. [Pauli exclusion principle](../../../../pauli-exclusion-principle.md) restricts collisions near the [Fermi surface](../../../../fermi-surface.md); in a regular three-dimensional [Fermi liquid](../../../../fermi-liquid-split.md),

$$
\frac{\hbar}{\tau}\sim\frac{(\epsilon-\mu)^2+(\pi k_BT)^2}{E_*}.
$$

Thus the width is small compared with excitation [energy](../../../../energy-split.md) sufficiently near the surface at low [temperature](../../../../temperature-split.md). This permits particle-like counting and transport even when microscopic interactions are strong. It does not make every interaction disappear: the [Landau quasiparticle energy functional](../../../../landau-quasiparticle-energy-functional.md) contains residual interactions,

$$
\delta E=\sum_a\epsilon_a\delta n_a+\frac1{2\mathcal V}\sum_{ab}f_{ab}\delta n_a\delta n_b.
$$

Specific heats and magnetic susceptibilities need not equal their bare-gas values. Logarithmic corrections can modify the lifetime scale in two dimensions, and a [Luttinger liquid](../../../../luttinger-liquid.md) or a fractional Hall fluid is not an ordinary weakly perturbed [electron](../../../../electron.md) gas.

An electron-like excitation in a normal metal and a neutral fermionic excitation in normal [helium-3](../../../../helium-3.md) are [Landau quasiparticles](../../../../landau-quasiparticle.md). More generally, [phonons](../../../../phonon.md), [magnons](../../../../magnon.md) and [excitons](../../../../exciton.md) are particle-like collective excitations, with their own statistics and quantum numbers; they are not all [Landau quasiparticles](../../../../landau-quasiparticle.md). [composite fermions](../../../../composite-fermion.md) are another emergent description, reorganizing correlations in a partly occupied [Landau level](../../../../landau-level.md) rather than simply replacing the [electron](../../../../electron.md) mass in an ordinary band.

Attach two statistical flux quanta $\Phi_0=h/e$ to each [electron](../../../../electron.md). Even attachment preserves fermionic exchange statistics, while the average statistical field opposes the applied field:

$$
B^*=B-2n_s\Phi_0,\qquad \nu=\frac{n_s\Phi_0}{B},\qquad
\nu^*=\frac{n_s\Phi_0}{B^*}=\frac{\nu}{1-2\nu}.
$$

This is an effective description of correlations, not literal flux tubes produced by small solenoids. An integer number of filled effective levels can give an incompressible electronic fractional Hall state. This is the correspondence between integer Hall quantization of [composite fermions](../../../../composite-fermion.md) and selected fractional Hall states of [electrons](../../../../electron.md).[1989 publisher abstract: fractional Hall states as integer states after even flux attachment](../../../../composite-fermion-approach-for-the-fractional-quantum-hall-effect-by-j-k-jain.md)

Setting the signed effective filling to integer $p$ gives

$$
p(1-2\nu)=\nu,\qquad\boxed{\nu=\frac{p}{2p+1}.}
$$

Positive $p$ gives $1/3,2/5,3/7,\ldots$ below $1/2$. Negative $p=-q$, $q>0$, gives $q/(2q-1)$ above it, including $2/3,3/5,4/7,\ldots$. The sign records reversed $B^*$. At $\nu=1/2$, the mean effective field vanishes, so the simplest description is a compressible composite-fermion sea rather than another member with finite integer $p$. Fractional charged excitations of gapped Hall states and the charge used in this semiclassical composite-fermion orbit description should not be conflated.

A direct probe away from the incompressible fractions is [composite-fermion geometric resonance](../../../../composite-fermion-geometric-resonance.md). One implementation patterned a high-mobility GaAs/AlGaAs [Hall bar](../../../../hall-bar.md) into periodic and random antidot arrays. [electron beam lithography](../../../../electron-beam-lithography.md) followed by an approximately $130\,\mathrm{nm}$ reactive-ion etch made arrays with periods $400$–$700\,\mathrm{nm}$. Four-terminal low-current measurements swept a perpendicular [magnetic field](../../../../magnetic-field-split.md) at low [temperature](../../../../temperature-split.md); red-light illumination varied density and the modulation. Periodic arrays showed commensurability structure near half filling and a Hall anomaly; matched random arrays did not. Unpatterned sections supplied another reference.[pp.3598–3600, fabrication, measurement method and Figs.1–3](../../../../composite-fermions-in-periodic-and-random-antidot-lattices-by-j-h-smet-and-others.md)

The semiclassical explanation uses, for a fully spin-polarized sea,

$$
k_F^*=\sqrt{4\pi n_s},\qquad R_c^*=\frac{\hbar k_F^*}{e|B-B_{1/2}|},\qquad
B_{1/2}=\frac{2hn_s}{e}.
$$

The mass cancels from the orbit [radius](../../../../radius.md). A selected orbit fits the lattice when $2R_c^*\simeq C a$, with a geometry-dependent constant $C$ of order unity. Pinned orbits around antidots then alter longitudinal transport, producing features near

$$
\boxed{|B-B_{1/2}|\simeq\frac{2\hbar\sqrt{4\pi n_s}}{eCa}.}
$$

The simplest single-antidot scale has $C\simeq1$; detailed peak positions require the actual potential and orbit family. The two field directions bend orbits oppositely. The diagnostic is an orbit scale controlled by the small residual $B^*$, rather than the much larger applied $B$. At the same density the fully polarized $k_F^*$ is $\sqrt2$ times the zero-field spin-degenerate [electron](../../../../electron.md) value; this is an independent counting test.

Calibrate density from independent Hall/filling measurements and compare several lattice periods. Use small excitation and [temperature](../../../../temperature-split.md) sweeps, and check periodic, random and unpatterned regions. Density variation changes both $B_{1/2}$ and the orbit scale, so simply plotting against uncorrected field can mislead. [mean free path](../../../../mean-free-path.md) and density inhomogeneity limit resolution; illumination can soften or substantially change the imposed potential, so it cannot automatically be treated as density adjustment alone. These qualifications are part of the inference from geometry to emergent particles, rather than a claim that every feature near half filling is a new fractional plateau.

<a id="2/image-composite-fermion-orbit-test"></a>
![](../../../../past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2012/paper-1-composite-orbits.png)

**[Figure 4](#2/image-composite-fermion-orbit-test). Composite-fermion orbit test**.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the physics of Nanoelectronic Systems course of the University of Cambridge](../../../split.md)
5. [Physics of Nanoelectronic Systems course of the University of Cambridge](../../../../physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
