<h1 id="a6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\varepsilon_s$ be the energy of one adsorbed atom, using the same energy reference as the gas-phase value $\varepsilon_0$. For equivalent, noninteracting [adsorption sites](../../../../../adsorption-site.md), choosing the occupied positions gives

$$
\Omega(M,N_1)=\binom{M}{N_1}=\frac{M!}{N_1!(M-N_1)!}.
$$

Every configuration has energy $N_1\varepsilon_s$, so the [canonical lattice-gas partition function](../../../../../canonical-lattice-gas-partition-function.md) is

$$
\boxed{Z_{N_1}=\binom{M}{N_1}e^{-\beta N_1\varepsilon_s}},\qquad \beta=\frac1{k_BT}.
$$

There is no further $1/N_1!$ factor: the combinatorial choice already counts indistinguishable adsorbates correctly. The [Helmholtz free energy](../../../../../helmholtz-free-energy.md), using [Stirling's approximation](../../../../../stirling-formula.md) for a macroscopic number of occupied and empty sites, is

$$
A_s\simeq N_1\varepsilon_s+k_BT\left[N_1\ln N_1+(M-N_1)\ln(M-N_1)-M\ln M\right].
$$

Hence the adsorbed-phase [chemical potential](../../../../../chemical-potential-split.md) at fixed $T,M$ is

$$
\mu_s=\left(\frac{\partial A_s}{\partial N_1}\right)_{T,M}
=\varepsilon_s+k_BT\ln\frac{N_1}{M-N_1}
=\varepsilon_s+k_BT\ln\frac{\theta_1}{1-\theta_1}.
$$

The logarithm comes from configurational entropy: adding an atom is less favorable when vacancies are scarce. In the gas, the stipulated expression can be written

$$
\mu_g=\varepsilon_0+k_BT\ln\frac{p\Lambda^3}{k_BT},\qquad
\Lambda=\frac{h}{\sqrt{2\pi m k_BT}},
$$

where $\Lambda$ is the [thermal de Broglie wavelength](../../../../../thermal-de-broglie-wavelength.md). Equality of [chemical potentials](../../../../../chemical-potential-split.md) at [chemical equilibrium](../../../../../chemical-equilibrium.md) gives

$$
\frac{\theta_1}{1-\theta_1}=\frac{p\Lambda^3}{k_BT}
 e^{(\varepsilon_0-\varepsilon_s)/(k_BT)}=bp.
$$

Therefore

$$
\boxed{\theta_1=\frac{bp}{1+bp}},\qquad
\boxed{b=\frac{\Lambda^3}{k_BT}e^{(\varepsilon_0-\varepsilon_s)/(k_BT)}}.
$$

The [binding energy](../../../../../binding-energy.md) $E_b=\varepsilon_0-\varepsilon_s$ is positive for favorable binding. The units of $b$ are inverse pressure, making $bp$ dimensionless. Choosing the adsorbed energy as zero simply sets $\varepsilon_s=0$ and leaves the same physics; it must not remove the relative [binding energy](../../../../../binding-energy.md). This is the [Langmuir isotherm](../../../../../langmuir-adsorption-model.md), with low-pressure linear uptake and high-pressure monolayer saturation.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [A6](../../a6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the chemistry A course of the University of Cambridge](../../../../split.md)
6. [Chemistry A course of the University of Cambridge](../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
