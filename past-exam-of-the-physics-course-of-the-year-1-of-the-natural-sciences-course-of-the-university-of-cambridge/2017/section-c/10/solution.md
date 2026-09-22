<h1 id="section-c/10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

Expand the cloud's [potential energy](../../../../potential-energy.md) about a [stable equilibrium](../../../../stable-equilibrium.md): $U(z)=U(0)+U'(0)z+U''(0)z^2/2+\cdots$. Equilibrium gives $U'(0)=0$, stability gives $U''(0)=k>0$, and reflection symmetry also removes odd terms. For small displacements, $U-U(0)\simeq kz^2/2$ and $F=-dU/dz\simeq-kz$.

Including the electric and damping forces, [Newton's second law](../../../../newton-s-second-law.md) is $m\ddot z=qE(t)-b\dot z-kz$. Dividing by $m$ gives the [Lorentz oscillator model](../../../../lorentz-oscillator-model.md)

$$
\boxed{\ddot z+2\gamma\dot z+\omega_0^2z=\frac qmE(t),\qquad \omega_0=\sqrt{\frac km},\quad \gamma=\frac b{2m}.}
$$

The specified convention uses $2\gamma$ as the damping coefficient per unit [mass](../../../../mass.md).

For the steady response, represent the field by $E_0e^{i\omega t}$ and the displacement by $\widetilde z e^{i\omega t}$, taking real parts for physical quantities. Substitution gives

$$
(\omega_0^2-\omega^2+2i\gamma\omega)\widetilde z=\frac{qE_0}{m},\qquad \widetilde z=\frac{qE_0/m}{\omega_0^2-\omega^2+2i\gamma\omega}.
$$

Define the nonnegative [amplitude](../../../../wave-amplitude.md) $z_0=|\widetilde z|$ and $\delta=\operatorname{atan2}(2\gamma\omega,\omega_0^2-\omega^2)$. Then

$$
\boxed{z_0=\frac{|q|E_0/m}{\sqrt{(\omega_0^2-\omega^2)^2+4\gamma^2\omega^2}},\qquad \phi=\arg q-\delta\pmod{2\pi}.}
$$

For positive $q$, $\phi=-\delta$. For electrons $q<0$, the [phase of a negatively charged driven oscillator](../../../../phase-of-a-negatively-charged-driven-oscillator.md) is $\phi=\pi-\delta$: the low-[frequency](../../../../frequency.md) displacement is opposite to the field, rather than in [phase](../../../../phase-waves.md) with it. A signed [amplitude](../../../../wave-amplitude.md) could absorb this extra $\pi$, but the [phase](../../../../phase-waves.md) convention must then be stated. The induced dipole $p=qz$ has [phase](../../../../phase-waves.md) $-\delta$ for either charge sign. Transient free oscillations have been omitted because the question asks for steady state.

For the electron cloud, $q/m=-e/m_e$ and

$$
\omega_0=\sqrt{\frac{k/n}{m_e}}=\sqrt{\frac{100}{9.109\times10^{-31}}}=1.05\times10^{16}\,\mathrm{rad\,s^{-1}}.
$$

The visible range corresponds to $\omega=2\pi c/\lambda$ between $2.35\times10^{15}$ and $4.71\times10^{15}\,\mathrm{rad\,s^{-1}}$, below this [resonance](../../../../resonance.md). The resonant [wavelength](../../../../wavelength.md) is about $180\,\mathrm{nm}$, in the ultraviolet.

The [acceleration](../../../../acceleration.md) [amplitude](../../../../wave-amplitude.md) is $\omega^2z_0$. At fixed incident field [amplitude](../../../../wave-amplitude.md), the scattered intensity is therefore proportional to

$$
\boxed{I_{\mathrm{sc}}(\omega)\propto\frac{\omega^4}{(\omega_0^2-\omega^2)^2+4\gamma^2\omega^2}.}
$$

Well below [resonance](../../../../resonance.md) and outside strong damping corrections, $z_0$ is nearly [frequency](../../../../frequency.md)-independent and this becomes the [Rayleigh scattering wavelength dependence](../../../../rayleigh-scattering-wavelength-dependence.md) $I_{\mathrm{sc}}\propto\omega^4\propto\lambda^{-4}$. The shortest visible wavelengths are consequently scattered much more strongly into directions away from the direct solar beam than the longest ones, producing a blue sky. The simple fourth-power approximation gives a factor 16 between 400 and 800 nm at equal incident intensity. Retaining the undamped denominator with the given [resonance](../../../../resonance.md) raises that factor to about 22.7, since the upper end is not extremely far below [resonance](../../../../resonance.md). The exact ratio needs the unspecified damping and incident solar spectrum; the stronger scattering of the blue end is the robust conclusion here.

<a id="section-c/10/image-bound-charge-response-below-an-ultraviolet-resonance-favors-short-visible-wavelengths"></a>
![](../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017-bound-charge-scattering.png)

**[Figure 2](#section-c/10/image-bound-charge-response-below-an-ultraviolet-resonance-favors-short-visible-wavelengths). Bound-charge response below an ultraviolet resonance favors short visible wavelengths**.

The model describes [frequency](../../../../frequency.md)-dependent scattering, not the detailed perceived color after solar-spectrum weighting and human visual response. It also explains why treating the electrons as free at visible frequencies would miss the bound-charge fourth-power limit.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Section C](../../section-c.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
