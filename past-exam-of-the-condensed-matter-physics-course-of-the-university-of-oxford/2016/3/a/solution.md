<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the two allowed [moment projections](../../../../spin-state-population-and-net-polarization.md) as $\pm\mu$, where $\mu=g\mu_B/2$ for [spin one-half](../../../../spin-one-half.md). Their [Zeeman energies](../../../../zeeman-splitting.md) in the prescribed [flux density](../../../../magnetic-field-split.md) are $\mp\mu B$. The single-particle [partition function](../../../../canonical-partition-function.md) and the mean moment along the field are

$$
z=e^{\beta\mu B}+e^{-\beta\mu B}=2\cosh x,\qquad
\langle\mu_z\rangle=\mu\frac{e^x-e^{-x}}{e^x+e^{-x}}=\mu\tanh x,
\quad x=\frac{\mu B}{k_BT}.
$$

For noninteracting moments, [magnetization](../../../../magnetization.md) is moment per volume:

$$
\boxed{M=M_s\tanh(\eta B/T),\qquad M_s=\frac{N\mu}{V},\quad
\eta=\frac\mu{k_B}.}
$$

For electron-like [spin-only](../../../../spin-only-magnetic-moment.md) moments $g\simeq2$, these become $M_s=N\mu_B/V$ and $\eta=\mu_B/k_B$.

[Differentiate](../../../../derivative.md) with respect to the specified $B$ to obtain

$$
\boxed{\chi_B=\left(\frac{\partial M}{\partial B}\right)_T
=\frac{N\mu^2}{Vk_BT}\operatorname{sech}^2x.}
$$

This $B$ [derivative](../../../../derivative.md) is not a dimensionless SI [volume susceptibility](../../../../volume-magnetic-susceptibility.md). In the weak-feedback approximation $B\simeq\mu_0H$, the usual dimensionless [differential susceptibility](../../../../differential-magnetic-susceptibility.md) is $\chi_{\rm diff}\simeq\mu_0\chi_B$. The [small-field limit](../../../../linear-response-theory.md) gives Curie's law $\chi_0=\mu_0N\mu^2/(Vk_BT)$. At finite bias a secant response $M/H\simeq\mu_0M/B=\chi_0\tanh(x)/x$ differs from the differential slope $\chi_0\operatorname{sech}^2x$. For an internal $B=\mu_0(H+M)$ retained self-consistently, the exact local conversion is $\chi_H=\mu_0\chi_B/(1-\mu_0\chi_B)$; [demagnetizing](../../../../demagnetizing-field.md) geometry can further affect an applied-field measurement. Stating the field convention avoids a hidden factor of $\mu_0$ or confusion between a slope and a ratio.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
