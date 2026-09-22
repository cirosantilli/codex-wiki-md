<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Normalize the [linear growth factor](../../../../../linear-growth-factor.md) to $D(0)=1$. The collapse overdensity at the collapse epoch is $\delta_{\rm sc}\simeq1.686$ for the matter-dominated [spherical-collapse model](../../../../../spherical-collapse-model.md). The [present-extrapolated spherical-collapse barrier](../../../../../present-extrapolated-spherical-collapse-barrier.md) is

$$
\boxed{\delta_c(t)=\frac{\delta_{\rm sc}}{D(t)}.}
$$

It is the initial linear overdensity, extrapolated to today, required to collapse by $t$; it is not the nonlinear [density contrast](../../../../../density-contrast.md) of a virialized halo. The [smoothed matter density variance](../../../../../smoothed-matter-density-variance.md) $\sigma^2(M,z)$ is the variance of the linear [density contrast](../../../../../density-contrast.md) smoothed on a Lagrangian comoving scale containing mass $M$. For a spherical [top-hat filter](../../../../../top-hat-filter.md),

$$
M=\frac{4\pi}3\bar\rho_{m,0}R^3,\qquad
\sigma^2(M,z)=\frac1{2\pi^2}\int_0^\infty k^2P(k,z)|W(kR)|^2dk,
\quad W(x)=3\frac{\sin x-x\cos x}{x^3}.
$$

Consequently $\sigma(M,z)=D(z)\sigma(M,0)$ for scale-independent linear growth. The equivalent [halo peak height](../../../../../halo-peak-height.md) conventions are $\nu=\delta_c(t)/\sigma(M,0)=\delta_{\rm sc}/\sigma(M,z)$; using both an evolved barrier and an evolved variance would count growth twice.

To calculate a number-density growth time, use a narrow fixed-mass bin, not the collapsed mass fraction itself. Differentiate the [Press-Schechter formalism](../../../../../press-schechter-formalism.md) mass fraction and divide the mass density in the resulting interval by $M$. This gives the [Press-Schechter halo mass function](../../../../../press-schechter-halo-mass-function.md)

$$
\frac{dn}{dM}=\sqrt{\frac2\pi}\frac{\bar\rho_{m,0}}{M^2}
\left|\frac{d\log\sigma(M,0)}{d\log M}\right|\nu e^{-\nu^2/2}.
$$

At fixed $M$, the mass factor and logarithmic slope do not depend on time. Since $\dot\nu/\nu=-\dot D/D$, the [Press-Schechter abundance growth at fixed mass](../../../../../press-schechter-abundance-growth-at-fixed-mass.md) is

$$
\boxed{\frac{\partial\log n}{\partial t}\bigg|_M=(\nu^2-1)\frac{\dot D}{D},\qquad
t_d=\left[(\nu^2-1)\frac{\dot D}{D}\right]^{-1}.}
$$

The prefactor $\nu$ matters here: the exponential-only rare-peak approximation drops the minus one and is accurate only for $\nu\gg1$.

Read the supplied variance relation as a mass-scale calibration using the numerical velocity label given for the selected population. It gives $\sigma(M,3)=0.85\sqrt{250/10}=4.25$. Matter domination between the two high-redshift epochs gives $D(19)/D(3)\simeq4/20$, so $\sigma(M,19)\simeq0.85$ and $\nu\simeq1.984$. At the epoch in question,

$$
H(19)=H_0\sqrt{0.25(20)^3+0.75},\qquad
H^{-1}(19)\simeq3.19\times10^8\,\mathrm{yr},\qquad \dot D/D\simeq H.
$$

Thus the requested fixed-mass-bin growth estimate with that calibration is

$$
\boxed{t_d\simeq\frac{3.19\times10^8}{(1.686/0.85)^2-1}\,\mathrm{yr}
\simeq1.09\times10^8\,\mathrm{yr}.}
$$

An exponential-only approximation gives about $8.1\times10^7\,\mathrm{yr}$, which is somewhat shorter because this is only a roughly two-sigma population.

The wording leaves two sample conventions worth distinguishing. First, an actual [virial velocity of a spherical-overdensity halo](../../../../../virial-velocity-of-a-spherical-overdensity-halo.md) is epoch-dependent at fixed mass. If the variance fit is instead calibrated using physical virial velocities at redshift three, the same mass whose velocity is $10\,\mathrm{km\,s^{-1}}$ at redshift nineteen has $v(3)\simeq10\sqrt{4/20}=4.47\,\mathrm{km\,s^{-1}}$. The [halo virial-velocity conversion between epochs](../../../../../halo-virial-velocity-conversion-between-epochs.md) then gives $\sigma(M,19)\simeq1.271$, $\nu\simeq1.327$ and **$t_d\simeq4.2\times10^8\,\mathrm{yr}$** for a fixed-mass bin. The two numerical answers reflect the velocity-label convention in the supplied fit, not two ways of differentiating one fixed fit.

Second, a cumulative number density is $n(>M)=\int_M^\infty(dn/dM')dM'$, not simply $\bar\rho_{m,0}f(>M)/M$: the latter is a mass fraction divided by a threshold mass, not the number of objects. The cumulative derivative is an abundance-weighted average of $(\nu(M')^2-1)\dot D/D$ over that integral. If the supplied power-law variance fit is extended over all larger masses, with the same velocity-label convention, direct integration gives a cumulative-number growth time of about $8.4\times10^7\,\mathrm{yr}$ instead. A sample maintained at fixed physical velocity at successive epochs additionally moves its mass boundary and needs a selection convention. The numerical estimate above explicitly uses the ordinary fixed-mass differential interpretation. These distinctions are important when an exact growth time rather than a rare-tail estimate is intended.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
