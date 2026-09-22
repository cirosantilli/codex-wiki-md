<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

Write the real [displacement](../../../../../displacement.md) as $U_n(t)=\operatorname{Re}[u e^{i\omega t-iqna}]$, choosing real positive peak amplitude $u$. Nearest-neighbour harmonic springs store [energy](../../../../../energy-split.md) in their extension $U_n-U_{n+1}$, each spring counted once. Therefore the instantaneous physical [energy](../../../../../energy-split.md) is

$$
\boxed{E=\frac12M\sum_n\dot U_n^2+\frac12\alpha\sum_n(U_n-U_{n+1})^2.}
$$

The printed complex [displacement](../../../../../displacement.md) is a calculation device: squaring the complex [phasor](../../../../../phasor.md) itself would not produce physical [energy](../../../../../energy-split.md). The chain sketch in the accompanying figure shows [masses](../../../../../mass.md) at [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) spacing $a$, with longitudinal [displacements](../../../../../displacement.md) along the chain.

The two spring [forces](../../../../../force-split.md) on site $n$ give

$$
M\ddot U_n=\alpha(U_{n+1}+U_{n-1}-2U_n).
$$

Substituting the normal-mode [phasor](../../../../../phasor.md) and cancelling its nonzero amplitude gives

$$
-M\omega^2=\alpha(e^{iqa}+e^{-iqa}-2),\qquad
\boxed{\omega^2=\frac{4\alpha}{M}\sin^2\left(\frac{qa}{2}\right).}
$$

The long-wavelength limit is acoustic, $\omega\simeq a\sqrt{\alpha/M}|q|$, and the first [Brillouin zone](../../../../../brillouin-zone.md) ends at $|q|=\pi/a$. The maximum [angular frequency](../../../../../angular-frequency.md) is **$\omega_m=2\sqrt{\alpha/M}$**.

Time averaging uses $\langle[\operatorname{Re}(ze^{i\omega t})]^2\rangle=|z|^2/2$. Consequently

$$
\frac{\langle T\rangle}{N}=\frac14M\omega^2u^2,\qquad
\frac{\langle V\rangle}{N}=\frac14\alpha u^2|1-e^{-iqa}|^2
=\frac12\alpha(1-\cos qa)u^2.
$$

The [dispersion relation](../../../../../dispersion-relation-split.md) makes these two contributions equal, giving

$$
\boxed{\langle E\rangle/N=\frac14M\omega^2u^2+
\frac12\alpha(1-\cos qa)u^2=\frac12M\omega^2u^2.}
$$

This is equality of time-averaged kinetic and [potential energies](../../../../../potential-energy.md) in a harmonic [normal mode](../../../../../normal-mode.md); the instantaneous [energy](../../../../../energy-split.md) partition need not be equal.

Use [periodic boundary conditions](../../../../../periodic-boundary-conditions.md) on length $L=Na$ to count modes: $q_j=2\pi j/L$. The density on the signed $q$ axis is $L/(2\pi)$. Using [folded wave-number counting for a monatomic chain](../../../../../folded-wave-number-counting-for-a-monatomic-chain.md) combines $q$ and $-q$ at positive magnitude and counts both directions, so the convention used by the requested expression is

$$
\boxed{g(q)=\frac{2L}{2\pi}=\frac{Na}{\pi},\quad 0<q<\pi/a.}
$$

This is a large-$N$ continuum density, not a second independent branch. It gives $N$ modes after integrating over that half-zone; endpoint counting changes only finite-size corrections.

For positive $q$, $\omega=\omega_m\sin(qa/2)$ and

$$
\frac{d\omega}{dq}=\frac a2\sqrt{\omega_m^2-\omega^2},\qquad
\boxed{g(\omega)=g(q)\left|\frac{dq}{d\omega}\right|
=\frac{2N}{\pi\sqrt{\omega_m^2-\omega^2}},\quad0<\omega<\omega_m.}
$$

The [density of states of a monatomic harmonic chain](../../../../../density-of-states-of-a-monatomic-harmonic-chain.md) vanishes outside the band, is constant to leading order near zero, and has an integrable [Van Hove singularity](../../../../../van-hove-singularity.md) at the upper band edge where [group velocity](../../../../../group-velocity.md) vanishes. Normalization checks the directional counting:

$$
\int_0^{\omega_m}g(\omega)\,d\omega
=\frac{2N}{\pi}[\arcsin(\omega/\omega_m)]_0^{\omega_m}=N.
$$

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
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
