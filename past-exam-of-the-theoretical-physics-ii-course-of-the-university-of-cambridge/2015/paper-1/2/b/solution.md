<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $\tau=t_f-t_i>0$ and split it into $M$ intervals of width $\Delta t=\tau/M$. The [markov property](../../../../../markov-property.md) and Gaussian [convolution](../../../../../convolution.md) give

$$
K=\int_{\mathbb R^{M-1}}\prod_{j=1}^{M-1}dx_j
\prod_{j=0}^{M-1}\frac{\exp[-(x_{j+1}-x_j)^2/(4D\Delta t)]}
{\sqrt{4\pi D\Delta t}},
\qquad x_0=x_i,\ x_M=x_f.
$$

This finite-dimensional identity is exact for every positive $M$. Define the path-integral measure by these normalized [time](../../../../../time-in-physics.md) slices:

$$
\int\mathcal D x\,(\cdots)
=\lim_{M\to\infty}(4\pi D\Delta t)^{-M/2}
\int\prod_{j=1}^{M-1}dx_j\,(\cdots).
$$

In the [time-sliced diffusion path integral](../../../../../time-sliced-diffusion-path-integral.md), the discrete exponent is $\sum_j[(x_{j+1}-x_j)/\Delta t]^2\Delta t/(4D)$. Its conventional continuum notation is therefore

$$
\boxed{K(x_f,t_f|x_i,t_i)
=\int_{x_i}^{x_f}\mathcal D x\,
\exp\!\left[-\int_{t_i}^{t_f}\frac{\dot x^2}{4D}\,dt\right].}
$$

The time-slice normalization is essential, not an arbitrary multiplicative constant. Brownian paths are almost surely nondifferentiable, so the displayed [action](../../../../../action.md) is shorthand for the Gaussian limiting measure rather than an ordinary integral of the derivative of each typical path.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
