<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $x=g\mu_BB/(k_BT)$. The single-ion [partition function](../../../../canonical-partition-function.md) and mean projected [magnetic moment](../../../../magnetic-dipole-moment.md) are

$$
Z_J(x)=\sum_{m_J=-J}^{J}e^{xm_J},\qquad
\langle\mu_z\rangle=g\mu_B\frac{\sum m_J e^{xm_J}}{\sum e^{xm_J}}
=g\mu_B\frac{\partial\ln Z_J}{\partial x}.
$$

For $J>0$, the geometric sum also gives

$$
\langle\mu_z\rangle=g\mu_B\left[
\left(J+\tfrac12\right)\coth\!\left(\left(J+\tfrac12\right)x\right)
-\tfrac12\coth(x/2)\right].
$$

In the high-temperature, weak-polarization regime $|x|J\ll1$, expand the [Boltzmann factors](../../../../boltzmann-factor.md). The numerator's zero-order term vanishes because $\sum m_J=0$, and the first-order term uses $\sum m_J^2=J(J+1)(2J+1)/3$. The denominator is $2J+1+O(x^2)$. Therefore

$$
\boxed{\langle\mu_z\rangle\simeq\frac{(g\mu_B)^2J(J+1)B}{3k_BT}
=\frac CT,\qquad
C=\frac{(g\mu_B)^2J(J+1)B}{3k_B}.}
$$

This [fixed-field per-ion Curie coefficient](../../../../fixed-field-per-ion-curie-coefficient.md) describes **mean moment per ion at fixed field**, so it includes $B$. It is not the field-independent volume-susceptibility [Curie constant](../../../../curie-constant.md). For [number density](../../../../number-density.md) $n$ and $B\simeq\mu_0H$, the latter is $C_\chi=n\mu_0(g\mu_B)^2J(J+1)/(3k_B)$, giving $\chi_H=C_\chi/T$. At $J=0$, the specified moment is zero and both expressions vanish.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
