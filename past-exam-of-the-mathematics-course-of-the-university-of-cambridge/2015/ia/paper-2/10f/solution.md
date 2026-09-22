<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

The proposed [probability density function](../../../../../probability-density-function.md) is nonnegative. To check its integral, put $I=\int_{\mathbb R}e^{-x^2/2}\,dx$. The [Gaussian integral](../../../../../gaussian-integral.md) can be evaluated by squaring and using polar coordinates:

$$
I^2=\int_{\mathbb R^2}e^{-(x^2+y^2)/2}\,dx\,dy=2\pi\int_0^\infty re^{-r^2/2}\,dr=2\pi.
$$

Since $I>0$, $I=\sqrt{2\pi}$ and $\int\phi=1$. Thus $X$ has the [standard normal distribution](../../../../../standard-normal-distribution.md). Completing the square in its [moment-generating function](../../../../../moment-generating-function.md) gives, for every real $t$,

$$
M_X(t)=\frac1{\sqrt{2\pi}}\int_{\mathbb R}e^{tx-x^2/2}\,dx=e^{t^2/2}\frac1{\sqrt{2\pi}}\int_{\mathbb R}e^{-(x-t)^2/2}\,dx=\boxed{e^{t^2/2}}.
$$

Differentiation under the integral is justified near every finite $t$ by Gaussian decay. Expanding $e^{t^2/2}=\sum_{m\geq0}t^{2m}/(2^m m!)$ gives **all moments**:

$$
\boxed{\mathbb E[X^{2m+1}]=0,\qquad\mathbb E[X^{2m}]=\frac{(2m)!}{2^m m!}\quad(m\geq0).}
$$

To obtain the [two-term bounds for Mills ratio](../../../../../two-term-bounds-for-mills-ratio.md), use $\phi'(t)=-t\phi(t)$. [Integration by parts](../../../../../integration-by-parts.md) gives, for $x>0$,

$$
\int_x^\infty\phi(t)\,dt=\frac{\phi(x)}x-\int_x^\infty\frac{\phi(t)}{t^2}\,dt.
$$

The positive remainder proves $r(x)<1/x$. A second [integration by parts](../../../../../integration-by-parts.md) gives

$$
\int_x^\infty\frac{\phi(t)}{t^2}\,dt=\frac{\phi(x)}{x^3}-3\int_x^\infty\frac{\phi(t)}{t^4}\,dt.
$$

Substitution and division by the strictly positive $\phi(x)$ show

$$
r(x)=\frac1x-\frac1{x^3}+\frac3{\phi(x)}\int_x^\infty\frac{\phi(t)}{t^4}\,dt.
$$

The last integral is strictly positive for every finite $x>0$, proving **$\boxed{1/x-1/x^3<r(x)<1/x}$**. Both remainders are finite for every fixed positive $x$; the lower bound remains valid even when it is negative.

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
