<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use time dependence $e^{-i\omega t}$ and assume the dopants supply $N$ mobile [electrons](../../../../electron.md) per unit volume. The [Drude model](../../../../drude-model.md) equation is

$$
m_e^*(\ddot{\mathbf x}+\gamma\dot{\mathbf x})=-e\mathbf E_0e^{-i\omega t},\qquad
\mathbf x_0=\frac{e\mathbf E_0}{m_e^*(\omega^2+i\gamma\omega)}.
$$

The free-carrier [electric polarization](../../../../polarization-density.md) is $\mathbf P_c=-Ne\mathbf x$, so, after adding the bound-electron background,

$$
\mathbf D=\epsilon_0\epsilon_\infty\mathbf E+\mathbf P_c
=\epsilon_0\left[\epsilon_\infty-\frac{Ne^2}{\epsilon_0m_e^*(\omega^2+i\gamma\omega)}\right]\mathbf E.
$$

Therefore

$$
\boxed{\epsilon_r(\omega)=\epsilon_\infty\left(1-\frac{\omega_p^2}{\omega^2+i\gamma\omega}\right),\qquad\omega_p^2=\frac{Ne^2}{\epsilon_0\epsilon_\infty m_e^*}.}
$$

The symbol $\omega_p$ here is the background-screened [plasma frequency](../../../../plasma-frequency.md); the unscreened carrier frequency is $\sqrt{\epsilon_\infty}\,\omega_p$. For positive $\gamma$, the [imaginary part](../../../../imaginary-part.md) of $\epsilon_r$ is positive in this time convention, consistent with absorption. Incomplete dopant ionization would replace the nominal doping density by the actual mobile [carrier density](../../../../carrier-density.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the condensed matter physics major option course of the University of Oxford](../../../split.md)
5. [Condensed matter physics major option course of the University of Oxford](../../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
