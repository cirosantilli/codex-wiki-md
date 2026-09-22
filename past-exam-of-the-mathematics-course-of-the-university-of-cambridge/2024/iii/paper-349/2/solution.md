<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [galaxy mass--metallicity relation](../../../../../galaxy-mass-metallicity-relation.md) is the observed tendency for more massive galaxies to have larger [gas-phase metallicity](../../../../../gas-phase-metallicity.md) and [stellar metallicity](../../../../../stellar-metallicity.md). Gas metallicity is commonly inferred from nebular emission-line ratios in star-forming [H II regions](../../../../../h-ii-region.md), often quoted as $12+\log_{10}(\mathrm O/\mathrm H)$ and measured within a finite spectroscopic aperture. Stellar metallicity comes from stellar absorption features or population-synthesis fits and is luminosity weighted unless the analysis explicitly reconstructs a mass-weighted distribution. [Galaxy stellar mass](../../../../../galaxy-stellar-mass.md) is inferred from photometry or a spectral-energy-distribution fit and depends on the adopted [initial mass function](../../../../../initial-mass-function.md). Radial metallicity gradients, dust, line calibration, and aperture selection must consequently be matched before samples are compared.

The usual physical explanation is that a shallow potential well lets a low-mass galaxy lose a larger fraction of newly synthesized metals in [galactic outflows](../../../../../galactic-outflow.md). The [closed-box model of galactic chemical evolution](../../../../../closed-box-model-of-galactic-chemical-evolution.md) is therefore replaced by a [leaky-box model of galactic chemical evolution](../../../../../leaky-box-model-of-galactic-chemical-evolution.md) with

$$
\dot M_{\rm out}=\lambda\dot M_*,
$$

where $\lambda$ is the [mass-loading factor](../../../../../mass-loading-factor.md). Under the [instantaneous recycling approximation](../../../../../instantaneous-recycling-approximation.md), let $y_z$ be the [stellar yield](../../../../../stellar-yield.md), absorb the returned mass fraction into the definitions, and suppose the escaping gas has the current gas metallicity $Z_g$. Then [mass conservation](../../../../../mass-conservation.md) and metal conservation are

$$
dM_g=-(1+\lambda)dM_*,
$$



$$
d(M_gZ_g)=y_z\,dM_*-(1+\lambda)Z_g\,dM_*.
$$

Substitution of the first equation into the second cancels the terms that merely transfer pre-existing metals and leaves

$$
M_g\,dZ_g=y_z\,dM_*.
$$

Because the mass of metals locked into stars obeys $dM_{z,*}=Z_g\,dM_*$, integration gives $M_{z,*}=M_*Z_*=\int Z_g\,dM_*$. The total newly made metal mass is partitioned between present gas, stars, and the outflow:

$$
y_zM_*=Z_gM_g+M_*Z_*+\lambda\int Z_g\,dM_*.
$$

Writing the [gas-to-stellar mass ratio](../../../../../gas-to-stellar-mass-ratio.md) as $r_g=M_g/M_*$ therefore produces

$$
\boxed{y_z=r_gZ_g+(1+\lambda)Z_*},
\qquad
\boxed{\lambda=\frac{y_z-r_gZ_g}{Z_*}-1}.
$$

Thus simultaneous gas and stellar metallicities, together with the gas fraction and an assumed nucleosynthetic yield, estimate the integrated mass loading. The corresponding [effective yield](../../../../../effective-yield.md) is $y_{\rm eff}=y_z/(1+\lambda)$, and the leaky box has

$$
Z_g=y_{\rm eff}\log\frac{M_{g,0}}{M_g}.
$$

The [G-dwarf problem](../../../../../g-dwarf-problem.md) is that the local Milky Way disk contains far fewer low-metallicity long-lived G dwarfs than the constant-yield closed-box metallicity distribution predicts. A yield that rises with metallicity may initially sound promising because enrichment would accelerate after the first generations. In fact it worsens the problem. In a closed box, $dM_*=-dM_g$ and

$$
M_g\,dZ=y_z(Z)\,dM_*.
$$

For $y_z=kZ$ and a nonzero initial metallicity $Z_0$ at gas mass $M_{g,0}$,

$$
\frac{dZ}{Z}=-k\frac{dM_g}{M_g},
\qquad
\boxed{Z=Z_0\left(\frac{M_{g,0}}{M_g}\right)^k}.
$$

Hence the cumulative mass of stars born below metallicity $Z$ is

$$
\boxed{M_*(\lt Z)=M_{g,0}\left[1-\left(\frac{Z_0}{Z}\right)^{1/k}\right]}.
$$

If the system begins at $Z_0=0$, the assumed yield also vanishes and enrichment never starts. For $Z_0>0$, the [metallicity distribution function](../../../../../metallicity-distribution-function.md) has

$$
\frac{dM_*}{dZ}=\frac{M_{g,0}}{k}Z_0^{1/k}Z^{-1-1/k},
$$

which puts still more stellar mass near the low-metallicity floor. Metal-poor gas inflow, pre-enrichment, and selective outflow are therefore more plausible ingredients in resolving the G-dwarf problem.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
