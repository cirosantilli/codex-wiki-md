<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For independent $\chi,\chi^*$, the derivatives needed in the $\chi^*$ [Euler-Lagrange field equation](../../../../euler-lagrange-field-equation.md) are

$$
\frac{\partial\mathcal L_2}{\partial\chi^*}=\frac{i\hbar}{2}\dot\chi-\mu(\chi+\chi^*),\qquad
\frac{\partial\mathcal L_2}{\partial\dot\chi^*}=-\frac{i\hbar}{2}\chi,\qquad
\frac{\partial\mathcal L_2}{\partial(\nabla\chi^*)}=-\frac{\hbar^2}{2M}\nabla\chi.
$$

Consequently the two conjugate field equations are

$$
\boxed{i\hbar\dot\chi=-\frac{\hbar^2}{2M}\nabla^2\chi+\mu(\chi+\chi^*),\qquad
-i\hbar\dot\chi^*=-\frac{\hbar^2}{2M}\nabla^2\chi^*+\mu(\chi+\chi^*).}
$$

Write $\chi=\chi_1+i\chi_2$ with real components, and put $A=\hbar^2/(2M)$. Separating real and imaginary parts gives

$$
-\hbar\dot\chi_2=(-A\nabla^2+2\mu)\chi_1,\qquad
\hbar\dot\chi_1=-A\nabla^2\chi_2.
$$

For each real field take the real part of a complex [plane wave](../../../../plane-wave.md) amplitude, $\chi_j=\operatorname{Re}[q_j e^{i(\mathbf k\cdot\mathbf r-\omega t)}]$. With $\epsilon_k=\hbar^2|\mathbf k|^2/(2M)$ the two equations become

$$
i\hbar\omega q_2=(\epsilon_k+2\mu)q_1,\qquad
-i\hbar\omega q_1=\epsilon_k q_2.
$$

A nonzero [normal mode](../../../../normal-mode.md) requires their [determinant](../../../../determinant.md) to vanish, so

$$
\hbar^2\omega^2=\epsilon_k(\epsilon_k+2\mu).
$$

The positive-frequency [Bogoliubov quasiparticle dispersion](../../../../bogoliubov-quasiparticle-dispersion.md) is therefore

$$
\boxed{\omega(\mathbf k)=\frac1\hbar\sqrt{\epsilon_k(\epsilon_k+2\mu)}
=\sqrt{\frac{|\mathbf k|^2}{2M}\left(\frac{\hbar^2|\mathbf k|^2}{2M}+2\mu\right)}.}
$$

There is also the negative-frequency conjugate solution, as required for real component fields. Since $\mu>0$, $\omega^2\geq0$, consistent with the stability of the chosen uniform [ground state](../../../../ground-state.md).

## ↑ Ancestors (14)

1. [D](../d.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
