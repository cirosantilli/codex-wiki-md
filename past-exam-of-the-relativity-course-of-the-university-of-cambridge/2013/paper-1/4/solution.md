<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**[redshift](../../../../redshift.md).** An incoming radial null ray satisfies $d\chi=-c\,dt/R(t)$. Consecutive wave crests follow the same comoving path, so the endpoint changes in the fixed path [integral](../../../../integral-split.md) obey $dt_0/R_0=dt_e/R_e$. Comoving clocks read [cosmic time](../../../../cosmic-time.md); hence their measured periods and frequencies satisfy

$$
\boxed{1+z=\frac{\lambda_0}{\lambda_e}=\frac{dt_0}{dt_e}=\frac{R_0}{R_e}}.
$$

The physical [wavelength](../../../../wavelength.md) stretches with the [scale factor](../../../../scale-factor-cosmology.md) during propagation. It is not necessary to assign a unique global inertial-frame recession [velocity](../../../../velocity.md) to a distant source.

**Radial coordinate and [cosmological look-back time](../../../../cosmological-look-back-time.md).** Differentiating $1+z=R_0/R(t)$ gives $dz/dt=-(1+z)H(z)$. Combining this with the null-ray [integral](../../../../integral-split.md) yields

$$
\boxed{\chi(z)=\frac c{R_0}\int_0^z\frac{d\bar z}{H(\bar z)},\qquad
t_0-t_e=\int_0^z\frac{d\bar z}{(1+\bar z)H(\bar z)}}.
$$

The extra factor $1+z$ in the second denominator records the conversion from scale-factor change to elapsed [cosmic time](../../../../cosmic-time.md).

**[proper-motion distance](../../../../proper-motion-distance.md).** A small transverse displacement at emission has proper length $d\ell=R_eS(\chi)d\theta$. Define its source-frame transverse speed as $v=d\ell/dt_e$; [cosmological time dilation](../../../../cosmological-time-dilation.md) makes $dt_0=(1+z)dt_e$. Therefore

$$
\dot\theta_0=\frac{v}{(1+z)R_eS(\chi)},\qquad
\boxed{d_M=\frac v{\dot\theta_0}=R_0S(\chi(z))}.
$$

Equivalently, $d_M=(1+z)d_A$, where the [angular diameter distance](../../../../angular-diameter-distance.md) is $d_A=R_eS(\chi)$. The observer-time versus source-time distinction is essential. This calculation uses the stated transverse speed convention and the homogeneous background, without additional peculiar radial [relativistic Doppler effect](../../../../relativistic-doppler-effect.md) or [gravitational lensing](../../../../gravitational-lensing-split.md).

**[redshift shell volume at the present epoch](../../../../redshift-shell-volume-at-the-present-epoch.md).** The induced spatial [metric tensor](../../../../metric-tensor.md) on the present slice gives $dV_0=R_0^3S^2(\chi)d\chi\,d\Omega$. Since $d\chi/dz=c/(R_0H)$,

$$
\boxed{dV_0=\frac{cR_0^2S^2(\chi(z))}{H(z)}\,dz\,d\Omega
=\frac{cd_M^2(z)}{H(z)}\,dz\,d\Omega}.
$$

This is the volume at the present epoch of the comoving shell intersected by the past [light cone](../../../../light-cone.md). Its proper volume at emission is smaller by $(1+z)^3$; a conserved population's proper [number density](../../../../number-density.md) is larger by the same factor, preserving its count.

**[Einstein-de Sitter cumulative number counts](../../../../einstein-de-sitter-cumulative-number-counts.md).** In flat geometry $S(\chi)=\chi$. Inserting the stated [Hubble parameter](../../../../hubble-parameter.md) into the radial [integral](../../../../integral-split.md) gives

$$
d_M(z)=\frac{2c}{H_0}\left[1-(1+z)^{-1/2}\right].
$$

The constant present-volume [number density](../../../../number-density.md) makes $dN=n_0dV_0$. With no members of the population before its formation epoch,

$$
\boxed{N=\frac{4c^3n_0}{H_0^3}\int_0^{z_f}
\frac{[1-(1+z)^{-1/2}]^2}{(1+z)^{3/2}}\,dz}.
$$

As an independent check, substitution $u=(1+z)^{-1/2}$ evaluates this to

$$
\boxed{N=\frac{8c^3n_0}{3H_0^3}\left[1-(1+z_f)^{-1/2}\right]^3
=\frac{n_0d_M^3(z_f)}3}.
$$

This is exactly the Euclidean [comoving volume](../../../../comoving-volume.md) per unit [solid angle](../../../../solid-angle.md) in the flat model. It assumes a complete count with the specified fixed population; [luminosity](../../../../luminosity.md) selection, mergers or subsequent number-density evolution would require additional factors.

<a id="4/image-original-einstein-de-sitter-proper-motion-and-angular-diameter-distances-differential-counts-and-cumulative-fraction"></a>
![](../../../../past-exam-of-the-relativity-course-of-the-university-of-cambridge/2013/paper-1-eds-distance-counts.png)

**[Figure 3](#4/image-original-einstein-de-sitter-proper-motion-and-angular-diameter-distances-differential-counts-and-cumulative-fraction). Original Einstein-de Sitter proper-motion and angular diameter distances, differential counts and cumulative fraction**.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
