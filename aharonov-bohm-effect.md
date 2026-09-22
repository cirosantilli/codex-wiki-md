# Aharonov-Bohm effect

↑ **Parent:** [Charge-flux composite](charge-flux-composite.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Aharonov-Bohm_effect)

The Aharonov-Bohm effect is the phase $q\Phi/\hbar$ acquired when a charge $q$ encircles magnetic flux $\Phi$, even when the magnetic field vanishes along the charge's path.

In the magnetic [Aharonov-Bohm effect](aharonov-bohm-effect.md), a coherent [electron](electron.md) wave takes two routes around inaccessible [magnetic flux](magnetic-flux.md). Recombination converts their relative [wave phase](phase-waves.md) into displaced [interference fringes](interference-fringe.md). In 1959, [Yakir Aharonov](yakir-aharonov.md) and [David Bohm](david-joseph-bohm.md) proposed a shielded [solenoid](solenoid.md) geometry and identified the obstruction to removing the [magnetic vector potential](magnetic-vector-potential.md) throughout the accessible region.[1959, §2, pp. 486–487, Fig. 2 and reflecting-barrier discussion](significance-of-electromagnetic-potentials-in-the-quantum-theory-by-yakir-aharonov-and-david-bohm.md)

Use [International System of Units](international-system-of-units.md), [electric charge](electric-charge-split.md) $q$, and [magnetic minimal coupling](magnetic-minimal-coupling.md) $H=(-i\hbar\nabla-q\mathbf A)^2/(2m)$. Let $\gamma_1,\gamma_2$ run from the same source $S$ to the same detector point $D$. The oriented closed curve $C$ follows $\gamma_1$ and then $\gamma_2$ backwards. For a static [magnetic vector potential](magnetic-vector-potential.md), the magnetic contribution to the relative [wave phase](phase-waves.md) is

$$
\delta=\frac q\hbar\left(\int_{\gamma_1}\mathbf A\cdot d\mathbf l-\int_{\gamma_2}\mathbf A\cdot d\mathbf l\right)
=\frac q\hbar\oint_C\mathbf A\cdot d\mathbf l
=\frac{q\Phi_C}{\hbar}\pmod{2\pi}.
$$

Here $\Phi_C=\int_\Sigma\mathbf B\cdot d\mathbf S$ is the oriented [magnetic flux](magnetic-flux.md) through a spanning surface. Equal or calibrated nonmagnetic propagation phases are assumed. For an [electron](electron.md), $q=-e$, where $e>0$ is the [elementary charge](elementary-charge.md); reversing $C$ reverses the sign. The observable is the [gauge-invariant](gauge-invariance.md) [holonomy](holonomy.md) $e^{i\delta}$, rather than a unique local value of the [magnetic vector potential](magnetic-vector-potential.md).

The accessible region is a [multiply connected region](multiply-connected-region.md): $C$ cannot contract to a point without entering the excluded flux region. [Stokes theorem](stokes-theorem.md) does not set the [line integral](line-integral.md) to zero, because a spanning surface must cross that excluded region, where the [magnetic field](magnetic-field-split.md) need not vanish. There is real [magnetic flux](magnetic-flux.md) in the apparatus; only the accessible paths are idealized as free of the [magnetic field](magnetic-field-split.md). The exterior of a finite straight [solenoid](solenoid.md) also permits routes around its ends, so its exact topology and leakage differ from those of an infinite [solenoid](solenoid.md) or an excluded solid [torus](torus.md).

An explicit model makes the obstruction visible. Outside an infinite flux tube of radius $a$, choose [cylindrical coordinates](cylindrical-coordinate-system.md) $(r,\theta,z)$ and

$$
\mathbf A=\frac{\Phi}{2\pi r}\,\widehat{\boldsymbol\theta},\qquad r>a.
$$

Its [curl](curl.md) vanishes there, but a loop with [winding number](winding-number.md) $n$ has $\oint_C\mathbf A\cdot d\mathbf l=n\Phi$. Locally $\mathbf A=\nabla(\Phi\theta/(2\pi))$; the angular coordinate changes by $2\pi$ on a circuit. For generic $q\Phi/\hbar$, that candidate gauge removal changes the [wave function](wave-function-split.md)'s single-valued boundary condition. On a [simply connected](simply-connected-space.md) region, a smooth static [magnetic vector potential](magnetic-vector-potential.md) with zero [curl](curl.md) instead has a globally defined scalar primitive and is a [pure gauge potential](pure-gauge-potential.md). Thus local zero [magnetic field](magnetic-field-split.md) and globally removable [magnetic vector potential](magnetic-vector-potential.md) are different conditions.

