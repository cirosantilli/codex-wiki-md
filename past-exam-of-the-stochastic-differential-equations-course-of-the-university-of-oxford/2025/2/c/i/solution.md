<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix $t<\infty$. Part (b)(i) makes $d\mathbb Q_t=Z_t\,d\mathbb P$ a [probability measure](../../../../../probability-measure.md) on $\mathcal F_t$, equivalent to $\mathbb P$ since $Z_t>0$. Its density process on $[0,t]$ is $Z_s=\mathbb E[Z_t\mid\mathcal F_s]$. The [Girsanov theorem](../../../../../girsanov-theorem.md), applied to the [stochastic exponential](../../../../../doleans-dade-exponential.md) with integrand $-\beta B_s$, says that

$$
W_s=B_s+\beta\int_0^sB_u\,du,\qquad 0\leq s\leq t,
$$

is standard [Brownian motion](../../../../../brownian-motion-split.md) under $\mathbb Q_t$. The required local square-integrability follows from path continuity, and the true [martingale](../../../../../martingale-split.md) property was proved in part (b)(i).

By part (b)(ii), under $\mathbb Q_t$ the process $B$ is therefore the zero-started [Ornstein-Uhlenbeck process](../../../../../ornstein-uhlenbeck-process.md):

$$
\boxed{dB_s=dW_s-\beta B_sds,\qquad
B_s=\int_0^se^{-\beta(s-u)}\,dW_u,\quad 0\leq s\leq t.}
$$

This identifies its full law on continuous path space, rather than just its one-time marginal. It is a centered [Gaussian process](../../../../../gaussian-process-split.md), since it consists of deterministic [Itô integrals](../../../../../ito-integral.md) against [Brownian motion](../../../../../brownian-motion-split.md). For $r,s\in[0,t]$, the [Itô isometry](../../../../../ito-isometry.md) gives its [covariance function](../../../../../covariance-function.md):

$$
\boxed{\operatorname{Cov}_{\mathbb Q_t}(B_r,B_s)
=\int_0^{r\wedge s}e^{-\beta(r-u)}e^{-\beta(s-u)}du
=\frac{e^{-\beta|s-r|}-e^{-\beta(s+r)}}{2\beta}.}
$$

In particular, its [Ornstein-Uhlenbeck transition distribution](../../../../../ornstein-uhlenbeck-transition-distribution.md) at the terminal time is

$$
B_t\sim N(0,v_t),\qquad v_t=\frac{1-e^{-2\beta t}}{2\beta}.
$$

## ↑ Ancestors (13)

1. [I](../i.md)
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
