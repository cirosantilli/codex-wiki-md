<h1 id="40c/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For real harmonic quantities

$$
f(t)=\operatorname{Re}(\widehat f e^{i\omega t}),
\qquad
g(t)=\operatorname{Re}(\widehat g e^{i\omega t}),
$$

define the period average by

$$
\langle fg\rangle
=\frac\omega{2\pi}\int_0^{2\pi/\omega}f(t)g(t)\,dt
=\frac12\operatorname{Re}(\widehat f\widehat g^*).
$$

This is the [time average of harmonic power](../../../../../../../time-average-of-harmonic-power.md).

At $r=a$, put $x=\omega a/c_0$. The velocity and pressure amplitudes are

$$
\widehat u_r(a)=i\omega\epsilon,
\qquad
\widehat p(a)=-i\rho_0\omega\widehat\phi(a)
=-\frac{\rho_0\omega^2\epsilon a}{1+ix}.
$$

Hence the mean outward work rate per unit area is

$$
\langle p'u_r\rangle
=\frac12\operatorname{Re}
\left(\widehat p\widehat u_r^*\right)
=\frac{\rho_0\omega^4\epsilon^2a^2}
{2c_0(1+x^2)}.
$$

Multiplication by the area $4\pi a^2$ yields

$$
\begin{aligned}
\langle\mathcal P\rangle
&=\frac{2\pi\rho_0\omega^4\epsilon^2a^4/c_0}
{1+\omega^2a^2/c_0^2}\\
&=\boxed{
2\pi a^2\rho_0\omega^2\epsilon^2c_0
\frac{\omega^2a^2}{c_0^2+\omega^2a^2}
}.
\end{aligned}
$$

This is the [mean acoustic power of a pulsating sphere](../../../../../../../mean-acoustic-power-of-a-pulsating-sphere.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [40C](../../../40c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
