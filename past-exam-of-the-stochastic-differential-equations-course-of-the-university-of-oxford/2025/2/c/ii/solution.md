<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $c=\beta/2-\alpha$. The change of measure and part (a)(iii) yield

$$
L(t,\alpha,\beta)=e^{-\beta t/2}\mathbb E_{\mathbb Q_t}e^{cB_t^2}.
$$

For a centered [normal random variable](../../../../../gaussian-random-variable.md) $G$ of [variance](../../../../../variance-split.md) $v>0$, a [Gaussian integral](../../../../../gaussian-integral.md) gives the [Gaussian quadratic exponential moment](../../../../../gaussian-quadratic-exponential-moment.md)

$$
\mathbb Ee^{cG^2}=(1-2cv)^{-1/2},\qquad 1-2cv>0.
$$

Here $c\leq\beta/2$ and $\beta v_t<1/2$ for finite positive $t$, so the required positivity holds, including when $c>0$. Thus

$$
L(t,\alpha,\beta)
=\left[e^{\beta t}\left(1-(\beta-2\alpha)
\frac{1-e^{-2\beta t}}{2\beta}\right)\right]^{-1/2}.
$$

Expanding the two exponentials in terms of [hyperbolic functions](../../../../../hyperbolic-function.md) gives

$$
\boxed{L(t,\alpha,\beta)
=\left(\cosh(\beta t)+\frac{2\alpha}{\beta}\sinh(\beta t)\right)^{-1/2}\quad(\beta>0).}
$$

At $t=0$ this is one. As $\beta\downarrow0$, the denominator tends to $1+2\alpha t$, recovering part (a)(i). At $\alpha=0$ it gives the [Laplace transform of the integrated square of Brownian motion](../../../../../laplace-transform-of-the-integrated-square-of-brownian-motion.md). The joint terminal-and-integral transform is the [Joint Laplace transform of Brownian square and its time integral](../../../../../joint-laplace-transform-of-brownian-square-and-its-time-integral.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
