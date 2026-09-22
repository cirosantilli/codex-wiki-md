<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Outside the emitting layer, take $m\simeq M_c$, $L_r\simeq L$ and $P=\mathcal R\rho T/\mu$. The [Kramers' opacity law](../../../../../../kramers-opacity-law.md) then reads $\kappa=(\kappa_0\mu/\mathcal R)PT^{-9/2}$. Division of the [radiative diffusion in a star](../../../../../../radiative-diffusion-in-a-star.md) equation by the [stellar hydrostatic equation](../../../../../../hydrostatic-pressure-support-equation.md) gives

$$
\frac{dP}{dT}=\frac{16\pi acGM_c}{3\kappa L}T^3,
\qquad
P\frac{dP}{dT}=\frac{16\pi acGM_c\mathcal R}{3\kappa_0L\mu}T^{15/2}.
$$

With the outer [pressure](../../../../../../pressure.md) [constant of integration](../../../../../../constant-of-integration.md) neglected, [integration](../../../../../../integral.md) yields

$$
\boxed{P=CT^{17/4},\qquad
C=\left(\frac{64\pi acGM_c\mathcal R}{51\kappa_0L\mu}\right)^{1/2},\qquad
\rho=\frac{\mu C}{\mathcal R}T^{13/4}.}
$$

Substitute this into [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md):

$$
\frac{17}4CT^{13/4}\frac{dT}{dr}
=-\frac{GM_c}{r^2}\frac{\mu C}{\mathcal R}T^{13/4},
\qquad
\frac{dT}{dr}=-\frac{4\mu GM_c}{17\mathcal Rr^2}.
$$

Define $B=4\mu GM_c/(17\mathcal R)$. The general [antiderivative](../../../../../../antiderivative.md) is $T=B/r+T_0$. The [Kramers radiative-zero envelope around a stellar core](../../../../../../kramers-radiative-zero-envelope-around-a-stellar-core.md) sets $T_0=0$, giving

$$
\boxed{T=\frac{4\mu GM_c}{17\mathcal Rr}.}
$$

This is exact for the idealized boundary $T\to0$ as $r\to\infty$. With a finite outer [radius](../../../../../../radius.md) $R_s$ and [temperature](../../../../../../temperature.md) $T_s$, instead $T=T_s+B(1/r-1/R_s)$; the displayed profile is the deep-envelope approximation when $R_s\gg R_c$ and $|T_s-B/R_s|\ll B/R_c$. Small outer [pressure](../../../../../../pressure.md) alone does not eliminate this [temperature](../../../../../../temperature.md) [constant of integration](../../../../../../constant-of-integration.md).

The specific [hydrogen burning](../../../../../../hydrogen-burning.md) rate becomes

$$
\epsilon=\epsilon_0\rho T^{67/4}
=\frac{\epsilon_0\mu C}{\mathcal R}T^{20}\propto r^{-20}.
$$

Consequently

$$
\boxed{\frac{\epsilon(1.05R_c)}{\epsilon(R_c)}=1.05^{-20}
=e^{-20\log(1.05)}\simeq0.377\simeq e^{-1}.}
$$

Its local radial e-folding length is $R_c/20$, so burning is concentrated within a small fraction of the [stellar core](../../../../../../stellar-core.md) [radius](../../../../../../radius.md). The volume heating is even steeper: $\rho\epsilon\propto C^2T^{93/4}$. Using the exterior envelope profile to estimate the thin shell's [luminosity](../../../../../../luminosity.md) gives

$$
L\simeq4\pi\epsilon_0\left(\frac{\mu C}{\mathcal R}\right)^2B^{93/4}
\int_{R_c}^{\infty}r^{-85/4}dr
=\frac{16\pi\epsilon_0}{81}\left(\frac{\mu C}{\mathcal R}\right)^2B^{93/4}R_c^{-81/4}.
$$

A finite but very extended upper limit changes the factor by $1-(R_c/R_s)^{81/4}$. The large exponent makes this correction small and further verifies the [hydrogen burning](../../../../../../hydrogen-burning.md) thin-shell approximation. Since $C^2\propto M_c/L$ and $B\propto M_c$, the [integral](../../../../../../integral.md) implies $L^2\propto M_c^{97/4}R_c^{-81/4}$. Hence

$$
\boxed{L\propto M_c^{97/8}R_c^{-81/8},\qquad
L\propto M_c^{97/8}\ \text{along the fixed-}R_c\text{ sequence}.}
$$

This is the [fixed-radius-core shell-burning luminosity relation](../../../../../../fixed-radius-core-shell-burning-luminosity-relation.md). The proportionality coefficient is a thin-shell estimate: [luminosity](../../../../../../luminosity.md) rises from its value beneath the shell to $L$ through the emitting layer, so treating it as constant there uses the exterior profile rather than resolving the burning region. The scaling holds while its [dimensionless](../../../../../../dimensionless-quantity.md) shell structure and [stellar composition](../../../../../../stellar-chemical-abundance.md) remain fixed.

For consistency, $M_c/R_c$ must provide a hot [hydrogen burning](../../../../../../hydrogen-burning.md) shell while the [stellar core](../../../../../../stellar-core.md) remains inert to [core helium burning](../../../../../../core-helium-burning.md); the [radiative envelope](../../../../../../radiative-envelope.md) [mass](../../../../../../mass.md) must be much less than $M_c$, and $R_c$ must be well inside an extended [radiative envelope](../../../../../../radiative-envelope.md). At the shell base the gas must remain a [nondegenerate gas](../../../../../../nondegenerate-gas.md) and dominated by [gas pressure](../../../../../../gas-pressure.md), in particular $aT_b^4/3\ll CT_b^{17/4}$ with $T_b=B/R_c$. The assumed [stellar core](../../../../../../stellar-core.md) sequence must genuinely have nearly fixed $R_c$ over the [mass](../../../../../../mass.md) interval considered. A cold [helium](../../../../../../helium.md) [stellar core](../../../../../../stellar-core.md) supported by a nonrelativistic [degenerate electron gas](../../../../../../degenerate-electron-gas.md) instead has the mass-radius law from part (a), so substituting that law would describe a different model and change the [luminosity](../../../../../../luminosity.md) exponent.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
