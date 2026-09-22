<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

At coexistence, the two phases have equal [chemical potential](../../../../../chemical-potential-split.md). For a single component, $d\mu=-s\,dT+v\,dp$, with [entropy](../../../../../entropy-split.md) and volume measured on the same molar or [mass](../../../../../mass.md) basis. Equating the phase [derivatives](../../../../../derivative.md) along coexistence gives $\Delta v\,dp=\Delta s\,dT$. Reversible [latent heat](../../../../../latent-heat.md) satisfies $L=T\Delta s$, hence

$$
\boxed{\frac{dp}{dT}=\frac{L}{T\Delta v}.}
$$

Here $p$ and $T$ are coexistence [pressure](../../../../../pressure-split.md) and absolute [temperature](../../../../../temperature-split.md), $L$ is [latent heat](../../../../../latent-heat.md) for transforming phase 1 to phase 2, and $\Delta v=v_2-v_1$ uses the same amount of material as $L$.

For vaporization, neglect liquid [molar volume](../../../../../molar-volume.md) compared with ideal-vapour volume $RT/p$. The ideal-vapour Clausius-Clapeyron approximation becomes

$$
\frac{dp}{dT}=\frac{pL_e}{RT^2},\qquad
\ln\frac p{p_b}=-\frac{L_e}{R}\left(\frac1T-\frac1{T_b}\right).
$$

Using the normal boiling reference $T_b=373.15\,\mathrm K$, $p_b=1.01325\times10^5\,\mathrm{Pa}$ and the supplied constant $L_e$ gives

$$
\boxed{p(273\,\mathrm K)\simeq8.2\times10^2\,\mathrm{Pa}.}
$$

This deliberately constant-latent-heat extrapolation does not reproduce the supplied triple-point [pressure](../../../../../pressure-split.md) exactly. It predicts the liquid-vapour branch, metastable against ice below the triple-point [temperature](../../../../../temperature-split.md); it is not a precision sublimation-pressure prediction.

The [phase diagram](../../../../../phase-diagram.md) has solid, liquid and vapour regions meeting at the [triple point](../../../../../triple-point.md). The [sublimation](../../../../../sublimation.md) and vaporization boundaries have positive slopes, whereas the ordinary ice–water boundary slopes negatively because ice has larger specific volume. The liquid–vapour line terminates at a [critical point](../../../../../critical-point.md); the original schematic below emphasizes topology and marks the supplied [triple point](../../../../../triple-point.md).

<a id="section-c/c10/image-schematic-pressure-temperature-phase-topology-of-ordinary-water-with-negative-melting-slope-and-the-supplied-triple-point"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2-water-phase.png)

**[Figure 1](#section-c/c10/image-schematic-pressure-temperature-phase-topology-of-ordinary-water-with-negative-melting-slope-and-the-supplied-triple-point). Schematic pressure–temperature phase topology of ordinary water, with negative melting slope and the supplied triple point**.

For the melting-pressure estimate, [Archimedes' principle](../../../../../archimedes-principle.md) gives $\rho_i=0.90\rho_w=900\,\mathrm{kg\,m^{-3}}$, so

$$
\Delta v=v_w-v_i=\frac1{1000}-\frac1{900}
=-1.111\times10^{-4}\,\mathrm{m^3\,kg^{-1}}.
$$

Convert the molar evaporation [heat](../../../../../heat-split.md) using water [molar mass](../../../../../molar-mass.md) $M\simeq0.0180\,\mathrm{kg\,mol^{-1}}$, rounded from the tabulated value $18.0153\,\mathrm{g\,mol^{-1}}$.[Water entry, CAS 7732-18-5, molecular weight 18.0153](../../../../../nist-chemistry-webbook-srd-69.md) An [enthalpy](../../../../../enthalpy-split.md) cycle through vapour then gives

$$
L_f=L_s-\frac{L_e}{M}
\simeq2.8\times10^6-\frac{40700}{0.0180}
\simeq5.39\times10^5\,\mathrm{J\,kg^{-1}}.
$$

This uses the question's temperature-independent evaporation [heat](../../../../../heat-split.md) all the way to the [triple point](../../../../../triple-point.md); no replacement experimental fusion [heat](../../../../../heat-split.md) is inserted. The [melting pressure inferred from flotation and latent heats](../../../../../melting-pressure-inferred-from-flotation-and-latent-heats.md), on holding $L_f$ and $\Delta v$ constant, is

$$
\boxed{p-p_t=\frac{L_f}{\Delta v}\ln\frac T{T_t}
\simeq5.37\times10^7\,\mathrm{Pa},\qquad
p\simeq54\,\mathrm{MPa},}
$$

using $T_t=273.16\,\mathrm K$ and $T=270.15\,\mathrm K$. Linearizing the logarithm about the [triple point](../../../../../triple-point.md) gives $53.4\,\mathrm{MPa}$ instead of $53.7\,\mathrm{MPa}$. Both are estimates within the stated constant-property approximation; the negative melting slope makes a positive [pressure](../../../../../pressure-split.md) necessary to lower the melting [temperature](../../../../../temperature-split.md).

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
