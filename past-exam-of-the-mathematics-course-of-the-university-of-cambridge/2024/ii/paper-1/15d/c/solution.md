<h1 id="15d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Radiation conservation gives

$$
\rho_R=\rho_{R0}a^{-4}.
$$

Consequently

$$
H^2=H_0^2\Omega_{R0}a^{-4}
+\frac{\Lambda c^2}{3}.
$$

Evaluating at $t_0$, where $a=1$, shows that

$$
\frac{\Lambda c^2}{3}=H_0^2(1-\Omega_{R0}).
$$

Put

$$
A=H_0^2\Omega_{R0},
\qquad
B=H_0^2(1-\Omega_{R0}),
\qquad
b=a^2.
$$

Then $\dot b=2\sqrt{A+Bb^2}$. Choosing the big bang as $t=0$ and integrating gives

$$
b=\sqrt{\frac AB}\sinh(2\sqrt B\,t).
$$

Therefore

$$
\boxed{
a(t)=\alpha[\sinh(\beta t)]^{1/2}},
$$

where

$$
\boxed{
\alpha=\left(\frac{\Omega_{R0}}{1-\Omega_{R0}}\right)^{1/4},
\qquad
\beta=2H_0\sqrt{1-\Omega_{R0}}}.
$$

At early times, $\sinh(\beta t)\sim\beta t$, so $a\propto t^{1/2}$, as in a radiation-dominated universe. At late times,

$$
a\sim\frac{\alpha}{\sqrt2}e^{\beta t/2},
$$

the expected de Sitter expansion with $H\to\sqrt{\Lambda c^2/3}$.

[Acceleration](../../../../../../acceleration.md) begins when the radiation deceleration and cosmological-constant [acceleration](../../../../../../acceleration.md) balance:

$$
H_0^2\Omega_{R0}a^{-4}
=H_0^2(1-\Omega_{R0}).
$$

Thus $a=\alpha$, which in the exact solution means $\sinh(\beta t_\Lambda)=1$. Hence

$$
\boxed{
t_\Lambda=\frac{\operatorname{arsinh}1}
{2H_0\sqrt{1-\Omega_{R0}}}}.
$$

This is the [radiation-to-cosmological-constant transition](../../../../../../radiation-to-cosmological-constant-transition.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15D](../../15d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
