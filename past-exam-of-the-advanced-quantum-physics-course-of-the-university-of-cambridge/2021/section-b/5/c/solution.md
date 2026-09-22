<h1 id="section-b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The only relevant position [matrix element](../../../../../matrix-element.md) is $z_{01}=\sqrt{\hbar/(2m\omega_0)}$. To first order in the radiation amplitude, the two ground–excited-state cross terms give

$$
\langle z\rangle_t=2\sqrt{\frac{\hbar}{2m\omega_0}}
\operatorname{Re}\left[e^{-i\omega_0t}b_1(t)\right].
$$

Multiplying by the charge $-e$ gives the induced [electric dipole moment](../../../../../electric-dipole-moment.md). Since $2\sqrt{\hbar/(2m\omega_0)}C=eA_0/m$, the coefficient derived in part (b) yields

$$
\mathbf P(t)=-\frac{e^2A_0}{m}\hat{\mathbf z}\operatorname{Re}\left[
 e^{i\theta}\frac{e^{-i\omega t}-e^{-i\omega_0t}}{i(\omega_0-\omega)}
+e^{-i\theta}\frac{e^{i\omega t}-e^{-i\omega_0t}}{i(\omega_0+\omega)}\right]
$$

at linear order. Taking the complex conjugate inside the real part of the second term changes it to minus the same term with $e^{i\theta}$ and reversed frequency signs. Thus

$$
\boxed{\mathbf P(t)=-\frac{e^2A_0}{m}\hat{\mathbf z}\operatorname{Re}\left[e^{iky}\left(
\frac{e^{-i\omega t}-e^{-i\omega_0t}}{i(\omega_0-\omega)}
-\frac{e^{-i\omega t}-e^{i\omega_0t}}{i(\omega_0+\omega)}\right)\right].}
$$

The terms at $\omega_0$ are switch-on transients, while those at $\omega$ describe the driven response. Both are needed to make $\mathbf P(0)=0$. The expression is understood by continuity at $\omega=\omega_0$; the first quotient then tends to $t e^{-i\omega_0t}$, producing resonant secular growth rather than an infinite dipole at a finite time.

There is also an initial-velocity check on this [harmonic-oscillator dipole response to switched radiation](../../../../../harmonic-oscillator-dipole-response-to-switched-radiation.md). The formula gives $\dot P_z(0^+)=-2e^2A_0\cos(ky)/m$. Because the [magnetic vector potential](../../../../../magnetic-vector-potential.md) jumps at zero time, its time derivative contains an impulsive [electric field](../../../../../electric-field-split.md). Equivalently, the mechanical velocity is $(p_z+eA_z)/m$, whose initial mean is $2eA_0\cos(ky)/m$. The transient therefore implements the specified switch-on correctly.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Physics course of the University of Cambridge](../../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
