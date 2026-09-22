<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use $\mathcal R$ for the [stellar gas constant](../../../../../stellar-gas-constant.md), reserving $R$ for the stellar [radius](../../../../../radius.md). The [specific internal energy](../../../../../specific-internal-energy.md) of a [monatomic gas](../../../../../monatomic-gas.md) obeying the [ideal gas](../../../../../ideal-gas.md) law is $e=P/[(\gamma-1)\rho]=3P/(2\rho)$. At fixed enclosed [mass](../../../../../mass.md), the [first law of thermodynamics](../../../../../first-law-of-thermodynamics.md) gives the heat available to the outgoing [luminosity](../../../../../luminosity.md) as $\epsilon=-\partial_te-P\partial_t(1/\rho)$ when there is no [stellar nuclear fusion](../../../../../stellar-nuclear-fusion.md) heating. Therefore

$$
\boxed{\epsilon=-\frac3{2\rho}\left(\frac{\partial P}{\partial t}\right)_m
+\frac{5P}{2\rho^2}\left(\frac{\partial\rho}{\partial t}\right)_m.}
$$

The second coefficient includes both the [mass density](../../../../../density.md) dependence of $e$ and [pressure](../../../../../pressure.md) work. This is [gravitational energy generation in a homologously contracting ideal-gas star](../../../../../gravitational-energy-generation-in-a-homologously-contracting-ideal-gas-star.md).

Write the characteristic scales as

$$
\rho_0=\frac M{4\pi R^3},\qquad P_0=\frac{GM^2}{4\pi R^4},\qquad T_0=\frac{\mu GM}{\mathcal R R}.
$$

Then $\rho=\rho_0b$, $P=P_0p$, $T=T_0p/b$, $m=Mq$ and $L_r=Ll$. Since $d/dr=R^{-1}d/dx$, direct substitution in the [stellar hydrostatic equation](../../../../../hydrostatic-pressure-support-equation.md) and [mass conservation](../../../../../mass-conservation.md) gives

$$
\boxed{\frac{dp}{dx}=-\frac{bq}{x^2},\qquad\frac{dq}{dx}=x^2b.}
$$

For [radiative diffusion in a star](../../../../../radiative-diffusion-in-a-star.md), dividing the [temperature](../../../../../temperature.md) equation by $T_0/R$ gives

$$
\frac d{dx}\left(\frac pb\right)
=-\frac{3\kappa_0\rho_0L}{16\pi acRT_0^4}\frac{bl}{x^2(p/b)^3}
=-D\frac{b^4l}{x^2p^3},\qquad
\boxed{D=\frac{3\kappa_0\mathcal R^4L}{64\pi^2ac\mu^4G^4M^3}.}
$$

In particular the fourth power here is of $\mathcal R$, not of the [radius](../../../../../radius.md).

Because $q(x)$ is fixed and $M$ is constant, a fixed [mass](../../../../../mass.md) label has fixed $x$. Thus [stellar homology](../../../../../stellar-homology.md) gives $\partial_t\rho=-3\rho\dot R/R$ and $\partial_tP=-4P\dot R/R$. The heating rate reduces to $\epsilon=-3P\dot R/(2\rho R)$, positive during [Kelvin-Helmholtz contraction](../../../../../kelvin-helmholtz-mechanism.md). Substitution in $dL_r/dr=4\pi r^2\rho\epsilon$ now yields

$$
\frac{dl}{dx}=-\frac{6\pi R^2\dot R}{L}x^2P
=Ex^2p,\qquad
\boxed{E=-\frac{3GM^2\dot R}{2R^2L}>0.}
$$

The [dimensionless](../../../../../dimensionless-quantity.md) profiles fix $D$ and $E$. In a common [stellar homology](../../../../../stellar-homology.md) family with fixed [stellar composition](../../../../../stellar-chemical-abundance.md) and [opacity](../../../../../opacity.md) normalization, the expression for $D$ implies

$$
\boxed{L=\frac{64\pi^2ac\mu^4G^4D}{3\kappa_0\mathcal R^4}M^3\propto M^3.}
$$

It is independent of [radius](../../../../../radius.md) and constant in time for a particular fixed-mass star. The formula for $E$ gives $\dot R=-2ELR^2/(3GM^2)$, which integrates to

$$
\frac1{R(t)}=\frac1{R_0}+\frac{2ELt}{3GM^2}.
$$

When the initial-radius term is negligible,

$$
\boxed{\frac{RLt}{GM^2}=\frac3{2E}.}
$$

This is the [Kelvin-Helmholtz contraction](../../../../../kelvin-helmholtz-mechanism.md) time law in the prescribed [stellar homology](../../../../../stellar-homology.md) model. Infinite initial [radius](../../../../../radius.md) is a limiting idealization; a finite initial [radius](../../../../../radius.md) retains the first term.

At [main sequence](../../../../../main-sequence.md) arrival, [CNO cycle](../../../../../cno-cycle.md) heating with fixed [stellar composition](../../../../../stellar-chemical-abundance.md) has [luminosity](../../../../../luminosity.md)

$$
L_{\rm nuc}=\epsilon_0M\rho_0T_0^{16}\int_0^1b(q)\left(\frac{p(q)}{b(q)}\right)^{16}dq
\propto\frac{M^{18}}{R^{19}}.
$$

The [integral](../../../../../integral.md) is [dimensionless](../../../../../dimensionless-quantity.md) and fixed within the [stellar homology](../../../../../stellar-homology.md) family. The constant-[opacity](../../../../../opacity.md) radiative scaling still gives $L\propto M^3$. Equating the [stellar nuclear fusion](../../../../../stellar-nuclear-fusion.md) and transported [luminosities](../../../../../luminosity.md) gives

$$
\boxed{R_{\rm MS}\propto M^{15/19}.}
$$

Finally the [Kelvin-Helmholtz contraction](../../../../../kelvin-helmholtz-mechanism.md) law evaluated at $R_{\rm MS}$ gives $t_{\rm MS}\propto M^2/(LR_{\rm MS})\propto M^{-34/19}$. In a coeval [star cluster](../../../../../star-cluster.md), the [mass](../../../../../mass.md) just arriving at the [main sequence](../../../../../main-sequence.md) consequently satisfies

$$
\boxed{M_{\rm arrival}\propto t^{-19/34}.}
$$

These results comprise [constant-opacity homologous contraction to CNO ignition](../../../../../constant-opacity-homologous-contraction-to-cno-ignition.md); their [mass](../../../../../mass.md) exponents compare fixed-composition models with common [dimensionless](../../../../../dimensionless-quantity.md) profiles.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
