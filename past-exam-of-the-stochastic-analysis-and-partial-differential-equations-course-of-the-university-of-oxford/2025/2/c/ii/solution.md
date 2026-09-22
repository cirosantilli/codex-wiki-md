<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $a<0$, set $v_\infty=-\sigma^2/(2a)>0$. The candidate [invariant probability law of a Markov process](../../../../../invariant-probability-law-of-a-markov-process.md) is

$$
\boxed{\pi=\mathcal N\left(0,-\frac{\sigma^2}{2a}\right),\qquad
\pi(dx)=\sqrt{\frac{-a}{\pi\sigma^2}}\exp\left(\frac{ax^2}{\sigma^2}\right)\,dx.}
$$

To prove invariance rather than merely guess a limiting [probability distribution](../../../../../probability-distribution-split.md), initialize $X_t\sim\pi$ independently of future [Brownian increments](../../../../../brownian-increment.md). Integrating the [conditional characteristic function](../../../../../conditional-characteristic-function.md) from part (i) against this centered [normal distribution](../../../../../normal-distribution.md) gives

$$
\begin{aligned}
\mathbb E[e^{iuX_{t+\Delta}}]
&=e^{-u^2v_\Delta/2}\,\mathbb E[e^{iu e^{a\Delta}X_t}]\\
&=\exp\left[-\frac12u^2\left(v_\Delta+e^{2a\Delta}v_\infty\right)\right]
=e^{-u^2v_\infty/2},
\end{aligned}
$$

because $v_\Delta=v_\infty(1-e^{2a\Delta})$. The [uniqueness theorem for characteristic functions](../../../../../uniqueness-theorem-for-characteristic-functions.md) implies $X_{t+\Delta}\sim\pi$ for every $\Delta\geq0$. This proves $\pi P_\Delta=\pi$, as required. The [time-homogeneous Markov property](../../../../../time-homogeneous-markov-property.md) then also makes the process with this [Ornstein-Uhlenbeck stationary initialization](../../../../../ornstein-uhlenbeck-stationary-initialization.md) a [strictly stationary process](../../../../../strictly-stationary-process.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic analysis and partial differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic analysis and partial differential equations course of the University of Oxford](../../../../../stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
