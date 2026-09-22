<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the critically damped case, causality reduces the [convolution](../../../../../convolution.md) to

$$
y(t)=\int_0^\infty s e^{-\kappa s}\cos[\kappa(t-s)]\,ds.
$$

Although the forcing is not integrable on the full real line, this integral converges absolutely because the [Green's function](../../../../../green-s-function-split.md) is integrable. Thus the calculation is valid directly; the corresponding [Fourier transform](../../../../../fourier-transform-split.md) can be interpreted as a [tempered distribution](../../../../../tempered-distribution.md).

Use the [complex exponential](../../../../../complex-exponential-function.md) and $\int_0^\infty s e^{-as}\,ds=a^{-2}$ for $\operatorname{Re}a>0$:

$$
y(t)=\operatorname{Re}\left[e^{i\kappa t}\int_0^\infty s e^{-\kappa(1+i)s}\,ds\right]
=\operatorname{Re}\left[\frac{e^{i\kappa t}}{\kappa^2(1+i)^2}\right].
$$

Since $(1+i)^2=2i$, the [convolution](../../../../../convolution.md) response is

$$
\boxed{y(t)=\frac{\sin(\kappa t)}{2\kappa^2}}.
$$

This is the bounded steady response to the stated forcing acting for all time. Without an [initial condition](../../../../../initial-condition.md) or the [convolution](../../../../../convolution.md) selection, the general solution additionally contains $(C_1+C_2t)e^{-\kappa t}$. No switch-on at $t=0$ was specified, so zero initial displacement and [velocity](../../../../../velocity.md) should not be imposed on this all-time forcing.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
