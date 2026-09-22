<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take the [two-dimensional electron gas](../../../../two-dimensional-electron-gas.md) in the $xy$ plane, the [Hall bar](../../../../hall-bar.md) along $x$, and $\mathbf B=B\hat{\mathbf z}$ with $B>0$ perpendicular to it. An [electron](../../../../electron.md) has charge $-e$. The confining [electron](../../../../electron.md) [potential energy](../../../../potential-energy.md) $U(y)$ is approximately flat inside a wide strip and rises at either boundary; smooth [quenched disorder](../../../../quenched-disorder.md) adds hills and valleys. For a slowly varying edge, each spin-resolved [Landau level](../../../../landau-level.md) approximately follows

$$
E_{n,s}(Y)=\hbar\omega_c(n+\tfrac12)+U(Y)+s\frac{g^*\mu_BB}{2},\qquad
\omega_c=\frac{eB}{m^*},\qquad \ell_B=\sqrt{\frac{\hbar}{eB}}.
$$

Here $s=\pm1$, and $Y$ is the [guiding centre](../../../../guiding-center.md). For $\mathbf A=(-By,0,0)$, $Y=\ell_B^2k_x$ and the edge [group velocity](../../../../group-velocity.md) is

$$
\boxed{v_x=\frac1\hbar\frac{\partial E}{\partial k_x}=\frac{U'(Y)}{eB}.}
$$

Thus [electrons](../../../../electron.md) move along $+x$ at the upper edge and $-x$ at the lower edge. The [Lorentz force](../../../../lorentz-force.md) gives counterclockwise bulk cyclotron motion in this convention. At a hard boundary its interrupted circles become directed [skipping orbits](../../../../skipping-orbit.md); a smooth boundary gives the corresponding guiding-centre drift. Smooth bulk [quenched disorder](../../../../quenched-disorder.md) generally gives closed drift contours around localized hills or valleys, with extended trajectories appearing near a broadened level's critical [energy](../../../../energy-split.md). Realistic [electrostatic screening](../../../../electrostatic-screening.md) can produce alternating [compressible quantum Hall edge strips](../../../../compressible-quantum-hall-edge-strip.md) and [incompressible quantum Hall edge strips](../../../../incompressible-quantum-hall-edge-strip.md), so the unscreened bending curves are an effective sketch rather than an exact self-consistent edge profile.

In the original diagram, contacts are ordered around the [electron](../../../../electron.md) propagation direction: upper-left $1\to2\to3$, then lower-right $4\to5\to6$. Let $I_1=I$, $I_4=-I$ and the other leads be ideal [equilibrating voltage probes](../../../../equilibrating-voltage-probe.md). Define $R_H=(V_2-V_6)/I$ and $R_{xx}=(V_2-V_3)/I$. These choices fix the [voltage](../../../../voltage.md) sign; reversing the field reverses chirality and the Hall polarity. For spin-resolved plateau index $N$,

$$
\boxed{R_H=\frac{h}{Ne^2},\qquad R_{xx}=0.}
$$

At fixed sheet [carrier density](../../../../carrier-density.md) and increasing field, $N$ decreases, giving successively higher Hall plateaus; longitudinal peaks occur between them. Unresolved [spin](../../../../spin.md) branches can suppress odd plateaus. The sketch uses resistance magnitudes, and every integer step is not promised in an arbitrary sample.

<a id="1/image-hall-states-and-resistance"></a>
![](../../../../past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2012/paper-1-hall-states.png)

**[Figure 1](#1/image-hall-states-and-resistance). Hall states and resistance**.

For [Fermi-energy oscillations in a two-dimensional electron gas](../../../../fermi-energy-oscillations-in-a-two-dimensional-electron-gas.md), first distinguish fixed density from fixed reservoir [chemical potential](../../../../chemical-potential-split.md). At negligible [temperature](../../../../temperature-split.md) the former is determined by state counting. Each resolved [Landau level](../../../../landau-level.md) contains $eB/h$ states per unit [area](../../../../surface-area.md), so

$$
\nu=\frac{n_sh}{eB},\qquad E_n=\hbar\omega_c(n+\tfrac12).
$$

Ignoring [spin](../../../../spin.md) and broadening for the counting illustration, if $N<\nu<N+1$ then $N$ levels are full and level $N$ is partly full: $\mu=E_N$. At fixed $n_s$, increasing $B$ increases both level [energy](../../../../energy-split.md) and degeneracy. The partly filled level rises in [energy](../../../../energy-split.md) until the lower levels can contain all [electrons](../../../../electron.md); $\mu$ then drops to the next lower level. The resulting sawtooth is periodic in $1/B$, with **$\Delta(1/B)=e/(n_sh)$ per resolved branch**. At an exactly integer filling in an ideal gap, any [chemical potential](../../../../chemical-potential-split.md) within the gap gives the same zero-temperature particle number; the plotted discontinuity denotes its limiting values.

At fixed $B$ while $n_s$ increases, the ideal [chemical potential](../../../../chemical-potential-split.md) stays at a partly occupied level and steps upward after each additional density $eB/h$. It therefore has a staircase superposed on the rising zero-field trend, not a repeated downward sawtooth. [Landau-level broadening](../../../../landau-level-broadening.md) and finite [temperature](../../../../temperature-split.md) smooth both ideal graphs. With an externally pinned [chemical potential](../../../../chemical-potential-split.md), density changes instead; the fixed-density sawtooth cannot simultaneously be imposed. In a realistic disordered sample, the [Fermi energy](../../../../fermi-energy.md) sweeps localized states between transport-carrying level centres. The following schematic omits [spin](../../../../spin.md) for clarity and does not attempt an interaction-corrected [density of states](../../../../density-of-states.md).

<a id="1/image-landau-filling-and-chemical-potential"></a>
![](../../../../past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2012/paper-1-fermi-oscillations.png)

**[Figure 2](#1/image-landau-filling-and-chemical-potential). Landau filling and chemical potential**.

For $N$ transmitted spin-resolved [quantum Hall edge states](../../../../quantum-hall-edge-state.md), the [Landauer-Büttiker formula](../../../../landauer-buttiker-formula.md) reduces, in that contact order, to

$$
I_i=\frac{Ne^2}{h}(V_i-V_{i-1}),\qquad V_0\equiv V_6.
$$

Zero probe currents imply $V_2=V_3=V_1$ and $V_5=V_6=V_4$. Hence $I=(Ne^2/h)(V_1-V_4)$ and the boxed resistance results follow. The [spin-resolved conductance quantum](../../../../spin-resolved-conductance-quantum.md) arises because the one-dimensional [density of states](../../../../density-of-states.md) times velocity is $1/h$ per unit [energy](../../../../energy-split.md); a reservoir imbalance supplies $e^2\Delta V/h$ per channel. Its value does not depend on edge slope or sample width.

On a plateau, opposite-moving edge channels are separated by a wide bulk with a [mobility gap](../../../../mobility-gap.md). Ordinary [elastic scattering](../../../../elastic-scattering.md) on one edge has no counterpropagating channel into which to reflect; closed bulk orbits do not connect the contacts. Changing $B$ or $n_s$ can alter the occupancy of localized states without changing the number of transmitting edge channels. This accounts for the **finite plateau width**, which an entirely clean set of sharp levels would not explain. Accuracy requires negligible backscattering between opposite edges, low enough current to avoid breakdown, equilibrating contacts and negligible probe loading. The finite-width plateau and the precision of its quantized value are related but distinct observations.

An [antidot](../../../../quantum-hall-antidot.md) is a depleted potential hill, not a potential well. Its closed edge circulates oppositely to the outer boundary. In a constriction, tunnelling through an antidot orbit can transfer an [electron](../../../../electron.md) from a forward edge into the returning edge: [resonant antidot backscattering](../../../../resonant-antidot-backscattering.md) produces conductance dips. For $N$ otherwise open spin-resolved channels and one active [resonance](../../../../resonance.md),

$$
G=\frac{e^2}{h}\bigl[N-\mathcal R(E_F)\bigr],\qquad
\mathcal R(E)=\frac{\Gamma_L\Gamma_R}{(E-\epsilon_m)^2+(\Gamma_L+\Gamma_R)^2/4}.
$$

At symmetric coupling a single [resonance](../../../../resonance.md) can remove $e^2/h$; asymmetry or thermal averaging reduces its depth. If the background constriction is closed and the resonant route instead supplies forward transmission, peaks occur. The lead connectivity must therefore accompany the conductance sketch. In the fixed-area single-particle limit, successive alignments change enclosed flux by $\Phi_0=h/e$, giving the [Aharonov-Bohm antidot period](../../../../aharonov-bohm-antidot-period.md)

$$
\boxed{\Delta B\simeq\frac{h}{eA_{\rm eff}}.}
$$

The effective orbit [area](../../../../surface-area.md), not merely the etched island [area](../../../../surface-area.md), enters. Charging, screening and [spin](../../../../spin.md) can modify this simple sequence; two coupled [spin](../../../../spin.md) branches can yield a near-$h/(2e)$ pattern without changing the elementary flux quantum.[2000 author abstract: charging model and two resonances per $h/e$ flux cycle](../../../../coulomb-blockade-of-tunnelling-through-compressible-rings-formed-around-an-antidot-by-m-kataoka-and-others.md)

<a id="1/image-antidot-resonant-backscattering"></a>
![](../../../../past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2012/paper-1-antidot.png)

**[Figure 3](#1/image-antidot-resonant-backscattering). Antidot resonant backscattering**.

## ↑ Ancestors (13)

1. [1](../1.md)
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
