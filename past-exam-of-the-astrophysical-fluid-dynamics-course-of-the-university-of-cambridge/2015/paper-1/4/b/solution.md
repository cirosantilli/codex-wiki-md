<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathcal L$ be net cooling per unit volume, positive when energy is lost. At thermal equilibrium $\mathcal L=0$. For a slow perturbation that maintains [pressure](../../../../../pressure-split.md) balance, the linearized thermal equation is

$$
\rho_0c_p\frac{d\delta T}{dt}=-\left(\frac{\partial\mathcal L}{\partial T}\right)_P\delta T.
$$

The heat capacity factor is positive. A positive derivative restores equilibrium: hotter gas cools more strongly, while cooler gas is heated. This is [isobaric thermal stability of a heated ideal gas](../../../../../isobaric-thermal-stability-of-a-heated-ideal-gas.md).

For fully ionized [hydrogen](../../../../../hydrogen.md), both protons and electrons contribute to the [ideal gas law](../../../../../ideal-gas-law.md), so **$P=2nk_BT$**. Treat the stated constant heat input $\Gamma$ as a fixed heating rate per unit volume. Substituting $n=P/(2k_BT)$ into the cooling gives

$$
\mathcal L(T;P)=\frac{3P^2\alpha_B(T)}{8k_BT}-\Gamma.
$$

At equilibrium $T_0$, its derivative is

$$
\boxed{\left(\frac{\partial\mathcal L}{\partial T}\right)_{P,T_0}
=\frac\Gamma{T_0}\left(\frac{d\ln\alpha_B}{d\ln T}-1\right)_{T_0}.}
$$

With a temperature-independent recombination coefficient, the derivative is $-\Gamma/T_0$: **the equilibrium is thermally unstable to isobaric perturbations**. More generally, any nonincreasing $\alpha_B(T)$ also gives instability; stability requires its logarithmic slope to exceed one. Heating at fixed volume and pressure-balanced perturbations are distinct assumptions: the density falls as a parcel is heated, reducing the quadratic-density cooling.

No temperature law for $\alpha_B$ is supplied, so the displayed slope criterion states the general result without inventing one. A constant incident ultraviolet flux need not imply constant local volumetric heating in a self-consistent ionization-balance calculation. If the heating instead varies with density, temperature or neutral fraction, its derivative must be included; the conclusion here uses the explicit constant-$\Gamma$ model.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
