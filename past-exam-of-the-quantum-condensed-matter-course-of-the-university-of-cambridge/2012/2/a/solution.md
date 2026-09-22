<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [solar cell](../../../../solar-cell.md) uses the [photovoltaic effect](../../../../photovoltaic-effect.md) to turn [photon](../../../../photon.md) [energy](../../../../energy-split.md) into electrical work. In a [semiconductor](../../../../semiconductor-split.md), above-gap [photon absorption](../../../../photon-absorption.md) generates an [electron](../../../../electron.md) in the [conduction band](../../../../conduction-band.md) and an [electron hole](../../../../electron-hole.md) in the [valence band](../../../../valence-band.md). A [p-n junction](../../../../p-n-junction.md), together with selective electrical contacts, collects the two carrier species at opposite terminals. Carrier [diffusion](../../../../diffusion.md) and the built-in [electric field](../../../../electric-field-split.md) help separate them before [electron-hole recombination](../../../../electron-hole-recombination.md). Illumination maintains different [quasi-Fermi levels](../../../../quasi-fermi-level.md) for [electrons](../../../../electron.md) and [electron holes](../../../../electron-hole.md); their splitting, divided by $e$, sets the available terminal voltage in an ideal device. The equilibrium [built-in potential](../../../../built-in-potential.md) alone cannot continuously deliver work.

For an ideal junction, the illuminated output [current density](../../../../current-density.md) is

$$
J(V)=J_{\rm sc}-J_0\left(e^{eV/(k_BT)}-1\right),\qquad
V_{\rm oc}=\frac{k_BT}{e}\log\left(1+\frac{J_{\rm sc}}{J_0}\right).
$$

Here $J_{\rm sc}$ is the photogenerated short-circuit [current density](../../../../current-density.md) and $J_0$ the [diode saturation current](../../../../diode-saturation-current.md). The useful operating point maximizes $VJ$, rather than either current or voltage separately. With [solar-cell fill factor](../../../../solar-cell-fill-factor.md) $\mathrm{FF}=P_{\max}/(V_{\rm oc}I_{\rm sc})$,

$$
\eta=\frac{P_{\max}}{P_{\rm in}}
=\frac{V_{\rm oc}I_{\rm sc}\mathrm{FF}}{P_{\rm in}}.
$$

Series resistance, shunts, incomplete [photon absorption](../../../../photon-absorption.md) and [nonradiative recombination](../../../../nonradiative-recombination.md) reduce the attainable efficiency.

<a id="2/a/image-ideal-illuminated-solar-cell-current-delivered-power-and-the-maximum-power-point"></a>
![](../../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012-solar-cell-output.png)

**[Figure 2](#2/a/image-ideal-illuminated-solar-cell-current-delivered-power-and-the-maximum-power-point). Ideal illuminated solar cell: current, delivered power and the maximum-power point**.

The [Shockley-Queisser limit](../../../../shockley-queisser-limit.md) removes these avoidable losses but retains the following physical constraints. There is one [semiconductor](../../../../semiconductor-split.md) junction with one [band gap](../../../../band-gap.md); each absorbed above-gap [photon](../../../../photon.md) yields at most one collected [electron-hole pair](../../../../electron-hole-pair.md); carriers thermalize to the cell [temperature](../../../../temperature-split.md); and the inverse optical process produces unavoidable [radiative recombination](../../../../radiative-recombination.md). If $\Phi_{\odot}(E)$ is the incident [photon](../../../../photon.md) flux per unit [energy](../../../../energy-split.md), ideal [photon absorption](../../../../photon-absorption.md) gives

$$
J_{\rm sc}=e\int_{E_g}^{\infty}\Phi_{\odot}(E)\,dE.
$$

The same ability to absorb [light](../../../../light.md) requires the junction to emit it. At a forward voltage $V$, the emitted [photon](../../../../photon.md) population has a [chemical potential](../../../../chemical-potential-split.md) $eV$; in the ordinary nondegenerate limit the resulting recombination current is the exponential diode term above. Maximizing $VJ$ with this radiative $J_0$, and then choosing $E_g$, gives the limiting efficiency.

A small [band gap](../../../../band-gap.md) collects many [photons](../../../../photon.md) but gives a low voltage and large thermalization losses. A large [band gap](../../../../band-gap.md) permits a larger voltage but transmits too much of the incident spectrum. Below-gap [photons](../../../../photon.md) are lost to transmission, excess [photon](../../../../photon.md) [energy](../../../../energy-split.md) above the gap becomes heat, and radiative emission and its associated entropy loss keep $eV_{\rm oc}$ below $E_g$. **The optimum single-junction conversion is roughly thirty percent under ordinary unconcentrated sunlight; the precise ceiling depends on spectrum, cell [temperature](../../../../temperature-split.md) and optical geometry.** The original detailed-balance calculation gave about $30\%$ at $E_g\simeq1.1\,\mathrm{eV}$ under its specified assumptions.[Detailed Balance Limit of Efficiency of p-n Junction Solar Cells, Journal of Applied Physics 32 (1961), 510–519; abstract and calculation](https://doi.org/10.1063/1.1736034) Multiple junctions and optical concentration change the assumptions and consequently change the bound.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
