<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Denote [aerosol optical depth](../../../../aerosol-optical-depth.md) by $\tau_a$ to distinguish it from [cloud optical depth](../../../../optical-depth.md). Retrieve $N$ as in [d](../d.md), collocate it with $\tau_a$, and estimate an [aerosol-to-droplet susceptibility](../../../../aerosol-cloud-interaction.md)

$$
s_a=\left.\frac{d\log N}{d\log\tau_a}\right|_{\text{matched meteorology and cloud-water conditions}}.
$$

A [regression](../../../../regression-analysis.md) should control for [water content](../../../../liquid-water-content.md), updraught and [cloud](../../../../cloud.md) regime; [aerosol optical depth](../../../../aerosol-optical-depth.md) is not itself a direct measurement of activated nuclei. For an approximately constant $s_a$ over a factor two in [aerosol](../../../../aerosol.md), $N_2/N_1=2^{s_a}$.

Integrate the supplied [cloud albedo susceptibility](../../../../cloud-albedo-susceptibility.md) rather than treating a finite doubling as infinitesimal:

$$
d\log\frac A{1-A}=\tfrac13d\log N,
\qquad
\boxed{A_2=\frac{2^{s_a/3}A_1}{1-A_1+2^{s_a/3}A_1}.}
$$

For a small response, $\Delta A\simeq A_1(1-A_1)s_a\log2/3$. If $F_{\rm sw}$ is the appropriate mean incoming shortwave flux and $f_c$ the fraction of the scene occupied by these [clouds](../../../../cloud.md), the leading top-of-atmosphere perturbation, positive downward, is

$$
\boxed{\Delta F_{\rm TOA}\simeq-f_cF_{\rm sw}\,\mathcal T_{\rm above}^{\downarrow}\mathcal T_{\rm above}^{\uparrow}\,(A_2-A_1).}
$$

The two [transmissions](../../../../transmittance.md) account approximately for the atmosphere above the [cloud](../../../../cloud.md) and may be absorbed into an effective illuminating flux. In the simplest global transparent-overburden estimate $F_{\rm sw}=L_{\circledast}/4$. Positive $s_a$ gives increased reflection and negative [shortwave forcing](../../../../radiative-forcing.md), the [Twomey effect](../../../../twomey-effect.md). Numerical forcing cannot be determined from the given susceptibility alone: it needs baseline [albedo](../../../../albedo.md), [cloud](../../../../cloud.md) fraction, illumination and an empirically constrained $s_a$. Humidity swelling, [cloud](../../../../cloud.md) contamination of [aerosol](../../../../aerosol.md) retrievals and common meteorological influences can create spurious correlations. Changes in [cloud](../../../../cloud.md) amount, [water path](../../../../liquid-water-path.md) or lifetime are additional adjustments, not the fixed-water Twomey term derived here.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
