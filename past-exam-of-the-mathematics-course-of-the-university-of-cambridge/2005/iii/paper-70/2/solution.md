<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Thermal energy versus electrostatic repulsion.** The mean translational [kinetic energy](../../../../../kinetic-energy.md) of one nonrelativistic thermal proton is

$$
\langle E\rangle=\frac32kT_c=4.2\times10^{-9}\ \mathrm{erg}\simeq2.6\ \mathrm{keV}.
$$

Using the center-to-center touching separation $2r_p$, the [Coulomb barrier](../../../../../coulomb-barrier.md) estimate is

$$
E_C\sim\frac{e^2}{2r_p}=1.15\times10^{-6}\ \mathrm{erg}\simeq0.72\ \mathrm{MeV}.
$$

Thus $E_C/\langle E\rangle\simeq274$. Using $r_p$ rather than $2r_p$ as the rough interaction distance doubles the estimate but leaves the conclusion unchanged. Typical solar thermal energies are far below the classical barrier. The two essential ideas are **the high-energy tail of the thermal distribution and quantum tunnelling through the [Coulomb barrier](../../../../../coulomb-barrier.md)**: neither a mean-energy estimate nor a sharp classical cutoff describes the reacting population.

For two equal-mass protons, let $v$ be their relative speed. In the center-of-mass frame each has speed $v/2$, so their total collision energy is

$$
\boxed{E=2\left[\frac12m_p(v/2)^2\right]=\frac14m_pv^2=\frac12\mu_rv^2,\qquad\mu_r=\frac{m_p}{2}.}
$$

Here $\mu_r$ is the [reduced mass](../../../../../reduced-mass.md), not the stellar [mean molecular weight](../../../../../mean-molecular-weight.md).

In the low-energy, nonresonant approximation, the geometrical quantum-wave factor in a [collision cross-section](../../../../../collision-cross-section.md) is proportional to the squared de Broglie wavelength, hence to $1/E$. The slowly varying short-range reaction probability is absorbed into $S_0$; for proton–proton fusion it also includes the small weak-reaction probability. The rapidly varying exponential is the [quantum tunnelling](../../../../../quantum-tunnelling.md) probability. For a Coulomb potential $V(r)=e^2/r$, its leading semiclassical exponent is

$$
-\frac2\hbar\int_0^{e^2/E}\sqrt{2\mu_r(e^2/r-E)}\,dr
=-\frac{\pi e^2\sqrt{2\mu_r}}{\hbar\sqrt E}
=-2\sqrt{E_B/E}.
$$

The integral follows from $r=(e^2/E)\sin^2\theta$; its dimensionless integral is $\pi/2$. A finite nuclear radius modifies the short-distance factor absorbed into $S_0$. In this convention $E_B=\pi^2\mu_re^4/(2\hbar^2)$: it is a penetration-energy scale, distinct from the classical contact energy $E_C$.

**Thermal averaging and pair counting.** Each proton samples collision partners with number [density](../../../../../density.md) $N$ and collision flux $v$, so its collision rate is $N\langle\sigma v\rangle$. Multiplying by the number of protons counts each identical pair twice. The [thermonuclear reaction rate](../../../../../thermonuclear-reaction-rate.md) is therefore

$$
\boxed{R_{pp}=\frac12N^2\int_0^\infty v\sigma(v)n(v)\,dv.}
$$

The relative speed of two independent thermal protons has a [Maxwell-Boltzmann velocity distribution](../../../../../maxwell-boltzmann-velocity-distribution.md) with reduced mass $m_p/2$. Changing variables with $E=m_pv^2/4$ gives the normalized energy [density](../../../../../density.md)

$$
f_E(E)=\frac2{\sqrt\pi}\frac{E^{1/2}}{(kT)^{3/2}}e^{-E/(kT)}.
$$

Substituting $v=2\sqrt{E/m_p}$ and the [collision cross-section](../../../../../collision-cross-section.md) causes the energy powers to cancel:

$$
\boxed{R_{pp}=\frac{S_0N^2}{(kT)^{3/2}}\sqrt{\frac4{\pi m_p}}
\int_0^\infty\exp\left[-\frac E{kT}-2\sqrt{\frac{E_B}E}\right]dE.}
$$

**The Gamow peak and its Gaussian width.** Set $\Phi(E)=E/(kT)+2\sqrt{E_B/E}$. It diverges at either endpoint and has its unique minimum where

$$
\Phi'(E)=\frac1{kT}-\frac{\sqrt{E_B}}{E^{3/2}}=0.
$$

Thus the energy called $E_G$ in this question is the [Gamow peak](../../../../../gamow-peak.md) energy,

$$
\boxed{E_G=[E_B(kT)^2]^{1/3}.}
$$

In the stellar tunnelling regime $E_B\gg kT$,

$$
\frac{E_G}{kT}=\left(\frac{E_B}{kT}\right)^{1/3}\gg1,\qquad
\frac{E_G}{E_B}=\left(\frac{kT}{E_B}\right)^{2/3}\ll1.
$$

This establishes the requested hierarchy in its physical regime; it is not an inequality valid at arbitrary [temperature](../../../../../temperature.md).

At the minimum, $\Phi(E_G)=3E_G/(kT)$ and $\Phi''(E_G)=3/(2kTE_G)$. Hence

$$
\Phi(E)=\frac{3E_G}{kT}+\frac{3(E-E_G)^2}{4kTE_G}+\cdots.
$$

The Gaussian standard deviation is $\sqrt{2kTE_G/3}$, small compared with $E_G$ when $kT\ll E_G$. Extending the lower endpoint to $-\infty$ relative to the peak then gives

$$
\int_0^\infty e^{-\Phi(E)}dE\simeq\sqrt{\frac{4\pi kTE_G}{3}}\,e^{-3E_G/(kT)}.
$$

Combining this with the thermal prefactor yields the [Gaussian approximation to a nonresonant thermonuclear rate](../../../../../gaussian-approximation-to-a-nonresonant-thermonuclear-rate.md),

$$
R_{pp}\simeq\frac{4S_0N^2E_B^{1/6}}{\sqrt{3m_p}(kT)^{2/3}}
\exp\left[-3\left(\frac{E_B}{kT}\right)^{1/3}\right].
$$

At fixed reactant [density](../../../../../density.md) and fixed $S_0,E_B$, comparison with the requested [temperature](../../../../../temperature.md) form gives

$$
\boxed{\alpha=\frac23,\qquad\beta=\frac{27E_B}{k}.}
$$

The constant $\beta$ here has dimensions of [temperature](../../../../../temperature.md); it is not inverse [temperature](../../../../../temperature.md). Resonances, plasma screening or variation of $S(E)$ would require corrections to this particular approximation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
