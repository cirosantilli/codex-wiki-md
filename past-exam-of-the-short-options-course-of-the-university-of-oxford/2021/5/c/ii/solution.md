<h1 id="5/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Substitute $\widehat u=e^{-b(t)s^2}$ into the transformed [partial differential equation](../../../../../partial-differential-equation-split.md). Comparing coefficients gives $b'=1-2b$, $b(0)=0$, whence

$$
\boxed{b(t)=\frac{1-e^{-2t}}2,\qquad\widehat u(s,t)=\exp\!\left[-\frac{1-e^{-2t}}2s^2\right].}
$$

The stated Gaussian [Fourier transform](../../../../../fourier-transform-split.md) pair, with its inverse factor $1/(2\pi)$, gives

$$
\boxed{u(x,t)=\frac{1}{\sqrt{2\pi(1-e^{-2t})}}\exp\!\left[-\frac{x^2}{2(1-e^{-2t})}\right],\qquad t>0.}
$$

This is a [normal distribution](../../../../../normal-distribution.md) density with mean zero and [variance](../../../../../variance-split.md) $1-e^{-2t}$. Its total integral is one. As $t\downarrow0$ it converges to $\delta$ in the sense of [distributions](../../../../../distribution-mathematical-analysis.md), while as $t\to\infty$ it tends to the standard [normal distribution](../../../../../normal-distribution.md) density. This is the transition density from zero of the [Ornstein-Uhlenbeck process](../../../../../ornstein-uhlenbeck-process.md) with drift $-x$ and diffusion coefficient $\sqrt2$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
