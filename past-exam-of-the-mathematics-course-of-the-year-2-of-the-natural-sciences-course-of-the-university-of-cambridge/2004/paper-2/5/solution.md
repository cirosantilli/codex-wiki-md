<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For causal functions the [convolution](../../../../convolution.md) is $(f*g)(t)=\int_0^t f(\tau)g(t-\tau)d\tau$. In a half-plane of absolute convergence, changing variables $u=t-\tau$ in its [Laplace transform](../../../../laplace-transform.md) and using [Fubini's theorem](../../../../fubini-s-theorem.md) gives

$$
\mathcal L(f*g)(s)=\int_0^\infty\int_0^\infty e^{-s(u+\tau)}f(\tau)g(u)du\,d\tau=F(s)G(s).
$$

This proves the [convolution theorem for Laplace transforms](../../../../convolution-theorem-for-laplace-transforms.md). Transforming the differential equation gives $(s^2+1)Y(s)=sy(0)+y'(0)+F(s)$. The direct transform pairs $\mathcal L(\cos t)=s/(s^2+1)$ and $\mathcal L(\sin t)=1/(s^2+1)$ then give

$$
\boxed{y(t)=y(0)\cos t+y'(0)\sin t+\int_0^t f(\tau)\sin(t-\tau)d\tau.}
$$

For a continuous forcing, call the last term $w(t)$. The [Leibniz integral rule](../../../../leibniz-integral-rule.md) gives $w'=\int_0^t f(\tau)\cos(t-\tau)d\tau$ and $w''=f(t)-w(t)$. Also $w(0)=w'(0)=0$. Thus both the original equation and the initial values hold.

For an impulse at positive time $T$, the [Dirac delta](../../../../dirac-delta-function.md) evaluates the convolution, yielding

$$
\boxed{y(t)=y(0)\cos t+y'(0)\sin t+H(t-T)\sin(t-T).}
$$

Here $H$ is the [Heaviside step function](../../../../heaviside-step-function.md). The displacement remains continuous at $T$, while its derivative jumps upward by one, exactly as required by integrating the differential equation across the unit impulse.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [2004](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
