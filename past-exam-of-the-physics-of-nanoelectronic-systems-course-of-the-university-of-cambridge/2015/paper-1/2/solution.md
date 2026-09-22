<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Integer Hall transport and filling.** A clean [two-dimensional electron gas](../../../../two-dimensional-electron-gas.md) at low temperature in a strong perpendicular [magnetic field](../../../../magnetic-field-split.md) forms [Landau levels](../../../../landau-level.md) with orbital spacing $\hbar\omega_c$, where $\omega_c=e|B|/m^*$. Examples include semiconductor heterojunctions and inversion layers. On integer plateaus,

$$
\boxed{|\sigma_{xy}|=\nu\frac{e^2}{h},\qquad\sigma_{xx}\simeq0,
\qquad |R_{xy}|=\frac h{\nu e^2},\qquad R_{xx}\simeq0,}
$$

with integer plateau index $\nu$. The [density of states](../../../../density-of-states.md) in one resolved Landau branch is $e|B|/h$ per unit area, so the actual [filling factor](../../../../filling-factor-quantum-hall-effect.md) is

$$
\boxed{\nu_{\rm fill}=\frac{n_sh}{e|B|}.}
$$

It varies continuously with density and field. Within a disorder-broadened plateau, localized states can change occupation without changing the integer number of transporting edge branches; the filling need not equal the plateau integer at every point in that interval.

At a boundary, the confining potential bends the Landau energies through the [Fermi energy](../../../../fermi-energy.md), giving chiral edge states, interpreted semiclassically as skipping orbits. Opposite edges carry opposite propagation directions. An ideal spin-resolved transmitted edge channel contributes $e^2/h$; $\nu$ such channels give $I=\nu(e^2/h)(V_S-V_D)$. Chirality and suppressed backscattering between well-separated edges explain vanishing longitudinal [voltage](../../../../voltage.md). Ideal reservoirs and appropriate probe equilibration are part of this edge-state transport model.

**A gated [antidot](../../../../quantum-hall-antidot.md).** A local repulsive gate potential depletes an island inside the [Hall bar](../../../../hall-bar.md). Edge states circulate around its boundary as closed [antidot](../../../../quantum-hall-antidot.md) orbits. When a localized orbit is weakly coupled to extended channels on opposite sides, resonance at the reservoir [electrochemical potential](../../../../electrochemical-potential.md) permits backscattering and produces conductance dips on an otherwise quantized transmitting plateau. If the path instead adds a transmission route between otherwise disconnected channels, resonant peaks can occur: the sign depends on the device's tunnel connectivity and what conductance is measured. An isolated [antidot](../../../../quantum-hall-antidot.md) too far from every conducting edge has negligible transport signature.

For the simplest opposite-edge backscattering picture with one active branch,

$$
G(B,V_g)\simeq\frac{e^2}{h}[f-\mathcal R_{\rm res}(B,V_g)],\qquad
0\le\mathcal R_{\rm res}\le1,
$$

where $f$ branches would otherwise transmit. A gate moves the resonance through the [Fermi energy](../../../../fermi-energy.md) by changing both confinement and orbit area. Stronger depletion of the constrictions also changes $f$, producing broad conductance plateaus or pinch-off, with narrow resonances superposed where coupling is finite. Low temperature resolves individual resonances; thermal and [tunnel broadening](../../../../tunnel-broadening.md) can merge them.

For a fixed-area single-electron orbit, a phase change of $2\pi$ corresponds to

$$
\boxed{\Delta B\simeq\frac{\Phi_0}{A_{\rm eff}},\qquad\Phi_0=\frac he.}
$$

Sweeping gate [voltage](../../../../voltage.md) at fixed field shifts enclosed area and level energy, giving oscillatory resonance tracks. This period is not automatically set by the lithographic gate area. [Charging energy](../../../../charging-energy.md), self-consistent screening and [spin](../../../../spin.md) branches modify spacings; in particular coupled [spin](../../../../spin.md) branches in a charging model can generate two resonances per $h/e$ cycle without changing the [electron](../../../../electron.md) flux quantum.[Primary abstract: charging model, two spin branches and two outer-edge resonances per h/e cycle](../../../../coulomb-blockade-of-tunnelling-through-compressible-rings-formed-around-an-antidot-by-m-kataoka-and-others.md)

