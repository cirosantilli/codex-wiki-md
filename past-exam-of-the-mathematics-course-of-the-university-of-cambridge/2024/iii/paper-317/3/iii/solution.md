<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Multiplying $y''=-\omega^2y^2$ by $y'$ and integrating gives

$$
\frac12(y')^2+\frac{\omega^2}{3}y^3
=\frac{\omega^2}{3}T_0^{21},
$$

where the base conditions fixed the constant. At the surface, $y=0$ and $y'=AF_s$, with $F_s=L/(4\pi R^2)$. Therefore

$$
A^2F_s^2=\frac{2\omega^2}{3}T_0^{21},
$$

and

$$
\boxed{T_0\propto
\left(\frac{L}{4\pi R^2}\right)^{2/21}}.
$$

Separating variables in the first integral gives

$$
x_0=\sqrt{\frac{3}{2\omega^2}}
\int_0^{T_0^7}\frac{dy}{\sqrt{T_0^{21}-y^3}}.
$$

Set $y=T_0^7\eta$. Then

$$
x_0=\sqrt{\frac{3}{2\omega^2}}T_0^{-7/2}
\int_0^1\frac{d\eta}{\sqrt{1-\eta^3}}
\propto T_0^{-7/2}.
$$

Since $x_0=\Sigma_0^2/2$ and $\Sigma_0=M_{\rm env}/(4\pi R^2)$,

$$
T_0\propto\Sigma_0^{-4/7}.
$$

Combining this with $F_s\propto T_0^{21/2}$ yields

$$
\boxed{
\frac{L}{4\pi R^2}
\propto
\left(\frac{M_{\rm env}}{4\pi R^2}\right)^{-6}}.
$$

This inverse relation signals [thin-shell instability](../../../../../../thin-shell-instability.md). Hydrogen burning has extreme temperature sensitivity, $\epsilon\propto\rho T^{15}$, while the weight of the thin envelope fixes its pressure and limits thermostatic expansion. As burning consumes envelope mass, the equilibrium luminosity rises sharply, accelerating consumption rather than restoring the original state. A thermal runaway can therefore lead to a shell flash or [classical nova](../../../../../../classical-nova.md) rather than steady stable burning.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
