<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

After complete [ionization](../../../../../ionization.md), each [hydrogen](../../../../../hydrogen.md) nucleus supplies one [ion](../../../../../ion.md) and one [Electron](../../../../../electron.md), while each [helium-4](../../../../../helium-4.md) nucleus supplies one [ion](../../../../../ion.md) and two [Electrons](../../../../../electron.md). Neglecting the small [metal mass fraction](../../../../../metal-mass-fraction.md) $Z$ and putting $Y\simeq1-X$, the [mean molecular weight](../../../../../mean-molecular-weight.md) therefore satisfies

$$
\frac1\mu=2X+\frac34Y\simeq\frac{3+5X}{4},\qquad \boxed{\mu\simeq\frac4{3+5X}}.
$$

Use [stellar homology](../../../../../stellar-homology.md) to compare models with common dimensionless profiles. The [stellar mass conservation equation](../../../../../stellar-mass-conservation-equation.md), [stellar hydrostatic equation](../../../../../hydrostatic-pressure-support-equation.md) and [ideal gas law](../../../../../ideal-gas-law.md) give

$$
\rho_c\propto\frac M{R^3},\qquad P_c\propto\frac{GM^2}{R^4},\qquad T_c\propto\frac{\mu M}{R}.
$$

The [radiative diffusion in a star](../../../../../radiative-diffusion-in-a-star.md) equation then gives $L_{\rm rad}\propto RT_c^4/(\kappa_c\rho_c)$. Inserting the specified [opacity](../../../../../opacity.md) yields $L_{\rm rad}\propto RT_c^7/(Z\rho_c^2)\propto\mu^7M^5/Z$. Independently, integrating the [stellar energy-generation rate](../../../../../stellar-energy-generation-rate.md) over the [mass](../../../../../mass.md) gives $L_{\rm nuc}\propto X^2\rho_cT_c^5M\propto X^2\mu^5M^7/R^8$. Equating these in [stellar thermal equilibrium](../../../../../stellar-thermal-equilibrium.md) gives the [radiative homology with fifth-power hydrogen burning and inverse-cubic opacity](../../../../../radiative-homology-with-fifth-power-hydrogen-burning-and-inverse-cubic-opacity.md):

$$
R^8\propto X^2Z\mu^{-2}M^2,\qquad R\propto X^{1/4}Z^{1/8}\mu^{-1/4}M^{1/4},\qquad T_c\propto\frac{\mu^{5/4}M^{3/4}}{X^{1/4}Z^{1/8}}.
$$

At fixed [solar mass](../../../../../solar-mass.md) these reduce to **$L\propto\mu^7/Z$ and $T_c\propto\mu^{5/4}/(X^{1/4}Z^{1/8})$.** The [stellar homology](../../../../../stellar-homology.md) approximation, rather than merely the local power laws, is what permits these relations between whole stars.

Equal [luminosities](../../../../../luminosity.md) imply $\mu_2/\mu_1=(Z_2/Z_1)^{1/7}=2^{-1/7}$. Thus

$$
3+5X_2=2^{1/7}(3+5X_1),\qquad X_2=\frac{6.5\,2^{1/7}-3}{5}=0.8353\ldots,
$$

so **$X_2=0.8$ to one significant figure**. Retaining the unrounded [hydrogen mass fraction](../../../../../hydrogen-mass-fraction.md) when comparing [central temperatures](../../../../../central-stellar-temperature.md) gives

$$
\frac{T_{c,2}}{T_{c,1}}=2^{-3/56}\left(\frac{X_1}{X_2}\right)^{1/4}=0.9219\ldots<1.
$$

**The first model has the higher central temperature.**

For homogeneous [hydrogen burning](../../../../../hydrogen-burning.md) at fixed $M,Z$, fuel conservation gives $ME_0\dot X=-L$. Since $d\mu/dX=-5\mu^2/4$ and $L=L_0(\mu/\mu_0)^7$, the [homogeneous fuel-depletion luminosity feedback](../../../../../homogeneous-fuel-depletion-luminosity-feedback.md) obeys

$$
\dot\mu=\frac{5L_0}{4ME_0\mu_0^7}\mu^9,\qquad \frac{d}{dt}\mu^{-8}=-\frac{10L_0}{ME_0\mu_0^7}.
$$

Integration with the initial [mean molecular weight](../../../../../mean-molecular-weight.md) $\mu_0$ gives

$$
\boxed{L(t)=L_0\left(1-\frac{10\mu_0L_0t}{ME_0}\right)^{-7/8}}.
$$

This idealized [stellar evolution](../../../../../stellar-evolution.md) law stops when $X=0$; it does not predict a physically attainable infinite [luminosity](../../../../../luminosity.md). Indeed $\mu=4/3$ at fuel exhaustion, giving $t_H=ME_0[1-(3\mu_0/4)^8]/(10\mu_0L_0)$, strictly before the formal singularity.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
