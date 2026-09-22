<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [causal Green function](../../../../../causal-green-function.md) vanishes before the impulse. For $t>\tau$ it solves the homogeneous [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md), whose characteristic roots are $-q\pm2i$. Thus it has the form

$$
G(t,\tau)=e^{-q(t-\tau)}[A\cos2(t-\tau)+B\sin2(t-\tau)].
$$

Continuity at $t=\tau$ is necessary to avoid a delta derivative in $G_{tt}$, so $A=0$. Integrating its forced equation across the impulse gives the [jump condition for an impulse](../../../../../jump-condition-for-an-impulse.md), $G_t(\tau^+,\tau)-G_t(\tau^-,\tau)=1$. The derivative from below is zero and the derivative from above is $2B$, giving

$$
\boxed{G(t,\tau)=\frac12\Theta(t-\tau)e^{-q(t-\tau)}\sin[2(t-\tau)].}
$$

Here $\Theta$ is the [Heaviside step function](../../../../../heaviside-step-function.md). The zero initial data exclude any additional homogeneous response. By the [superposition principle](../../../../../superposition-principle.md), the output for a general locally integrable input is

$$
\boxed{x(t)=\int_0^tG(t,\tau)f(\tau)\,d\tau
=\frac12\int_0^te^{-q(t-\tau)}\sin[2(t-\tau)]f(\tau)\,d\tau.}
$$

The upper endpoint causes no unwanted term in the first derivative because $G(t,t)=0$; in the second derivative its unit derivative jump reproduces the input.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