<a id="image-two-accessible-paths-can-link-inaccessible-magnetic-flux"></a>
![](aharonov-bohm-two-path-flux-geometry.png)

**[Figure 1](#image-two-accessible-paths-can-link-inaccessible-magnetic-flux). Two accessible paths can link inaccessible magnetic flux**. [Source](aharonov-bohm-two-path-flux-geometry.py). Original functional geometry. Left: a cross-section of an ideal infinite flux tube; $C$ traverses the blue route forwards and the orange route backwards. Right: a meridional section of an excluded solid [torus](torus.md); the [magnetic field](magnetic-field-split.md) circulates inside its core, with opposite signs through the section. One route passes through the central hole and the other outside the [torus](torus.md). The drawn linking surface intersects one core section. Paths denote coherent alternatives, not measured trajectories; shielding thicknesses and beam optics are schematic.

For an original [interference](interference-wave-propagation.md) example, take mutually coherent scalar amplitudes with constant individual intensities $I_1,I_2$ and an imposed carrier phase $ky$, as in [off-axis holography](off-axis-holography.md). Then

$$
I(y)=I_1+I_2+2\sqrt{I_1I_2}\cos(ky+\delta),\qquad
\Delta y=-\frac\delta k\pmod{2\pi/k}.
$$

The [interference fringe spacing](interference-fringe-spacing.md) is $d=2\pi/k$. An [electron](electron.md) enclosing $\Phi=h/(4e)$ has $\delta=-\pi/2$, shifting maxima by $d/4$ for this orientation. Increasing the [magnetic flux](magnetic-flux.md) by $h/e$ changes $\delta$ by $-2\pi$ and restores the same pattern: the [electron](electron.md) [Aharonov-Bohm effect](aharonov-bohm-effect.md) has [magnetic flux quantum](magnetic-flux-quantum.md) $h/e$. This uses $h=2\pi\hbar$, the [Planck constant](planck-constant.md). It does not require the source's [magnetic flux](magnetic-flux.md) to vary continuously during a single exposure.

For $I_1=1$, $I_2=1/4$, the extrema are $I_{\max}=9/4$, $I_{\min}=1/4$, and the [interferometric visibility](interferometric-visibility.md) is $4/5$. A fixed [Aharonov-Bohm phase](aharonov-bohm-effect.md) translates these fringes without changing their contrast. Averaging unresolved fluctuating phases can reduce the contrast; a darkened pattern alone cannot identify enclosed [magnetic flux](magnetic-flux.md). These formulas assume coherence, indistinguishable alternatives and stable beam envelopes.

The appeal of the [Aharonov-Bohm effect](aharonov-bohm-effect.md) is that a local [Lorentz force](lorentz-force.md) calculation along either ideal path misses information carried by their global arrangement. It gives a physical example of [holonomy](holonomy.md) and supplies the encircling phase used in [Chern--Simons flux attachment](chern-simons-flux-attachment.md). This alone does not establish [intrinsic topological order](intrinsic-topological-order.md). The static comparison also matters: changing [magnetic flux](magnetic-flux.md) can induce an [electric field](electric-field-split.md), so a time-dependent experiment requires the scalar-potential contribution as well as the displayed spatial [line integral](line-integral.md).

**Table of contents**

- [Magnetic flux spectrum of a quantum ring](magnetic-flux-spectrum-of-a-quantum-ring.md)
  - [Cosine-potential gap in a quantum ring](cosine-potential-gap-in-a-quantum-ring.md)
- [Shielded toroidal-flux electron interference](shielded-toroidal-flux-electron-interference.md)
- [Discrete gauge cancellation in two-path interference](discrete-gauge-cancellation-in-two-path-interference.md)

## ↑ Ancestors (7)

1. [Charge-flux composite](charge-flux-composite.md)
2. [Anyon](anyon.md)
3. [Topological quantum matter](topological-quantum-matter-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Aharonov-Bohm effect](aharonov-bohm-effect.md)
- [Akira Tonomura](akira-tonomura.md)
- [Chern--Simons flux attachment](chern-simons-flux-attachment.md)
- [Inductive impulse outside a switched solenoid](inductive-impulse-outside-a-switched-solenoid.md)
- [Multiply connected region](multiply-connected-region.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022/section-b/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-342/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-342/1/c/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2014/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2017/4/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2/section-b/b6/d/solution.md)
- [Twisted boundary condition](twisted-boundary-condition.md)
- [Yakir Aharonov](yakir-aharonov.md)
