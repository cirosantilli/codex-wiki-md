<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An additional atomic input is needed: the total [Case B recombination](../../../../case-b-recombination.md) coefficient does not specify the number of [H-alpha](../../../../h-alpha.md) [photons](../../../../photon.md) per net [radiative recombination](../../../../radiative-recombination.md). Let $y_\alpha=\alpha_{\rm H\alpha}^{\rm eff}/\alpha_r$, where $\alpha_{\rm H\alpha}^{\rm eff}$ is the [effective recombination coefficient](../../../../effective-recombination-coefficient.md). At the approximately $10^4\ \mathrm K$ [temperature](../../../../temperature-split.md) implicit in the supplied $\alpha_r$, take $y_\alpha\simeq0.45$. The coefficient 2.2 used later in the paper corresponds to $y_\alpha=1/2.2\simeq0.455$, which we use consistently here.

For an unextinguished, fully filled [Strömgren sphere](../../../../stromgren-sphere.md) with negligible central cavity, the [H-alpha](../../../../h-alpha.md) [luminosity](../../../../luminosity.md) and [observed radiative flux](../../../../observed-radiative-flux.md) satisfy

$$
4\pi D^2F_{\rm H\alpha}=y_\alpha\frac{hc}{\lambda_{\rm H\alpha}}\alpha_rn_e^2\frac{4\pi r_S^3}{3},\qquad
r_S=\frac{\theta D}{2}.
$$

Substitution eliminates $r_S$ and gives

$$
\boxed{D=\frac{24F_{\rm H\alpha}\lambda_{\rm H\alpha}}
{y_\alpha hc\alpha_rn_e^2\theta^3}.}
$$

Convert the angular diameter to [radians](../../../../radian.md): $\theta=56\times10^{-3}/206265=2.7150\times10^{-7}$. Also $hc/\lambda_{\rm H\alpha}=3.0268\times10^{-19}\ \mathrm J$. Thus

$$
\boxed{D=1.5422\times10^{19}\ \mathrm m\simeq500\ \mathrm{pc},\qquad
r_S\simeq2.09\times10^{12}\ \mathrm m\simeq14.0\ \mathrm{au}.}
$$

The implied [hydrogen-ionizing photon production rate](../../../../hydrogen-ionizing-photon-production-rate.md) is $Q\simeq1.00\times10^{39}\ \mathrm{s^{-1}}$. Using $y_\alpha=0.45$ instead gives $D\simeq505\ \mathrm{pc}$. These values use the printed milliarcseconds and integrated line [observed radiative flux](../../../../observed-radiative-flux.md). Assuming one [H-alpha](../../../../h-alpha.md) [photon](../../../../photon.md) per recombination would give a different, unjustified distance. An appreciable cavity or a nonunit filling factor must also enter the emitting volume.

The [Brackett series](../../../../brackett-series.md) consists of transitions ending at $n=4$, at infrared [wavelengths](../../../../wavelength.md). They suffer much less [interstellar extinction](../../../../interstellar-extinction.md) than [H-alpha](../../../../h-alpha.md), so their corrected [observed radiative fluxes](../../../../observed-radiative-flux.md) can give a more reliable version of the same inference. At fixed measured angular size and [number density](../../../../number-density.md), the formula has $D\propto F$: uncorrected [interstellar extinction](../../../../interstellar-extinction.md) therefore makes this particular distance estimate too small. Infrared lines are weaker and need their own [effective recombination coefficients](../../../../effective-recombination-coefficient.md); their advantage is reduced sensitivity to dust.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
