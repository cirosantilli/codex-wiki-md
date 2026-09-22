<h1 id="section-b/b7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An incident [electromagnetic wave](../../../../../../electromagnetic-wave-split.md) generally produces reflected and transmitted waves because the two media have different electromagnetic response. Consider a flat interface between homogeneous, linear, lossless media with [permittivities](../../../../../../permittivity-split.md) $\epsilon_j$ and [magnetic permeabilities](../../../../../../permeability-electromagnetism.md) $\mu_j$. Their wave speeds and [wave impedances](../../../../../../wave-impedance.md) are

$$
v_j=\frac1{\sqrt{\mu_j\epsilon_j}},\qquad Z_j=\sqrt{\frac{\mu_j}{\epsilon_j}}.
$$

For each [plane electromagnetic wave](../../../../../../plane-electromagnetic-wave.md), $\mathbf H=\hat{\mathbf k}\times\mathbf E/Z_j$. With no [free surface](../../../../../../free-surface.md) charge or current, the [interface conditions for electromagnetic fields](../../../../../../interface-conditions-for-electromagnetic-fields.md) require continuous tangential $\mathbf E,\mathbf H$ and normal $\mathbf D,\mathbf B$. Equality of the [phase](../../../../../../phase-waves.md) at every point on the boundary gives equal [angular frequencies](../../../../../../angular-frequency.md) and tangential [wavevectors](../../../../../../wavevector.md). Hence the reflection [angle](../../../../../../angle.md) equals the incidence [angle](../../../../../../angle.md) and [Snell's law](../../../../../../snell-s-law.md) is

$$
n_1\sin\theta_i=n_2\sin\theta_t,
$$

where $n_j=c/v_j$ and each [angle](../../../../../../angle.md) is measured from the normal.

At normal incidence use the same tangential axis for all electric [amplitudes](../../../../../../wave-amplitude.md). The two independent boundary equations are

$$
E_i+E_r=E_t,\qquad \frac{E_i-E_r}{Z_1}=\frac{E_t}{Z_2}.
$$

Solving gives the [amplitude](../../../../../../wave-amplitude.md) [Fresnel equations](../../../../../../fresnel-equations.md)

$$
\boxed{r=\frac{E_r}{E_i}=\frac{Z_2-Z_1}{Z_2+Z_1},\qquad t=\frac{E_t}{E_i}=\frac{2Z_2}{Z_1+Z_2}.}
$$

For nonmagnetic media, these become $r=(n_1-n_2)/(n_1+n_2)$ and $t=2n_1/(n_1+n_2)$. Reflection into a medium of larger [refractive index](../../../../../../refractive-index.md) therefore reverses the electric [amplitude](../../../../../../wave-amplitude.md)'s sign at normal incidence.

The normal [Poynting vector](../../../../../../poynting-vector.md) determines the reflected and transmitted fractions of incident [power](../../../../../../power.md). At normal incidence,

$$
\mathcal R=|r|^2,\qquad \mathcal T=\frac{Z_1}{Z_2}|t|^2,\qquad
\boxed{\mathcal R+\mathcal T=1.}
$$

It is the [power](../../../../../../power.md) fractions, rather than the squared electric [amplitudes](../../../../../../wave-amplitude.md) alone, that add to unity.

At oblique incidence separate [transverse electric polarization](../../../../../../transverse-electric-polarization.md) ($s$, [electric field](../../../../../../electric-field-split.md) perpendicular to the incidence plane) from [transverse magnetic polarization](../../../../../../transverse-magnetic-polarization.md) ($p$, [electric field](../../../../../../electric-field-split.md) in that plane). For nonmagnetic media, writing $c_i=\cos\theta_i$ and $c_t=\cos\theta_t$, the [Fresnel equations](../../../../../../fresnel-equations.md) are

$$
r_s=\frac{n_1c_i-n_2c_t}{n_1c_i+n_2c_t},\qquad
t_s=\frac{2n_1c_i}{n_1c_i+n_2c_t},
$$



$$
r_p=\frac{n_2c_i-n_1c_t}{n_2c_i+n_1c_t},\qquad
t_p=\frac{2n_1c_i}{n_2c_i+n_1c_t}.
$$

Here choose a common $s$ direction and, for each ray, the $p$ direction as $\hat{\mathbf s}\times\hat{\mathbf k}$. This makes the reflected $p$ basis reverse its tangential direction at normal incidence, explaining why the displayed $r_p$ then has the opposite sign to $r_s$. Physical [reflectance](../../../../../../reflectance.md) is independent of this sign convention. For either polarization with propagating transmission,

$$
\mathcal R=|r|^2,\qquad \mathcal T=\frac{n_2\cos\theta_t}{n_1\cos\theta_i}|t|^2.
$$

For $p$ polarization, zero reflection occurs at the [Brewster angle](../../../../../../brewster-s-angle.md) $\tan\theta_B=n_2/n_1$. If $n_1>n_2$, incidence above the [critical angle for total internal reflection](../../../../../../critical-angle-for-total-internal-reflection.md) $\sin\theta_c=n_2/n_1$ produces an [evanescent field in total internal reflection](../../../../../../evanescent-field-in-total-internal-reflection.md) and $\mathcal R=1$ for an isolated lossless interface. A lossy second medium requires complex response coefficients and an absorption term in the [energy](../../../../../../energy-split.md) balance.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [B7](../../b7.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
