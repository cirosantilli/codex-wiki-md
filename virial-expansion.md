# Virial expansion

↑ **Parent:** [Statistical physics](statistical-physics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Virial_expansion)

The [virial expansion](virial-expansion.md) describes the first departures from the [ideal gas law](ideal-gas-law.md) as a [power series](power-series.md) in [number density](number-density.md). For a homogeneous, single-species [gas](gas.md) in three dimensions at [thermal equilibrium](thermal-equilibrium-split.md), write $n=N/V$, with $V$ the [volume](volume-thermodynamics.md), and define the [dimensionless](dimensionless-quantity.md) compressibility factor $Z$ by

$$
Z=\frac{p}{nk_BT}=1+B_2(T)n+B_3(T)n^2+\cdots,
\qquad p=nk_BT\bigl[1+B_2(T)n+B_3(T)n^2+\cdots\bigr].
$$

Here $p$ is absolute [pressure](pressure-split.md), $T$ is absolute [thermodynamic temperature](thermodynamic-temperature.md), and $k_B$ is the [Boltzmann constant](boltzmann-constant.md). The [second virial coefficient](second-virial-coefficient.md) determines the initial slope away from $Z=1$; higher coefficients describe further corrections. The symbol $Z$ here is an [equation of state](equation-of-state.md) ratio, not a [canonical partition function](canonical-partition-function.md). [Tong, Statistical Physics, section 2.5, equation 2.69](https://davidtong.org/teaching/statistical-physics/statmechhtml/S2#S2.S5)

<a id="image-controlled-gas-expansion-and-extraction-of-a-dilute-gas-slope-schematic-apparatus-and-explicitly-chosen-toy-curves"></a>
![](second-virial-pvt-and-slope.png)

**[Figure 12](#image-controlled-gas-expansion-and-extraction-of-a-dilute-gas-slope-schematic-apparatus-and-explicitly-chosen-toy-curves). Controlled gas expansion and extraction of a dilute-gas slope: schematic apparatus and explicitly chosen toy curves**.

The left panel sketches the measurement principle; the right panel uses deliberately chosen [polynomials](polynomial-split.md), $Z=1+bx+6x^2$ with $x=n\ell^3$ and $b=\pm2$, where $\ell$ is a reference length. These curves are not measured data. Their initial slopes have opposite signs, but both bend because of the quadratic term. Using a finite secant from $x=0$ to $x=h$ gives $(Z(h)-1)/h=b+6h$, rather than $b$: reducing the fitting range reduces this particular truncation bias. This algebra explains why measuring one nonideal [pressure](pressure-split.md) is insufficient to extract a reliable [second virial coefficient](second-virial-coefficient.md).

Waxman and Hastings's 1971 Burnett experiment used sample and expansion chambers in a thermostatic bath, with a valve between them and a [pressure](pressure-split.md) transducer linked to a piston gauge. They measured successive [isothermal expansions](isothermal-expansion.md): evacuate the expansion chamber, open the valve, record the equilibrated [pressure](pressure-split.md), isolate and evacuate that chamber again, then repeat. This avoids separately measuring the absolute gas amount and chamber [volumes](volume.md). For [carbon dioxide](carbon-dioxide.md) at $50\,{}^\circ\mathrm C$, their measurements below $35$ bar gave a molar [second virial coefficient](second-virial-coefficient.md) of approximately $-102.2\,\mathrm{cm^3\,mol^{-1}}$. [Waxman and Hastings, Journal of Research of the NBS 75C (1971), pages 165–176, abstract and apparatus](https://nvlpubs.nist.gov/nistpubs/jres/75C/jresv75Cn3-4p165_A1b.pdf)

An idealized reduction makes the signal explicit. Let $q=(V_A+V_B)/V_A$ be the calibrated chamber [volume](volume.md) ratio, $p_i$ the pre-expansion [pressure](pressure-split.md), and $p_f$ the post-expansion [pressure](pressure-split.md). Particle conservation during one valve opening gives $n_f=n_i/q$. At the same [temperature](temperature-split.md), division of the two [equations of state](equation-of-state.md) yields

$$
\frac{p_i}{p_f}=q\frac{Z(n_i,T)}{Z(n_i/q,T)}
=q+(q-1)\frac{B_2(T)}{k_BT}p_i+O(p_i^2).
$$

Thus the intercept determines $q$, while the dilute-limit slope determines the [second virial coefficient](second-virial-coefficient.md). In the actual experiment, [helium](helium.md) runs calibrated the cell constant and chamber deformation corrections were included. Agreement of the [carbon dioxide](carbon-dioxide.md) low-[pressure](pressure-split.md) intercept with the [helium](helium.md) calibration, and the absence of an anomalous low-[pressure](pressure-split.md) upturn, checked for gas adsorption on chamber walls. [Waxman and Hastings (1971), data reduction and adsorption checks, especially equation 13 and page 176](https://nvlpubs.nist.gov/nistpubs/jres/75C/jresv75Cn3-4p165_A1b.pdf)

For a limited dilute-gas fit, hold [temperature](temperature-split.md) fixed, allow [thermal equilibrium](thermal-equilibrium-split.md) after every expansion, calibrate absolute [pressure](pressure-split.md) and the chamber ratio, and check leaks and sample composition. Repeat the analysis with a smaller upper [pressure](pressure-split.md) cutoff and an added curvature term; compare the resulting [second virial coefficients](second-virial-coefficient.md) with their uncertainties. Too wide a range mixes in higher coefficients; too narrow a range makes the nonideal signal hard to distinguish from instrument error. The displayed chamber equation neglects deformation, dead spaces and adsorption, so it is a teaching reduction rather than the complete experimental analysis.

Units matter. With [number density](number-density.md) in $\mathrm{m^{-3}}$, $B_2$ has units $\mathrm{m^3}$ and $B_3$ has units $\mathrm{m^6}$. For molar density $c=n/N_{\mathrm A}$ in $\mathrm{mol\,m^{-3}}$, the same [equation of state](equation-of-state.md) is

$$
Z=\frac{p}{cRT}=1+B_{2,\mathrm m}c+B_{3,\mathrm m}c^2+\cdots,
\qquad B_{2,\mathrm m}=N_{\mathrm A}B_2,\qquad
B_{3,\mathrm m}=N_{\mathrm A}^2B_3.
$$

Here $N_{\mathrm A}$ is the [Avogadro constant](avogadro-constant.md) and $R=N_{\mathrm A}k_B$ is the [molar gas constant](molar-gas-constant.md); the molar coefficients have units $\mathrm{m^3\,mol^{-1}}$ and $\mathrm{m^6\,mol^{-2}}$. A coefficient tabulated per [mole](mole-unit.md) must therefore multiply molar density, not [number density](number-density.md).

For the classical formulas below, use a [nondegenerate gas](nondegenerate-gas.md) with [thermal de Broglie wavelength](thermal-de-broglie-wavelength.md) $\lambda_{\mathrm{th}}$ satisfying $n\lambda_{\mathrm{th}}^3\ll1$, negligible quantum corrections to relative motion, and a stable, sufficiently short-ranged [pair potential](pair-potential.md). Diluteness must also control the omitted interaction terms: $|B_2n|\ll1$ alone is not enough when positive and negative contributions cancel. A finite truncation is a local low-[number density](number-density.md) approximation, not an [equation of state](equation-of-state.md) for a dense liquid or across a [phase transition](phase-transition.md). [Tong, section 2.2.4: classical-density condition](https://davidtong.org/teaching/statistical-physics/statmechhtml/S2#S2.S2.SS4) [Tong, section 2.5.1: dilute interacting gas](https://davidtong.org/teaching/statistical-physics/statmechhtml/S2#S2.S5.SS1)

**Table of contents**

- [Virial coefficients of the van der Waals gas](virial-coefficients-of-the-van-der-waals-gas.md)
- [Boyle temperature](boyle-temperature.md)
- [Second virial coefficient](second-virial-coefficient.md)
  - [Soft-core high-temperature second virial coefficient](soft-core-high-temperature-second-virial-coefficient.md)
  - [Density versus molar second virial convention](density-versus-molar-second-virial-convention.md)
  - [Exchange contribution to the second virial coefficient](exchange-contribution-to-the-second-virial-coefficient.md)
  - [Second virial coefficient of a bounded cubic repulsion](second-virial-coefficient-of-a-bounded-cubic-repulsion.md)
- [Cluster expansion](cluster-expansion.md)

## ↑ Ancestors (4)

1. [Statistical physics](statistical-physics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Boyle temperature](boyle-temperature.md)
- [Classical Gases by David Tong](classical-gases-by-david-tong.md)
- [Compressibility factor](compressibility-factor.md)
- [Density versus molar second virial convention](density-versus-molar-second-virial-convention.md)
- [Gas thermometer](gas-thermometer.md)
- [Hard-sphere gas](hard-sphere-gas.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3/33c/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/35a/iii/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2016/paper-1/1/a/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017/2/a/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2018/section-b/b3/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019/section-a/3/solution.md)
- [Second virial coefficient](second-virial-coefficient.md)
- [Virial expansion](virial-expansion.md)
