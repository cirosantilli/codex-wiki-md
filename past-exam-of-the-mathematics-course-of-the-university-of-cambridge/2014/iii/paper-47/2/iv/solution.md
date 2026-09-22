<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

At $\theta=0$, the field equations are

$$
\Box\phi-\sin\phi\cos\phi[(\partial\alpha)^2-m^2]=0,
\qquad\partial_\mu(\sin^2\phi\,\partial^\mu\alpha)=0.
$$

With $\alpha=\omega t+\alpha_0$ and static $\phi$, the second equation holds automatically and the first reduces to

$$
\phi_{xx}=(m^2-\omega^2)\sin\phi\cos\phi.
$$

For $|\omega|<m$, put $\kappa=\sqrt{m^2-\omega^2}$. The finite-energy $T=1$ solution is

$$
\boxed{\phi(x)=2\arctan e^{\kappa(x-x_0)},\qquad
\alpha(x,t)=\omega t+\alpha_0.}
$$

This is a [rotating charged kink in a spherical sigma model](../../../../../../rotating-charged-kink-in-a-spherical-sigma-model.md). Its orientation moves around a circle while its [energy](../../../../../../energy.md) profile stays at rest. The limiting value $|\omega|=m$ gives no localized finite-width [kink](../../../../../../scalar-field-kink.md); larger $|\omega|$ does not give this finite-energy interpolation.

Using $\phi_x=\kappa\sin\phi$ and $\int\sin^2\phi\,dx=2/\kappa$, its rest [energy](../../../../../../energy.md) and mechanical charge are

$$
\begin{aligned}
M&=\frac r4\int\left[\phi_x^2+(m^2+\omega^2)\sin^2\phi\right]dx
=\boxed{\frac{rm^2}{\kappa}},\\
Q_0&=\frac{r\omega}{2}\int\sin^2\phi\,dx
=\boxed{\frac{r\omega}{\kappa}}.
\end{aligned}
$$

Eliminating $\omega$ gives

$$
\boxed{M=m\sqrt{r^2+Q_0^2},\qquad
\omega=\frac{mQ_0}{\sqrt{r^2+Q_0^2}}.}
$$

For this part $Q=Q_0$ since $\theta=0$. The static [mass](../../../../../../mass.md) is recovered at $Q_0=0$, and the [mass](../../../../../../mass.md) grows with the magnitude of the global charge. If theta is restored, the [energy](../../../../../../energy.md) remains the same function of $Q_0$, but $Q_0=Q_\theta+\theta T/(2\pi)$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
