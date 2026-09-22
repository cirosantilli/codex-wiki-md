<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Band edges and optical transitions.** A [direct band gap](../../../direct-band-gap.md) has the conduction minimum and valence maximum at the same [crystal momentum](../../../crystal-momentum.md). A near-edge [photon](../../../photon.md) then connects the two almost vertically on an energy-versus-wavevector plot, because its [momentum](../../../momentum-split.md) is small on the [Brillouin zone](../../../brillouin-zone.md) scale. An [indirect band gap](../../../indirect-band-gap.md) has the extrema at different momenta, so an additional [momentum](../../../momentum-split.md) transfer, commonly supplied by [phonon](../../../phonon.md) absorption or emission, is required for a near-edge radiative transition. This reduces its probability relative to an allowed direct transition.

Near the zone centre, an isotropic direct-gap model has $E_c(k)=E_c+\hbar^2k^2/(2m_e^*)$ and downward valence dispersions $E_{v,j}(k)=E_v-\hbar^2k^2/(2m_{h,j}^*)$. The [heavy-hole and light-hole bands](../../../heavy-hole-and-light-hole-bands.md) are the upper branches with large and small positive hole masses: the heavy branch is flatter. In common cubic [semiconductors](../../../semiconductor-split.md) these arise from the $j=3/2$ manifold, while [spin-orbit coupling](../../../spin-orbit-interaction.md) places the $j=1/2$ [split-off valence band](../../../split-off-valence-band.md) lower by $\Delta_{\mathrm{so}}$. Its thermally generated hole population is suppressed by approximately $e^{-\Delta_{\mathrm{so}}/(k_BT)}$ relative to upper-valence holes, apart from density-of-states factors. Neglect is justified when $\Delta_{\mathrm{so}}\gg k_BT$; it is not a universal exclusion of this band at arbitrary [temperature](../../../temperature-split.md).

<a id="3/image-original-schematic-direct-and-indirect-band-edges-including-heavy-light-and-split-off-hole-branches"></a>
![](../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2017-semiconductor-bands.png)

