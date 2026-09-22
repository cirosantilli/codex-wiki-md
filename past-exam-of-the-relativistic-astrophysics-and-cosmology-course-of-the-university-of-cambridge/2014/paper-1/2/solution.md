<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The metric uses signature $(+---)$ and a time-valued interval $ds$: a comoving clock has $ds=dt$. Here $t$ is cosmic [proper time](../../../../proper-time.md), $R(t)$ a [scale factor](../../../../scale-factor-cosmology.md) with dimensions of [length](../../../../length.md), $c$ the [speed of light](../../../../speed-of-light.md), $\chi$ a [dimensionless](../../../../dimensionless-quantity.md) comoving radial coordinate, and $\theta,\phi$ the usual polar and azimuthal angles. With curvature normalized to $k=+1,0,-1$, $S(\chi)=\sin\chi,\chi,\sinh\chi$, respectively. Homogeneity and [isotropy](../../../../isotropy.md) apply to each constant-$t$ spatial slice. A comoving object's fixed coordinates do not imply a constant proper separation: spatial [lengths](../../../../length.md) scale with $R$.

Radial null propagation obeys $d\chi=c\,dt/R(t)$ in magnitude. Two neighbouring wave crests between the same comoving emitter and observer have the same radial integral, giving $\delta t_0/R_0=\delta t_e/R_e$. The [wavelength](../../../../wavelength.md) [redshift](../../../../redshift.md) is consequently

$$
\boxed{1+z=\frac{\lambda_0}{\lambda_e}=\frac{\delta t_0}{\delta t_e}=\frac{R_0}{R_e}.}
$$

Peculiar Doppler shifts are excluded by the comoving assumption. Define [angular diameter distance](../../../../angular-diameter-distance.md) by $d_\theta=\ell_\perp/\delta\theta$, where $\ell_\perp$ is proper transverse size at emission. The transverse metric gives $\ell_\perp=R_eS(\chi)\delta\theta$, hence

$$
\boxed{d_\theta=R_eS(\chi)=\frac{R_0S(\chi)}{1+z}.}
$$

This distance is neither the [photon](../../../../photon.md) travel [time](../../../../time-in-physics.md) [times](../../../../time-in-physics.md) $c$ nor the object's present proper distance.

The [comoving particle horizon](../../../../comoving-particle-horizon.md) at $t_1$, with the initial boundary at the [Big Bang](../../../../big-bang.md), is $\chi_p(t_1)=\int_0^{t_1}c\,dt/R(t)$. Its proper radial distance is $D_p=R(t_1)\chi_p$; for a power-law [scale factor](../../../../scale-factor-cosmology.md) $R=At^p$, $0<p<1$,

$$
\boxed{\chi_p=\frac{c\,t_1^{1-p}}{A(1-p)},\qquad D_p=\frac{ct_1}{1-p}.}
$$

Thus a matter-only flat [Einstein-de Sitter universe](../../../../einstein-de-sitter-universe.md), $p=2/3$, has $D_p=3ct_1$, and the flat radiation-only case, $p=1/2$, has $D_p=2ct_1$. Strictly, Einstein-de Sitter denotes the [pressureless matter](../../../../pressureless-matter.md) model; the radiation calculation uses the flat zero-$\Lambda$ radiation analogue requested here.

For the source seen at [time](../../../../time-in-physics.md) $t_1=t_{\rm rec}$, the radial coordinate is the integral from [recombination](../../../../recombination-cosmology.md) to today, not the earlier horizon integral. In these flat models,

$$
\chi_s=\frac{c}{A(1-p)}(t_0^{1-p}-t_1^{1-p}),\qquad
 d_\theta=\frac{ct_1^p}{1-p}(t_0^{1-p}-t_1^{1-p}).
$$

Taking the linear horizon scale in the question to be $D_p$, its small angular extent is

$$
\boxed{\theta_p=\frac{D_p}{d_\theta}
=\frac{(t_1/t_0)^{1-p}}{1-(t_1/t_0)^{1-p}}.}
$$

Therefore

$$
\boxed{\theta_{p,m}=\frac{(t_{\rm rec}/t_0)^{1/3}}{1-(t_{\rm rec}/t_0)^{1/3}},\qquad
\theta_{p,r}=\frac{(t_{\rm rec}/t_0)^{1/2}}{1-(t_{\rm rec}/t_0)^{1/2}}.}
$$

Using the supplied [times](../../../../time-in-physics.md) gives $\theta_{p,m}=0.02684\,\mathrm{rad}=1.54^\circ$ and $\theta_{p,r}=0.004244\,\mathrm{rad}=0.243^\circ$. There is a genuine radius/diameter convention to state: the supplied $3ct_1$ is a radial horizon distance. If angular diameter [means](../../../../expected-value-split.md) the full diameter of a spherical horizon patch of radius $D_p$, the two answers are instead **$2\theta_{p,m}=3.08^\circ$ and $2\theta_{p,r}=0.486^\circ$**. Both conventions follow from the same distance calculation; a factor of two should not be hidden in the word horizon.

Matter-only evolution is the better of these two approximations because the universe is already matter dominated around [recombination](../../../../recombination-cosmology.md) and evolves mostly through a subsequent matter era, rather than remaining radiation dominated to the present. Neither is exact: pre-recombination radiation changes the [particle horizon](../../../../particle-horizon.md), and late-time [dark energy](../../../../dark-energy.md) changes the distance to the last-scattering surface. No supplied ages have been replaced by later best-fit values.

The [cosmic microwave background](../../../../cosmic-microwave-background-split.md) originates near last scattering and samples many horizon-sized regions. In an always-decelerating hot-Big-Bang model, widely separated last-scattering patches lack overlapping early causal histories, motivating the [horizon problem](../../../../horizon-problem.md). The measured acoustic angular scale uses the smaller [sound horizon](../../../../sound-horizon.md), not automatically this light-travel [particle horizon](../../../../particle-horizon.md); baryon-photon pressure changes the propagation speed. Inflation supplies an earlier accelerated expansion during which the [comoving Hubble radius](../../../../comoving-hubble-radius.md) shrinks, allowing a patch with a common earlier causal history to expand to the size of the observable universe. Quantum perturbations can then seed later acoustic and density fluctuations. This does not require local [signals](../../../../signal.md) to propagate faster than light, and the [Hubble radius](../../../../hubble-radius.md) must not be equated indiscriminately with the [particle horizon](../../../../particle-horizon.md). CMB [temperature](../../../../temperature-split.md) and lensing spectra test the resulting perturbation and expansion model.[abstract; temperature/lensing spectra and the spatially flat standard cosmological model](../../../../planck-2013-results-xvi-cosmological-parameters-by-planck-collaboration.md)

<a id="2/image-original-horizon-length-angular-extents-in-the-two-stated-power-law-cosmologies-full-patch-diameters-are-twice-the-plotted-values"></a>
![](../../../../past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2014/paper-1-horizon-angles.png)

**[Figure 1](#2/image-original-horizon-length-angular-extents-in-the-two-stated-power-law-cosmologies-full-patch-diameters-are-twice-the-plotted-values). Original horizon-length angular extents in the two stated power-law cosmologies; full patch diameters are twice the plotted values**.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../split.md)
5. [Relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../../relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
