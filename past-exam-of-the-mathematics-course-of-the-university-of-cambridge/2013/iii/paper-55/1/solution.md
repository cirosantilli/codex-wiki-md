<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $\delta=(\rho-\bar\rho)/\bar\rho$ and define the [cosmological density power spectrum](../../../../../matter-power-spectrum.md) by $\langle\delta_{\mathbf k}\delta_{\mathbf k'}^*\rangle=(2\pi)^3\delta_{\rm D}(\mathbf k-\mathbf k')P(k)$. The contribution per logarithmic wave-number interval is the [dimensionless cosmological power spectrum](../../../../../dimensionless-cosmological-power-spectrum.md) $\Delta^2(k)=k^3P(k)/(2\pi^2)$. The linear [cosmological mass variance](../../../../../smoothed-matter-density-variance.md) on mass scale $M$ is

$$
\sigma^2(M,z)=\int_0^\infty\Delta^2(k,z)|W(kR)|^2d\ln k,\qquad M=\frac{4\pi}{3}\bar\rho_{m,0}R^3,
$$

with $R$ a comoving smoothing radius and $W$ the [top-hat filter](../../../../../top-hat-filter.md) in Fourier space. On halo scales the observed spectrum is consistent with greater variance at smaller masses. Growth therefore brings smaller objects to the collapse threshold earlier, statistically; larger structures assemble by accretion and [dark-matter halo mergers](../../../../../dark-matter-halo-merger.md). **This statistical growth from smaller bound systems to larger ones is [hierarchical galaxy formation](../../../../../hierarchical-galaxy-formation.md).** It is an ordering of dark-matter assembly, not a rule that every small visible galaxy must precede every large visible galaxy.

For linear modes the [linear growth factor](../../../../../linear-growth-factor.md) gives $P(k,z)=D^2(z)P(k,0)$. During matter domination $D\propto a$, so $P\propto a^2$ and the characteristic nonlinear mass increases. Once modes become nonlinear, coupling between scales and halo formation change the shape, so the same multiplication cannot be used for the entire late-time spectrum. At low redshift accelerated expansion suppresses linear growth. Galaxy clustering traces the matter spectrum with [galaxy bias](../../../../../galaxy-bias.md); it should not be equated directly with an unbiased matter measurement.

The broad linear shape was set by the [cosmological transfer function](../../../../../cosmological-transfer-function.md) before and around [matter-radiation equality](../../../../../matter-radiation-equality.md), with baryonic acoustic structure also imprinted before recombination. A nearly scale-invariant primordial curvature spectrum has $\mathcal P_{\mathcal R}(k)\propto k^{n_s-1}$, with $n_s$ close to one. After converting curvature perturbations to matter-density perturbations,

$$
P_{\rm lin}(k,z)\propto D^2(z)k^{n_s}T^2(k).
$$

Thus nearly scale-invariant primordial curvature does not mean a constant density $P(k)$. Modes with $k\ll k_{\rm eq}$ enter the horizon after equality and have $T\simeq1$. Modes with $k\gg k_{\rm eq}$ enter during radiation domination, when radiation controls the expansion and cold-matter perturbations grow only slowly. The [cold-dark-matter transfer function](../../../../../cold-dark-matter-transfer-function.md) behaves approximately as $T\propto\ln(k/k_{\rm eq})/(k/k_{\rm eq})^2$ at large $k$. Hence the density spectrum turns over near $k_{\rm eq}=a_{\rm eq}H_{\rm eq}/c$:

$$
P(k)\propto k^{n_s}\quad(k\ll k_{\rm eq}),\qquad
P(k)\propto k^{n_s-4}\ln^2(k/k_{\rm eq})\quad(k\gg k_{\rm eq}).
$$

The turnover records the equality horizon, while the late nonlinear excess records gravitational clustering. On galactic scales the effective slope is greater than $-3$, giving the growing small-scale variance needed for [hierarchical galaxy formation](../../../../../hierarchical-galaxy-formation.md).

[Cold dark matter](../../../../../cold-dark-matter.md) has negligible primordial thermal velocities and a very short [collisionless free streaming](../../../../../free-streaming.md) length on galactic scales. [Warm dark matter](../../../../../warm-dark-matter.md) has appreciable residual velocities while structure is being seeded; particles stream across small fluctuations and reduce their contrast. Its [cosmological transfer function](../../../../../cosmological-transfer-function.md) is consequently cut off below a characteristic length, suppressing low-mass halos and delaying their formation. Above that cutoff its assembly can still be hierarchical. **The important distinction is the free-streaming scale, rather than the present temperature or an arbitrary particle-mass label.**

Linear evolution assumes $|\delta|\ll1$. When $\delta$ becomes of order unity, overdense regions depart strongly from the Hubble flow and can turn around and collapse. Collisionless [dark matter](../../../../../dark-matter.md) develops multistream motion after trajectories cross; gravitational mixing redistributes energy and produces a bound [dark matter halo](../../../../../dark-matter-halo.md). The formal infinite-density collapse of an ideal spherical pressureless solution is not the physical endpoint. A roughly virialized halo has $2K+W\simeq0$ and a characteristic [virial velocity](../../../../../virial-velocity-of-a-spherical-overdensity-halo.md) $V_{\rm vir}^2=GM_h/r_{\rm vir}$. Its gas [virial temperature](../../../../../virial-temperature.md) is conventionally

$$
\boxed{k_BT_{\rm vir}\simeq\frac{\mu m_p}{2}V_{\rm vir}^2\simeq\frac{\mu m_pGM_h}{2r_{\rm vir}}.}
$$

It measures the thermal energy associated with the gravitational potential; the numerical factor depends on the velocity-dispersion convention. It does not imply that the collisionless dark matter has a thermodynamic gas temperature.

The unheaded request about [baryon conversion efficiency of a halo](../../../../../baryon-conversion-efficiency-of-a-halo.md) is also answered here. Define $f_*=M_{\rm stars}/(f_bM_h)$ using the [cosmic baryon fraction](../../../../../cosmic-baryon-fraction.md) $f_b$. In small halos, shallow potentials let [stellar feedback](../../../../../stellar-feedback.md) drive outflows or repeatedly heat star-forming gas; supernova energy per stellar mass is roughly fixed while binding energy per gas mass scales as $V_{\rm vir}^2$. Photoheating during [reionization](../../../../../reionization.md) also prevents very small halos from retaining or accreting cool gas. Molecular/atomic cooling thresholds further reduce star formation in the smallest systems. These effects make $f_*$ fall toward low mass.

Near $M_h\sim10^{12}M_\odot$, gas can cool efficiently and the potential is deep enough to retain more of it, while a long-lived hot atmosphere and maintenance heating are less effective than in larger systems. At high mass, higher [virial temperature](../../../../../virial-temperature.md) and lower cooling efficiency let a substantial hot atmosphere persist. [Active-galactic-nucleus feedback](../../../../../active-galactic-nucleus-feedback.md) can prevent that atmosphere from supplying cold gas and can expel some gas; the cooling-time bottleneck alone is not an adequate explanation for the low stellar fractions of massive groups and clusters. **The peak reflects a competition between gas supply/cooling and feedback, rather than complete conversion of all baryons at a sharply universal mass.** Its exact location and height depend on epoch, metallicity, gas history and the stellar population included.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
