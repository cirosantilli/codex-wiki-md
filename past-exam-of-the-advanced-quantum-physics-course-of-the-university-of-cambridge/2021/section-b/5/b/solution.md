<h1 id="section-b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the requested oscillator response, treat $y$ as the fixed transverse position of a one-dimensional [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator-split.md) along $z$, and put $\theta=ky$. The supplied radiation is transverse and already satisfies the [Coulomb gauge](../../../../../coulomb-gauge.md). Its perturbation is

$$
H_1(t)=\frac{eA_0}{m}p_z\left(e^{i\theta}e^{-i\omega t}+e^{-i\theta}e^{i\omega t}\right),\quad t>0.
$$

The [annihilation operator](../../../../../annihilation-operator.md) and [creation operator](../../../../../creation-operator.md) give

$$
p_z=i\sqrt{\frac{m\hbar\omega_0}{2}}(a^\dagger-a),\qquad
\langle n|p_z|0\rangle=i\sqrt{\frac{m\hbar\omega_0}{2}}\,\delta_{n1}.
$$

Thus the only first-order transition out of the [ground state](../../../../../ground-state.md) is to $|1\rangle$. More generally, the oscillator [electric-dipole selection rule](../../../../../electric-dipole-selection-rule.md) is $\Delta n=\pm1$. This is a rule for [matrix elements](../../../../../matrix-element.md); exact energy conservation is replaced by a finite-time resonance profile during a switched finite-duration interaction.

To display both the resonant and nonresonant terms without spurious singularities, define

$$
F_\nu(t)=\int_0^t e^{i\nu t'}dt'
=\begin{cases}(e^{i\nu t}-1)/(i\nu),&\nu\ne0,\\t,&\nu=0,\end{cases}
\qquad C= eA_0\sqrt{\frac{\omega_0}{2m\hbar}}.
$$

The [interaction picture](../../../../../interaction-picture.md) coefficient in the given expansion is then

$$
\boxed{b_1(t)=C\left[e^{i\theta}F_{\omega_0-\omega}(t)
+e^{-i\theta}F_{\omega_0+\omega}(t)\right],\qquad b_n(t)=0\ (n\geq2).}
$$

The full [Schrödinger picture](../../../../../schrodinger-picture.md) coefficient of $|1\rangle$ is $e^{-3i\omega_0t/2}b_1(t)$, while that of $|0\rangle$ is $e^{-i\omega_0t/2}$ at this order. The normalization changes only at order $A_0^2$. In particular, at $\omega=\omega_0$ the first term is $Ce^{i\theta}t$, finite for every finite time, and the perturbative result requires $|b_1|\ll1$.

The fixed-$y$ interpretation is needed for the displayed target formulae. If $p^2$ were instead a three-dimensional kinetic operator with no transverse confinement, that model would have no normalizable transverse [ground state](../../../../../ground-state.md), and $e^{\pm iky}$ would transfer transverse [momentum](../../../../../momentum-split.md) $\pm\hbar k$. A treatment of that different model needs specified transverse states and recoil energies; they are absent from the question. The following parts use the intended localized-oscillator response.

## ↑ Ancestors (14)

1. [B](../b.md)
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
