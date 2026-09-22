<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $a=\delta\lambda$, $t_0=\lambda^2$, and $h=(\beta^2-1)\lambda^2$. On the event $\{\tau^{1/2}>\beta\lambda,\ X_\tau^*\leq a\}$, one has $\tau>t_0$ and the Brownian path remains in $[-a,a]$ throughout the next $h$ time units after $t_0$.

For Brownian motion started at $x\in(-a,a)$, let $H$ be its first exit time from $(-a,a)$. The martingale $B_t^2-t$, stopped at $H\wedge n$, gives $\mathbb E_x(H\wedge n)\leq a^2-x^2$. [Monotone convergence](../../../../../monotone-convergence-theorem.md) first proves finite mean exit time, and [dominated convergence](../../../../../dominated-convergence-theorem.md) for the bounded stopped position then gives

$$
\mathbb E_xH=a^2-x^2\leq a^2.
$$

Thus [Markov's inequality](../../../../../markov-s-inequality.md) yields $\mathbb P_x(H>h)\leq a^2/h$. Remaining in the closed interval for a fixed positive duration has the same probability as avoiding boundary exit: Brownian motion crosses immediately after first hitting an endpoint.

Condition on $\mathcal F_{t_0}$. The event $\{\tau>t_0\}$ is measurable there because $\tau$ is a [stopping time](../../../../../stopping-time.md), and future Brownian increments are independent of this sigma-algebra. The preceding bound is uniform in the current point inside the interval. Therefore

$$
\begin{aligned}
\mathbb P(\tau^{1/2}>\beta\lambda,\ X_\tau^*\leq\delta\lambda)
&\leq\frac{a^2}{h}\mathbb P(\tau>t_0)\\
&=\boxed{\frac{\delta^2}{\beta^2-1}
\mathbb P(\tau^{1/2}>\lambda).}
\end{aligned}
$$

This is a [good-lambda bound for Brownian stopping time and maximum](../../../../../good-lambda-bound-for-brownian-stopping-time-and-maximum.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
