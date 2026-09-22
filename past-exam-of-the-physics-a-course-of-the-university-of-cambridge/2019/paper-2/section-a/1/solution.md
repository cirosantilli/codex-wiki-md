<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Build a narrow-band [wave packet](../../../../../wave-packet.md) from [plane waves](../../../../../plane-wave.md) with [wavenumbers](../../../../../wavenumber.md) close to $k_0$:

$$
\psi(x,t)=\int A(k)e^{i[kx-\omega(k)t]}\,dk.
$$

The [Taylor expansion](../../../../../taylor-expansion.md) of the [dispersion relation](../../../../../dispersion-relation-split.md) is $\omega(k)\simeq\omega_0+\omega'_0(k-k_0)$, where $\omega'_0=(d\omega/dk)_{k_0}$. Put $\kappa=k-k_0$ to obtain

$$
\psi(x,t)\simeq e^{i(k_0x-\omega_0t)}
\int A(k_0+\kappa)e^{i\kappa(x-\omega'_0t)}\,d\kappa
=e^{i(k_0x-\omega_0t)}f(x-\omega'_0t).
$$

The carrier's [wave phase](../../../../../phase-waves.md) travels at the [phase velocity](../../../../../phase-velocity.md) $\omega_0/k_0$, while the envelope has constant shape at constant $x-\omega'_0t$. Its [group velocity](../../../../../group-velocity.md) is therefore

$$
\boxed{v_g=\left.\frac{d\omega}{dk}\right|_{k_0}.}
$$

The approximation neglects higher derivatives of the [dispersion relation](../../../../../dispersion-relation-split.md). Those derivatives cause the [wave packet](../../../../../wave-packet.md) to spread or distort over sufficiently long propagation times; the result describes the local envelope speed of a sufficiently narrow band.

## ↑ Ancestors (14)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