**[Figure 3](#3/image-original-schematic-direct-and-indirect-band-edges-including-heavy-light-and-split-off-hole-branches). Original schematic direct and indirect band edges, including heavy, light and split-off hole branches**.

For an indirect material such as Si, the conduction minimum need not be at $\Gamma$. In applying the carrier-density formulae, $E_c$ must mean the actual minimum of the included conduction valley. The supplied scalar effective masses and densities of states constitute a simplified band-edge model; they do not specify Si's full valley anisotropy or multiplicity.

**Carrier populations.** Let $f(E)$ be the [Fermi-Dirac distribution](../../../fermi-dirac-distribution.md). In the nondegenerate conduction tail, $f(E)\simeq e^{-(E-\mu)/(k_BT)}$. Set $x=E-E_c$ and integrate the given [density of states](../../../density-of-states.md):

$$
n=\int_{E_c}^\infty g_e(E)f(E)\,dE=\frac1{2\pi^2}\left(\frac{2m_e^*}{\hbar^2}\right)^{3/2}e^{-(E_c-\mu)/(k_BT)}\int_0^\infty x^{1/2}e^{-x/(k_BT)}\,dx.
$$

The integral is $\Gamma(3/2)(k_BT)^{3/2}=\sqrt\pi(k_BT)^{3/2}/2$. Defining the [effective density of states](../../../effective-density-of-states.md) gives

$$
\boxed{n=N_c e^{-(E_c-\mu)/(k_BT)},\qquad N_c=2\left(\frac{m_e^*k_BT}{2\pi\hbar^2}\right)^{3/2}.}
$$

The factor two is already included in the supplied [density of states](../../../density-of-states.md); it must not be added a second time.

A hole is an unoccupied valence state. For $E$ sufficiently below $\mu$, $1-f(E)\simeq e^{(E-\mu)/(k_BT)}$. Substitution of $x=E_v-E$ gives in exactly the same way

$$
\boxed{p=N_v e^{-(\mu-E_v)/(k_BT)},\qquad N_v=2\left(\frac{m_h^*k_BT}{2\pi\hbar^2}\right)^{3/2}.}
$$

Their product eliminates the [chemical potential](../../../chemical-potential-split.md):

$$
\boxed{np=N_cN_v e^{-E_g/(k_BT)}=n_i^2.}
$$

This is the [semiconductor mass-action law](../../../semiconductor-mass-action-law.md) at [thermal equilibrium](../../../thermal-equilibrium-split.md). In an [intrinsic semiconductor](../../../intrinsic-semiconductor.md), [charge neutrality](../../../charge-neutrality.md) additionally gives

$$
\boxed{n=p=n_i=\sqrt{N_cN_v}\,e^{-E_g/(2k_BT)}=2\left(\frac{k_BT}{2\pi\hbar^2}\right)^{3/2}(m_e^*m_h^*)^{3/4}e^{-E_g/(2k_BT)}.}
$$

In a doped [semiconductor](../../../semiconductor-split.md) the product still applies in this nondegenerate equilibrium model, but the two populations need not be equal.

**Intrinsic [chemical potential](../../../chemical-potential-split.md).** Taking logarithms of $n=p$ yields the [intrinsic-semiconductor chemical potential](../../../intrinsic-semiconductor-chemical-potential.md)

$$
\boxed{\mu_i=\frac{E_c+E_v}{2}+\frac{k_BT}{2}\ln\frac{N_v}{N_c}=E_v+\frac{E_g}{2}+\frac{3k_BT}{4}\ln\frac{m_h^*}{m_e^*}.}
$$

For unequal band degeneracies, use the first form with the full $N_c,N_v$. For the supplied mass ratio $m_h^*/m_e^*=1/2$, the shift from midgap at $300\,\mathrm K$ is approximately $-13.4\,\mathrm{meV}$, toward the valence edge.

**Three [temperature](../../../temperature-split.md) regimes.** The original plot runs from high [temperature](../../../temperature-split.md) on the left to low [temperature](../../../temperature-split.md) on the right. At high [temperature](../../../temperature-split.md), thermal excitation across the gap dominates and $n\simeq p\simeq n_i$ rises rapidly with [temperature](../../../temperature-split.md). In the middle, donors and acceptors are effectively ionized, the material is extrinsic, and $n\simeq N_D-N_A$ makes the plateau. At low [temperature](../../../temperature-split.md), [dopant freeze-out](../../../dopant-freeze-out.md) binds increasing numbers of [electrons](../../../electron.md) to donor levels, reducing the mobile-electron population as the sample cools. Its activation scale is a donor [binding energy](../../../binding-energy.md), not the full [band gap](../../../band-gap.md). Compensation and incomplete ionization affect that regime.

**Gap estimate from the original figure.** On the dashed intrinsic branch, $n_i=C T^{3/2}e^{-E_g/(2k_BT)}$. Hence [band-gap extraction from intrinsic carrier activation](../../../band-gap-extraction-from-intrinsic-carrier-activation.md) uses the slope of $\ln(n_i/T^{3/2})$ versus $1/T$. With $x=1000\,\mathrm K/T$ and $k_B$ expressed in eV/K, two points give

$$
E_g=\frac{2000\,k_B\mathrm K}{x_2-x_1}\left[\ln\frac{n_{i,1}}{n_{i,2}}-\frac32\ln\frac{x_2}{x_1}\right].
$$

The very compressed intrinsic branch is only approximately readable: $n_i\sim10^{15}\,\mathrm{cm^{-3}}$ near $x\sim1.8$ and $n_i\sim10^{13}\,\mathrm{cm^{-3}}$ near $x\sim2.5$. These give **$E_g\sim1.0\,\mathrm{eV}$**, rather than a precision determination. Neglecting the thermal prefactor gives about $1.13\,\mathrm{eV}$ from those same rough points. Thus **a gap of order $1$–$1.1\,\mathrm{eV}$** is justified by this schematic plot; its resolution does not support distinguishing a few hundredths of an electronvolt. The declining freeze-out branch must not be used to infer the full gap.

**Room-temperature densities.** At $300\,\mathrm K$, the supplied masses give

$$
N_c=2.43\times10^{19}\,\mathrm{cm^{-3}},\qquad N_v=8.61\times10^{18}\,\mathrm{cm^{-3}}.
$$

In the fully ionized extrinsic plateau, put $N=N_D-N_A=10^{15}\,\mathrm{cm^{-3}}$. [Charge neutrality](../../../charge-neutrality.md) and the mass-action law imply

$$
n-p=N,\qquad np=n_i^2,\qquad n=\frac{N+\sqrt{N^2+4n_i^2}}2,\qquad p=\frac{n_i^2}{n}.
$$

Since $n_i\ll N$, **$n\simeq10^{15}\,\mathrm{cm^{-3}}$** is insensitive to the imprecise gap. The minority density is much more sensitive:

$$
\boxed{p\simeq\frac{N_cN_v}{N}e^{-E_g/(k_BT)}=2.10\times10^{23}e^{-E_g/(0.02585\,\mathrm{eV})}\,\mathrm{cm^{-3}}.}
$$

Using $E_g=1.0\,\mathrm{eV}$ gives $n_i\simeq5.8\times10^{10}\,\mathrm{cm^{-3}}$ and $p\simeq3.3\times10^6\,\mathrm{cm^{-3}}$. Using $1.1\,\mathrm{eV}$ instead gives $n_i\simeq8.3\times10^9\,\mathrm{cm^{-3}}$ and $p\simeq7.0\times10^4\,\mathrm{cm^{-3}}$. These are explicitly conditional estimates within the stated mass model. The plot alone cannot fix a precise minority density because the uncertain gap occurs inside an exponential.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [2017](../../2017-split.md)
3. [Past exam of the quantum condensed matter course of the University of Cambridge](../../split.md)
4. [Quantum Condensed Matter course of the University of Cambridge](../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../university-of-cambridge-split.md)
11. [List of universities](../../../list-of-universities.md)
12. [Codex Wiki](../../../split.md)
