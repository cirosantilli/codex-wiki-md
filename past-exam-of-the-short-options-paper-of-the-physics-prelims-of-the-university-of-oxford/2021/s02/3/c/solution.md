<h1 id="s02/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Evaluate the source's printed logarithm using the numerical magnitude value 21.0, with base-ten [logarithms](../../../../../logarithm.md):

$$
\log_{10}\frac{R_e}{\mathrm{kpc}}=1.3\log_{10}(250)-0.8\log_{10}(21)-1.36=0.69955,
\qquad \boxed{R_e\simeq5.01\,\mathrm{kpc}.}
$$

This is the literal printed-fit convention identified above. Convert the mean visual [surface brightness](../../../../../surface-brightness.md) to a linear [luminosity](../../../../../luminosity.md) per projected [area](../../../../../surface-area.md). At 10 [parsecs](../../../../../parsec.md), one square [arcsecond](../../../../../arcsecond.md) subtends $100/(206264.806)^2\,\mathrm{pc^2}$. The definition of [absolute magnitude](../../../../../absolute-magnitude.md) consequently gives

$$
\frac{\mathcal I_e}{L_{V,\odot}\,\mathrm{pc^{-2}}}=10^{-0.4(\mu_e-M_{V,\odot}-21.572)}
=10^{-0.4(21.0-4.8-21.572)}\simeq140.9.
$$

The constant $21.572=5\log_{10}(206264.806)-5$ is the conversion between the angular and physical projected [area](../../../../../surface-area.md). Since the [effective radius](../../../../../effective-radius.md) encloses half the total [luminosity](../../../../../luminosity.md),

$$
\boxed{L_V=2\pi R_e^2\mathcal I_e\simeq2.22\times10^{10}L_{V,\odot}.}
$$

For the stipulated [stellar population](../../../../../stellar-population.md) of [Solar-type stars](../../../../../solar-analog.md), approximate the stellar [mass-to-light ratio](../../../../../mass-to-light-ratio.md) by $M_\odot/L_{V,\odot}$. Summing 100 such galaxies then gives

$$
\boxed{M_{*,\mathrm{cluster}}\simeq100\frac{L_V}{L_{V,\odot}}M_\odot=2.22\times10^{12}M_\odot.}
$$

This assumes negligible [interstellar extinction](../../../../../interstellar-extinction.md) and that the supplied [surface brightness](../../../../../surface-brightness.md) is an intrinsic or already corrected value; an observed cosmological [surface brightness](../../../../../surface-brightness.md) requires additional dimming and passband corrections before this conversion.

For comparison only, if the empirical coefficients and intercept were instead meant for $\log_{10}(\mathcal I_e/[L_{V,\odot}\,\mathrm{pc^{-2}}])$, substituting $140.9$ in that fit would give $R_e=1.09\,\mathrm{kpc}$, $L_V=1.06\times10^9L_{V,\odot}$, and $M_{*,\mathrm{cluster}}=1.06\times10^{11}M_\odot$. Those are conditional alternative results, not an unannounced correction of the printed units.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [S02](../../../s02.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
