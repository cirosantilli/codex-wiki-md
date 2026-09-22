<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First fix a genuine normalization error in the original PDF: the Gaussian exponent uses $\sigma^2$, so $\sigma$ must be the [standard deviation](../../../../../../standard-deviation.md), the [variance](../../../../../../variance-split.md) is $\sigma^2$, and the normalized [probability density function](../../../../../../probability-density-function.md) is

$$
p_M(\delta)=\frac1{\sqrt{2\pi}\,\sigma(M,z)}
\exp\!\left(-\frac{\delta^2}{2\sigma^2(M,z)}\right).
$$

The printed prefactor has only $\sigma$ under its square root; its integral is $\sqrt{\sigma}$ rather than one. Use the normalized [normal distribution](../../../../../../normal-distribution.md) above.

The one-scale probability of exceeding the [linear spherical-collapse threshold](../../../../../../linear-spherical-collapse-threshold.md) is $P_M=\tfrac12\operatorname{erfc}[\delta_c/(\sqrt2\sigma)]$. In the [Press-Schechter formalism](../../../../../../press-schechter-formalism.md), the mass fraction above $M$ is assigned to

$$
F(>M,z)=2P_M=\operatorname{erfc}\!\left(\frac{\delta_c}{\sqrt2\sigma(M,z)}\right).
$$

The factor two is necessary to recover all the mass in the hierarchical limit $\sigma\to\infty$: the uncorrected one-point upper tail tends to only one half. A precise justification is available in the [excursion-set description of halo formation](../../../../../../excursion-set-description-of-halo-formation.md) with a [sharp-k smoothing filter](../../../../../../sharp-k-smoothing-filter.md). The smoothed [Gaussian random field](../../../../../../gaussian-random-field.md) then becomes [Brownian motion](../../../../../../brownian-motion-split.md) in its variance $S$. Reflecting a trajectory after its first crossing of $\delta_c$ pairs trajectories which crossed but end below the threshold with those which end above it. The [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) therefore gives $\Pr(\max_{s\le S}\delta(s)>\delta_c)=2\Pr(\delta(S)>\delta_c)$.

This multiscale mass assignment is an extra modelling prescription: a Gaussian one-point probability and a collapse threshold alone do not mathematically determine a halo mass function. The “all matter” normalization additionally assumes arbitrarily large small-scale variance; a finite variance cutoff leaves an uncollapsed fraction.

Differentiate at fixed $z$ and fixed $\delta_c$:

$$
\frac{\partial F}{\partial M}
=\sqrt{\frac2\pi}\frac{\delta_c}{\sigma^2}
\exp\!\left(-\frac{\delta_c^2}{2\sigma^2}\right)\frac{\partial\sigma}{\partial M}.
$$

For decreasing $\sigma(M,z)$, a mass interval contains the positive fraction $-F'(M)\,dM$. Its comoving mass is $\rho_{m,0}[-F'(M)]\,dM$, so division by halo mass gives the [Press-Schechter halo mass function](../../../../../../press-schechter-halo-mass-function.md):

$$
\boxed{\frac{dn}{dM}=\sqrt{\frac2\pi}\frac{\rho_{m,0}}M
\frac{\delta_c}{\sigma^2(M,z)}\left|\frac{\partial\sigma(M,z)}{\partial M}\right|
\exp\!\left(-\frac{\delta_c^2}{2\sigma^2(M,z)}\right).}
$$

The absolute value, or equivalently a minus sign multiplying $\partial_M\sigma$, is essential for a positive abundance. The original PDF correctly places absolute values around the abundance and the full [derivative](../../../../../../derivative.md) expression; these bars are lost in the converted TeX. The [density](../../../../../../density.md) is comoving, so the prefactor uses today's matter [mass density](../../../../../../density.md), rather than the physical [density](../../../../../../density.md) at redshift $z$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
