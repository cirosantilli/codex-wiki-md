<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

**[Magnetization](../../../../../magnetization.md) and field response.** A magnetic material contains microscopic magnetic moments associated with [electron](../../../../../electron.md) [spin](../../../../../spin.md) and orbital motion. The [magnetization](../../../../../magnetization.md) $\mathbf M$ is [magnetic dipole moment](../../../../../magnetic-dipole-moment.md) per unit [volume](../../../../../volume-thermodynamics.md). In SI the macroscopic fields satisfy

$$
\mathbf B=\mu_0(\mathbf H+\mathbf M).
$$

Here $\mathbf H$ separates free-current excitation from the material response. A uniform isotropic linear material has $\mathbf M=\chi_m\mathbf H$, giving

$$
\boxed{\mathbf B=\mu\mathbf H,\qquad\mu_r=1+\chi_m.}
$$

This constant scalar [magnetic permeability](../../../../../permeability-electromagnetism.md) model is useful only within its linear range. Crystals can have a susceptibility [tensor](../../../../../tensor.md); strongly magnetic materials depend on field and magnetic history. For a finite specimen the internal $\mathbf H$ also includes its demagnetizing field. In a uniformly magnetized ellipsoid, $H_{\mathrm{int}}=H_{\mathrm{applied}}-N_dM$ along a [principal axis](../../../../../principal-axis.md), so sample shape affects the apparent susceptibility.

**Diamagnetic and paramagnetic response.** [Diamagnetism](../../../../../diamagnetism.md) is a weak negative susceptibility caused by induced orbital response opposing the applied field. It occurs in all matter but can be masked by larger positive contributions. Closed-shell materials such as bismuth or many organic compounds show it clearly. Ordinary [diamagnetism](../../../../../diamagnetism.md) is often only weakly [temperature](../../../../../temperature-split.md) dependent; superconducting flux exclusion is a separate collective phenomenon and is not described by an arbitrarily small negative susceptibility.

[Paramagnetism](../../../../../paramagnetism.md) arises when available magnetic moments partially align with a field. Thermal disorder prevents complete alignment at weak fields. For independent localized moments of magnitude $m$, the classical weak-field result is

$$
M\simeq\frac{nm^2B}{3k_BT},\qquad
\chi_m\simeq\frac{\mu_0nm^2}{3k_BT},
$$

where the second expression uses $B\simeq\mu_0H$ in a weakly magnetic sample. Thus localized moments obey a [Curie law](../../../../../curie-s-law.md) in this regime. Quantum [angular momentum](../../../../../angular-momentum.md) changes the coefficient to the appropriate $J(J+1)$ expression and gives saturation at strong field. Conduction [electrons](../../../../../electron.md) instead exhibit [Pauli paramagnetism](../../../../../pauli-paramagnetism.md): only states near the [Fermi surface](../../../../../fermi-surface.md) can change [spin](../../../../../spin.md) populations, so a degenerate gas has a nearly temperature-independent response. Its orbital [diamagnetism](../../../../../diamagnetism.md) must also be included for a full metallic susceptibility.

**Collective magnetic order.** [Exchange interactions](../../../../../exchange-interaction.md) can favor parallel alignment, producing [ferromagnetism](../../../../../ferromagnetism.md) below the [Curie temperature](../../../../../curie-temperature.md). Iron, cobalt and nickel are familiar examples. A material may contain regions of spontaneous [magnetization](../../../../../magnetization.md), or [magnetic domains](../../../../../magnetic-domain.md), while having little net external moment because the domains point in different directions. Applied fields move domain walls and rotate moments; at large fields the [magnetization](../../../../../magnetization.md) approaches saturation. Pinning and [energy](../../../../../energy-split.md) barriers make this process hysteretic. [Remanence](../../../../../remanent-magnetization.md) is the [magnetization](../../../../../magnetization.md) left after removing the driving field, and [coercivity](../../../../../coercive-function.md) measures the reverse field needed to bring the chosen response back to zero.

The [area](../../../../../surface-area.md) of a closed $B$–$H$ loop is the [energy](../../../../../energy-split.md) dissipated per unit [volume](../../../../../volume-thermodynamics.md) per quasistatic cycle, $\oint H\,dB$, with positive dissipated magnitude. Consequently the [magnetic permeability](../../../../../permeability-electromagnetism.md) is neither one universal constant nor enough information to describe a ferromagnet: differential [magnetic permeability](../../../../../permeability-electromagnetism.md) $dB/dH$, saturation and [hysteresis](../../../../../hysteresis.md) all matter. Above the ordering [temperature](../../../../../temperature-split.md) the spontaneous moment disappears, and a Curie–Weiss law is often an appropriate approximate paramagnetic description away from the critical region.

In [antiferromagnetism](../../../../../antiferromagnetism.md), ordered opposing sublattices have equal moments and cancel macroscopically in the ideal compensated case. The order disappears above the [Néel temperature](../../../../../neel-temperature.md). In [ferrimagnetism](../../../../../ferrimagnetism.md), opposing sublattices have unequal moments and leave a net [magnetization](../../../../../magnetization.md). Ferrites combine ferrimagnetic response with relatively high electrical resistivity, making them valuable when eddy-current losses would be substantial in a metallic core.

**[Electromagnets](../../../../../electromagnet.md) and engineering choice.** A coil supplies free-current magnetomotive [force](../../../../../force-split.md) $NI$. For a simple uniform magnetic path, [Ampère's law](../../../../../ampere-s-circuital-law.md) gives $H\ell\simeq NI$ and flux $\Phi\simeq\mu ANI/\ell$. A high-[magnetic permeability](../../../../../permeability-electromagnetism.md) soft magnetic core concentrates flux and reduces the current required for a given field. With an air gap $g$,

$$
NI\simeq\frac{B\ell_c}{\mu_0\mu_r}+\frac{Bg}{\mu_0}.
$$

Even a short gap can dominate the [magnetic reluctance](../../../../../magnetic-reluctance.md). The approximate attractive [force](../../../../../force-split.md) across one uniform gap is $F\simeq B^2A/(2\mu_0)$, obtained from the field [energy](../../../../../energy-split.md), with fringing neglected.

Soft magnetic materials have small [coercivity](../../../../../coercive-function.md) and narrow [hysteresis](../../../../../hysteresis.md) loops; they suit relays, [electrical transformer](../../../../../transformer-electrical-engineering.md) cores and controllable [electromagnets](../../../../../electromagnet.md). Hard magnetic materials retain their [magnetization](../../../../../magnetization.md) and suit [permanent magnets](../../../../../permanent-magnet.md). Laminating metallic cores breaks large eddy-current loops; ferrites are useful at higher [frequencies](../../../../../frequency.md) because of their resistivity. Increasing current cannot increase $B$ indefinitely through the linear formula: core saturation, coil heating and leakage limit performance. A good design selects material for the field amplitude, switching [frequency](../../../../../frequency.md) and acceptable loss, rather than simply choosing the largest quoted [magnetic permeability](../../../../../permeability-electromagnetism.md).

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
