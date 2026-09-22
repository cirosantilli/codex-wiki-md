<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here $q=\kappa/R$, so the equation from part (b) becomes the [Euler-Cauchy equation](../../../../../../euler-cauchy-equation.md)

$$
B_z''+\frac2R B_z'+\frac{\kappa^2}{R^2}B_z=0.
$$

The [power-law ansatz](../../../../../../power-law-ansatz.md) $B_z=R^s$ gives the [indicial equation](../../../../../../indicial-equation.md)

$$
s^2+s+\kappa^2=0,
\qquad
s_\pm=\frac{-1\pm\sqrt{1-4\kappa^2}}2.
$$

For $0<\kappa<1/2$, the general field is therefore

$$
\boxed{B_R=0,\qquad
B_z=C_+R^{s_+}+C_-R^{s_-},\qquad
B_\phi=-\frac1\kappa
\left(s_+C_+R^{s_+}+s_-C_-R^{s_-}\right)}.
$$

The [polynomial discriminant](../../../../../../polynomial-discriminant.md) changes sign at

$$
\boxed{\kappa_c=\frac12}.
$$

For $\kappa>\kappa_c$, define $\mu=\sqrt{\kappa^2-1/4}$. A real form of the solution is

$$
B_z=R^{-1/2}\left[C\cos\!\left(\mu\ln\frac R{R_0}\right)
+D\sin\!\left(\mu\ln\frac R{R_0}\right)\right],
\qquad
B_\phi=-\frac R\kappa\frac{dB_z}{dR},
\qquad B_R=0.
$$

**Thus the field has a [log-periodic oscillation](../../../../../../log-periodic-oscillation.md): its phase is periodic in $\ln R$, so it oscillates as the radius changes geometrically.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
