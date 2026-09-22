<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First suppose $0<r<\rho=|z_0|$. For every $R>\rho$, the [planar Brownian annulus hitting probability](../../../../../planar-brownian-annulus-hitting-probability.md) gives

$$
\mathbb P(\tau_r<\infty)
\geq\mathbb P(\tau_r<\tau_R)
=\frac{\log(R/\rho)}{\log(R/r)}\longrightarrow1
\quad(R\to\infty).
$$

Hence $\tau_r<\infty$ [almost surely](../../../../../almost-sure-convergence.md). This uses increasing outer radii; letting the inner radius tend to zero instead proves the different claim in part (ii).

For $r>\rho$, the disk-exit estimate in (i), with outer radius $r$, directly yields $\mathbb E\tau_r\leq(r^2-\rho^2)/2<\infty$.

For $r=\rho$, retain the definition $\tau_r=\inf\{t>0:|B_t|=r\}$. The first case shows that radius $\rho/2$ is reached in finite time. Starting there, the [Strong Markov property](../../../../../strong-markov-property.md) of [Brownian motion](../../../../../brownian-motion-split.md) and the disk-exit argument show that radius $\rho$ is subsequently reached in finite time. Thus the infimum over positive hitting times is finite in this case as well. Altogether,

$$
\boxed{\mathbb P(\tau_r<\infty)=1\qquad\text{for every }r>0.}
$$

The conclusion can also be made simultaneous in all $r>0$: intersect the probability-one events for positive rational radii, then use continuity to cross each intermediate radius.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
