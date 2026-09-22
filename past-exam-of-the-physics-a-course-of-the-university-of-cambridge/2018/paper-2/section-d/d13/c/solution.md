<h1 id="section-d/d13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [dispersion relation](../../../../../../dispersion-relation-split.md) specifies the allowed [angular frequency](../../../../../../angular-frequency.md) $\omega(k)$ of a [wavevector](../../../../../../wavevector.md) $k$. A single harmonic wave $A\cos(kx-\omega t)$ has constant-phase surfaces moving at the [phase velocity](../../../../../../phase-velocity.md),

$$
\boxed{v_p=\omega/k}.
$$

For two nearby components, use the identity

$$
\cos(k_1x-\omega_1t)+\cos(k_2x-\omega_2t)
=2\cos\!\left(\frac{\Delta k\,x-\Delta\omega\,t}{2}\right)
\cos(\bar kx-\bar\omega t).
$$

The slowly varying envelope moves at $\Delta\omega/\Delta k$. Taking a narrowband limit gives the [group velocity](../../../../../../group-velocity.md),

$$
\boxed{v_g=\frac{d\omega}{dk}=v_p+k\frac{dv_p}{dk}}.
$$

More generally, expand $\omega(k)$ around the central [wavevector](../../../../../../wavevector.md) of a wavepacket. The linear term translates its envelope at $v_g$; the quadratic and higher terms produce [group velocity dispersion](../../../../../../group-velocity-dispersion.md) and packet distortion. This interpretation needs a sufficiently narrow spectrum and weak enough absorption and distortion for an identifiable envelope to persist.

For light in a transparent material, $k=n(\omega)\omega/c$, so

$$
\boxed{v_p=\frac cn},\qquad
\boxed{v_g=\frac{c}{n+\omega\,dn/d\omega}
=\frac{c}{n-\lambda_0\,dn/d\lambda_0}}.
$$

The derivative is evaluated at the wavepacket's central [frequency](../../../../../../frequency.md) and $\lambda_0$ is the vacuum [wavelength](../../../../../../wavelength.md). In a nondispersive medium with constant $n$, the two velocities coincide and a packet can propagate without dispersion. In normal optical dispersion $dn/d\lambda_0<0$, the displayed model gives $v_g<v_p$.

The two velocities can differ even without material dispersion: a waveguide mode with $\omega^2=\omega_c^2+c^2k^2$ has $v_p=\omega/k>c$ and $v_g=c^2k/\omega<c$, with $v_pv_g=c^2$. The [phase velocity](../../../../../../phase-velocity.md) is not a signal speed. Near strongly absorbing resonances an anomalous derivative can also make the [group velocity](../../../../../../group-velocity.md) exceed $c$ or become negative; reshaping then prevents its simple identification with information transport. Relativistic causality constrains the signal front, not the speed of an arbitrary moving [phase](../../../../../../phase-waves.md) or distorted intensity maximum.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
