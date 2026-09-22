<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Consider a small outward displacement $\delta r$ of a fluid element. It adjusts to the ambient [pressure](../../../../../pressure.md) while retaining its [specific entropy](../../../../../specific-entropy.md) and [stellar composition](../../../../../stellar-chemical-abundance.md), so an [adiabatic process](../../../../../adiabatic-process.md) gives $d\log\rho_{\rm parcel}=d\log P/\gamma$. Its excess [mass density](../../../../../density.md) over the new surroundings is, to first order,

$$
\rho_{\rm parcel}-\rho_{\rm ambient}
=\left[\frac\rho{\gamma P}\frac{dP}{dr}-\frac{d\rho}{dr}\right]\delta r.
$$

Restoring [buoyancy](../../../../../buoyancy.md) requires this bracket to be positive. With $\gamma=5/3$, the [Schwarzschild criterion](../../../../../schwarzschild-criterion.md) is therefore

$$
\boxed{\frac{dP}{dr}>\frac{5P}{3\rho}\frac{d\rho}{dr}.}
$$

Equality is neutral stability. For uniform [mean molecular weight](../../../../../mean-molecular-weight.md), the [ideal gas](../../../../../ideal-gas.md) law gives $d\log\rho=d\log P-d\log T$. Since [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) [pressure](../../../../../pressure.md) decreases outward, the inequality is equivalent to $\nabla=d\log T/d\log P<\nabla_{\rm ad}=2/5$. Dividing the [radiative diffusion in a star](../../../../../radiative-diffusion-in-a-star.md) and [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) [stellar structure equations](../../../../../stellar-structure-equations.md) gives

$$
\nabla_{\rm rad}=\frac{3\kappa L_rP}{16\pi acGmT^4},\qquad
\boxed{\frac{3\kappa L_rP}{16\pi acGmT^4}<\frac25.}
$$

This is the [stellar radiative temperature gradient](../../../../../stellar-radiative-temperature-gradient.md) test for [stellar convective stability](../../../../../stellar-convective-stability.md).

In the thin upper [stellar atmosphere](../../../../../stellar-atmosphere.md) take $m\simeq M$, $L_r\simeq L$ and use [gas pressure](../../../../../gas-pressure.md) dominance. The prescribed [opacity](../../../../../opacity.md) becomes $\kappa=\kappa_0\mu PT^{12}/\mathcal R$. Dividing the two structure equations then yields

$$
P\frac{dP}{dT}=\frac{16\pi acGM\mathcal R}{3\kappa_0L\mu}T^{-9}.
$$

At zero [optical depth](../../../../../optical-depth.md), the atmospheric boundary has $T_s^4=T_e^4/2$ and negligible [gas pressure](../../../../../gas-pressure.md). Integrating from that boundary, with $T_s^{-8}=4T_e^{-8}$, gives

$$
\boxed{P^2=\frac{4\pi acGM\mathcal R}{3\kappa_0L\mu T_e^8}
\left(4-\frac{T_e^8}{T^8}\right).}
$$

To locate the onset, put $y=T_e^8/T^8$. [Logarithmic derivative](../../../../../logarithmic-derivative.md) gives $d\log P/d\log T=4y/(4-y)$, hence

$$
\nabla_{\rm rad}=\frac{4-y}{4y}=\frac{T^8}{T_e^8}-\frac14.
$$

This starts at zero at the outer boundary and increases inward. It first reaches $2/5$ at

$$
\boxed{T_b=(13/20)^{1/8}T_e.}
$$

The corresponding [optical depth](../../../../../optical-depth.md) is $\tau_b=\tfrac43(\sqrt{13/20}-\tfrac12)>0$, so the onset lies inside the [stellar atmosphere](../../../../../stellar-atmosphere.md). This is [grey-atmosphere convection onset with thirteenth-power opacity](../../../../../grey-atmosphere-convection-onset-with-thirteenth-power-opacity.md).

Let the interior of the [fully convective star](../../../../../fully-convective-star.md) have $P=K_TT^{5/2}$, with $K_T$ spatially constant. At its boundary $T_b/T_e$ is fixed, so the atmospheric [pressure](../../../../../pressure.md) formula gives

$$
K_T^2=\frac{P_b^2}{T_b^5}\propto\frac M{LT_e^{13}}.
$$

The [Stefan–Boltzmann law](../../../../../stefan-boltzmann-law.md), $L=4\pi R^2\sigma T_e^4$ with $\sigma=ac/4$, consequently implies

$$
K_T^2\propto MR^{13/2}L^{-17/4}.
$$

The [ideal gas](../../../../../ideal-gas.md) equation transforms the interior relation into

$$
P=K_\rho\rho^{5/3},\qquad K_\rho=(\mathcal R/\mu)^{5/3}K_T^{-2/3}.
$$

For completeness, the mass-radius scaling follows by taking $\rho=\rho_c\theta^{3/2}$ and $r=\alpha\xi$ with $\alpha^2=5K_\rho\rho_c^{-1/3}/(8\pi G)$. [Hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) and [mass conservation](../../../../../mass-conservation.md) reduce to the [Lane-Emden equation](../../../../../lane-emden-equation.md) $(\xi^2\theta')'=-\xi^2\theta^{3/2}$, with $\theta(0)=1$, $\theta'(0)=0$. Its fixed [dimensionless](../../../../../dimensionless-quantity.md) profile gives $R\propto\alpha$ and $M\propto\alpha^3\rho_c$. Eliminating $\rho_c$ gives $R\propto K_\rho G^{-1}M^{-1/3}$, or $K_\rho\propto GM^{1/3}R$. Thus $K_T^2\propto M^{-1}R^{-3}$ at fixed [stellar composition](../../../../../stellar-chemical-abundance.md). Equating this with the atmospheric expression gives $L^{17/4}\propto M^2R^{19/2}$, and hence

$$
\boxed{L\propto M^{8/17}R^{38/17}.}
$$

This [Hayashi relation with thirteenth-power opacity](../../../../../hayashi-relation-with-thirteenth-power-opacity.md) concerns the interior of a [fully convective star](../../../../../fully-convective-star.md) beneath a thin [stellar atmosphere](../../../../../stellar-atmosphere.md). The coefficient $K_T$ may vary between stars; spatially constant [specific entropy](../../../../../specific-entropy.md) does not mean equal [specific entropy](../../../../../specific-entropy.md) across the whole sequence.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
