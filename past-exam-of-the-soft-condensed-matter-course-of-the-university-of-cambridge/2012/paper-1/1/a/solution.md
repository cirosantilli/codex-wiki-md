<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the squared three-dimensional endpoint [displacements](../../../../../displacement.md), not their arithmetic [mean](../../../../../expected-value-split.md). The [mean squared displacement](../../../../../mean-squared-displacement.md) estimate and corresponding [diffusion coefficient](../../../../../diffusion-coefficient.md) are

$$
\widehat{\langle\Delta r^2\rangle}=\frac{31^2+2^2+50^2+65^2+14^2}{5}=1577.2\,\mu\mathrm m^2,
\qquad \widehat D=\frac{1577.2}{6\times60}=4.38\,\mu\mathrm m^2\,\mathrm s^{-1}.
$$

The factor six is for three-dimensional [Brownian motion](../../../../../brownian-motion-split.md). For an isolated no-slip sphere, the [Stokes–Einstein relation](../../../../../stokes-einstein-relation.md) gives the [Brownian radius estimate from endpoint displacements](../../../../../brownian-radius-estimate-from-endpoint-displacements.md):

$$
\boxed{a=\frac{k_BT}{6\pi\eta\widehat D}\simeq5.6\times10^{-8}\,\mathrm m=56\,\mathrm{nm}.}
$$

Here room [temperature](../../../../../temperature-split.md) is taken as $298\,\mathrm K$; choosing $293\,\mathrm K$ gives $55\,\mathrm{nm}$, a much smaller difference than the sampling uncertainty. Under independent increments with a [normal distribution](../../../../../normal-distribution.md), $\operatorname{sd}(\widehat D)/D=\sqrt{2/(3n)}\simeq0.37$ for $n=5$. The [sampling uncertainty of an endpoint diffusivity estimate](../../../../../sampling-uncertainty-of-an-endpoint-diffusivity-estimate.md) therefore makes this a rough [radius](../../../../../radius.md) estimate. It assumes negligible drift and hydrodynamic coupling between probes, the supplied bulk [viscosity](../../../../../dynamic-viscosity-split.md), and actual three-dimensional tracking. Localization noise adds to the squared [displacements](../../../../../displacement.md) and would bias this inferred [radius](../../../../../radius.md) downward if uncorrected.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the soft condensed matter course of the University of Cambridge](../../../../split.md)
6. [Soft Condensed Matter course of the University of Cambridge](../../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