<a id="2/image-original-schematic-antidot-resonances-on-transmitting-plateaus-varied-coupling-and-gate-controlled-channel-opening-illustrative-coordinates-rather-than-experimental-data"></a>
![](../../../../past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2015/paper-1-antidot-conductance.png)

**[Figure 2](#2/image-original-schematic-antidot-resonances-on-transmitting-plateaus-varied-coupling-and-gate-controlled-channel-opening-illustrative-coordinates-rather-than-experimental-data). Original schematic antidot resonances on transmitting plateaus: varied coupling and gate-controlled channel opening; illustrative coordinates rather than experimental data**.

No [antidot](../../../../quantum-hall-antidot.md) dimensions, [capacitances](../../../../capacitance.md), lever arms or measured spectrum are supplied, so absolute periods and resonance [voltages](../../../../voltage.md) cannot be extracted. The sketch illustrates the mechanisms and regimes requested, rather than inventing a numerical device data set.

**Improving the bare edge potential.** A picture of noninteracting [Landau levels](../../../../landau-level.md) simply intersecting a prescribed smooth confinement ignores the redistribution and screening of [electron](../../../../electron.md) charge. A self-consistent electrostatic calculation combines gate and donor potentials, [electron](../../../../electron.md) density and Coulomb interactions. Where a partially occupied [Landau level](../../../../landau-level.md) has a large density response, [electrons](../../../../electron.md) screen strongly and create a compressible strip with nearly pinned level energy. Regions with the [chemical potential](../../../../chemical-potential-split.md) in a gap are incompressible and support much of the potential change. Consequently the screened edge alternates between compressible and incompressible strips, rather than preserving an arbitrary externally drawn slope. Finite temperature, disorder, exchange and edge reconstruction can require refinements beyond the simplest electrostatic model.[Physical Review B46,4026(1992), primary abstract: self-consistent confinement and alternating compressible/incompressible strips](../../../../electrostatics-of-edge-channels-by-d-b-chklovskii-and-others.md)

**Fractional states and [composite fermions](../../../../composite-fermion.md).** Very clean two-dimensional systems show plateaus at selected fractional fillings, with small longitudinal resistance and a many-electron excitation gap. Electron-electron correlations are essential; partial filling of a noninteracting [Landau level](../../../../landau-level.md) is not enough. The simplest [composite fermion](../../../../composite-fermion.md) binds two statistical flux quanta to each [electron](../../../../electron.md). This is a representation of correlated [electron](../../../../electron.md) motion, not a physical solenoid attached to a particle. With $B>0$, $\Phi_0=h/e$, and density $n_s$, the mean effective field is

$$
B^*=B-2n_s\Phi_0=B(1-2\nu),\qquad
\nu=\frac{n_s\Phi_0}{B}.
$$

Define a signed effective filling $\nu^*=n_s\Phi_0/B^*$. Then

$$
\boxed{\nu^*=\frac{\nu}{1-2\nu},\qquad
\nu=\frac{\nu^*}{2\nu^*+1}.}
$$

For $\nu^*=p>0$, filled composite-fermion levels produce $\nu=p/(2p+1)=1/3,2/5,3/7,\ldots$. For reversed effective field write $\nu^*=-p$, giving $\nu=p/(2p-1)=1,2/3,3/5,\ldots$; the nontrivial fractional upper sequence starts with $p=2$. If effective filling is defined as nonnegative using $|B^*|$, retain these as separate field-direction branches instead of using the signed expression blindly. At $\nu=1/2$ the mean $B^*$ vanishes and the effective filling diverges, so it is not an integer composite-fermion Hall plateau in this simplest construction. Attaching two flux quanta preserves fermionic statistics; the emergent integer-like gaps organize a prominent sequence of fractional electronic states.[Physical Review Letters63,199(1989), abstract: even-flux composite objects and fractional states as effective integer Hall states](../../../../composite-fermion-approach-for-the-fractional-quantum-hall-effect-by-j-k-jain.md)

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
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
