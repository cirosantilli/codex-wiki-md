<h1 id="31b/solution">Solution</h1>

↑ **Parent:** [31B](../31b.md)

Rotate the contour for the [Gaussian integral](../../../../../gaussian-integral.md) through angle $-\pi/4$; a small positive damping factor justifies the deformation and can then be removed. After scaling by $t^{-1/2}$, the [oscillatory Gaussian integral with negative phase](../../../../../oscillatory-gaussian-integral-with-negative-phase.md) gives

$$
\boxed{
\lim_{R\to\infty}\int_{-R}^R e^{-itu^2}du
=e^{-i\pi/4}\sqrt{\frac\pi t}.}
$$

Similarly, first scale $u=t^{-1/3}v$ and then rotate the positive ray through angle $-\pi/6$. Since $\int_0^\infty e^{-v^3}dv=\Gamma(4/3)$, the [cubic oscillatory Gamma integral](../../../../../cubic-oscillatory-gamma-integral.md) gives

$$
\boxed{
\lim_{R\to\infty}\int_0^R e^{-itu^3}du
=e^{-i\pi/6}t^{-1/3}\Gamma\left(\frac43\right).}
$$

For fixed $\alpha$, consider the complex phase

$$
\Phi(\theta)=x\sin\theta-\alpha\theta.
$$

Its unique interior stationary point is

$$
\theta_0=\arccos(\alpha/x)
=\frac\pi2-\frac\alpha x+O(x^{-3}),
$$

where

$$
\Phi(\theta_0)=x-\frac{\pi\alpha}{2}+O(x^{-1}),
\qquad
\Phi''(\theta_0)=-x+O(x^{-1}).
$$

The endpoint contributions are $O(x^{-1})$, while the [one-dimensional stationary-phase formula](../../../../../one-dimensional-stationary-phase-formula.md) has order $x^{-1/2}$. Taking its real part proves the [stationary-phase asymptotic for the generalized Bessel cosine integral](../../../../../stationary-phase-asymptotic-for-the-generalized-bessel-cosine-integral.md):

$$
\boxed{
Q_\alpha(x)\sim
\sqrt{\frac2{\pi x}}
\cos\left(x-\frac{\pi\alpha}{2}-\frac\pi4\right).}
$$

For $Q_x(x)$ the phase is $x(\sin\theta-\theta)$. Its stationary point has merged with the endpoint $\theta=0$, where

$$
\sin\theta-\theta=-\frac{\theta^3}{6}+O(\theta^5).
$$

Use the [cubic endpoint stationary-phase scaling](../../../../../cubic-endpoint-stationary-phase-scaling.md) $\theta=(6/x)^{1/3}u$. The other endpoint and the region away from zero contribute only $O(x^{-1})$, so

$$
\begin{aligned}
Q_x(x)
&\sim\frac1\pi\left(\frac6x\right)^{1/3}
\int_0^\infty\cos(u^3)du\\
&=\frac{6^{1/3}}{\pi x^{1/3}}
\Gamma\left(\frac43\right)\cos\frac\pi6.
\end{aligned}
$$

Therefore

$$
\boxed{
Q_x(x)\sim
\frac{\sqrt3 6^{1/3}}{2\pi}
\Gamma\left(\frac43\right)x^{-1/3}.}
$$

## ↑ Ancestors (10)

1. [31B](../31b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
