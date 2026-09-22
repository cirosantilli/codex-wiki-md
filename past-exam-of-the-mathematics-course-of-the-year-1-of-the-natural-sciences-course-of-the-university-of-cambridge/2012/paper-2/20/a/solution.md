<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the kernel as $K(s,t)=(4\pi t)^{-1/2}e^{-s^2/(4t)}$, with $t>0$. Its [partial derivatives](../../../../../partial-derivative.md) are

$$
K_t=\left(-\frac1{2t}+\frac{s^2}{4t^2}\right)K,
\qquad K_{ss}=\left(-\frac1{2t}+\frac{s^2}{4t^2}\right)K.
$$

Thus the [heat kernel](../../../../../heat-kernel.md) itself satisfies $K_t=K_{ss}$. The proposed [convolution](../../../../../convolution.md) consequently gives

$$
u_t(x,t)=\int_{\mathbb R}\varphi(\xi)K_t(x-\xi,t)\,d\xi
=\int_{\mathbb R}\varphi(\xi)K_{ss}(x-\xi,t)\,d\xi
=u_{xx}(x,t).
$$

This verifies the [heat equation](../../../../../heat-equation.md). The parameter is positive time; the real integral formula is not defined at negative time.

The passage of [derivatives](../../../../../derivative.md) through the [integral](../../../../../integral-split.md) needs justification. A sufficient condition is the Gaussian-weighted absolute integrability in [heat-kernel convergence for Gaussian-integrable initial data](../../../../../heat-kernel-convergence-for-gaussian-integrable-initial-data.md); it holds, in particular, for data of [polynomial growth](../../../../../polynomial-growth.md). On compact positive-time intervals strictly below an integrable later time, the differentiated kernels have an integrable Gaussian bound, so [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) applies.

Even if the PDF's assumed convergence is read as ordinary conditional convergence, one can justify the same calculation. Choose a later time $T>t$ and let $H(\xi)$ be a primitive of $\varphi(\xi)e^{-\xi^2/(4T)}$. Convergence at spatial point zero and time $T$ makes $H$ bounded on both tails. Put $q(x,\xi,t)=K(x-\xi,t)e^{\xi^2/(4T)}$. This [function](../../../../../function-split.md), its spatial and time [derivatives](../../../../../derivative.md), and their $\xi$-derivatives decay as Gaussians when $t<T$. [Integration by parts](../../../../../integration-by-parts.md) rewrites the [convolution](../../../../../convolution.md) as $-\int Hq_\xi\,d\xi$, with vanishing endpoint terms. Boundedness of $H$ now permits differentiation under this absolutely convergent [integral](../../../../../integral-split.md); since $q_t=q_{xx}$, the same equation follows. Thus one need not silently equate conditional and absolute convergence.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
