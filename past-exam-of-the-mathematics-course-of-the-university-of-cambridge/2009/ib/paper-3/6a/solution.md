<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

With $\Re\alpha<0$, the causal exponential is integrable and its [Fourier transform](../../../../../fourier-transform.md) is

$$
\widetilde h(\omega)=\int_0^\infty e^{(\alpha-i\omega)t}\,dt
=\left[\frac{e^{(\alpha-i\omega)t}}{\alpha-i\omega}\right]_0^\infty
=\boxed{\frac1{i\omega-\alpha}}.
$$

For the pendulum system, a [transfer function](../../../../../transfer-function.md) is the [Fourier transform](../../../../../fourier-transform.md) of its causal [impulse response](../../../../../impulse-response.md), equivalently the multiplier relating the transformed forcing to the transformed zero-initial-data response. Transforming [derivatives](../../../../../derivative.md) gives

$$
\widetilde R(\omega)=\frac1{(i\omega)^2+2i\omega+5}
=\frac1{(i\omega+1-2i)(i\omega+1+2i)}.
$$

Partial fractions therefore give

$$
\boxed{\widetilde R(\omega)=\frac1{4i}\left[\frac1{i\omega+1-2i}-\frac1{i\omega+1+2i}\right].}
$$

The exponential transform identifies the causal response as $R(t)=\tfrac12e^{-t}\sin2t$ for $t>0$ and zero for $t<0$. It solves the homogeneous equation for $t>0$, with $R(0^+)=0$ and $R'(0^+)=1$, the jump required by a unit impulse. The forcing is understood as switched on at zero; its transform is $1/(i\omega+4)$, and [convolution](../../../../../convolution.md) with $R$ gives, if the time response is wanted,

$$
\theta(t)=\frac1{13}e^{-4t}-\frac1{13}e^{-t}\cos2t+\frac3{26}e^{-t}\sin2t\quad(t\geq0).
$$

This has both stated initial values equal to zero.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
