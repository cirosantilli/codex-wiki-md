<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Fix $t>0$, a deterministic [partition of an interval](../../../../../partition-of-an-interval.md) $\pi$, and write $\eta(s)=t_j$ on $[t_j,t_{j+1})$. Its mesh is $|\pi|=\max_j(t_{j+1}-t_j)$. The [Brownian increment](../../../../../brownian-increment.md) [variance](../../../../../variance-split.md) gives

$$
\mathbb E\int_0^t|B_s-B_{\eta(s)}|^2ds
=\frac12\sum_j(\Delta t_j)^2\leq\frac{t|\pi|}{2}.
$$

Thus the left-endpoint sums $\sum_jB_{t_j}\Delta B_j$ converge in [L2 space](../../../../../l2-space-is-a-hilbert-space.md) to the [Itô integral](../../../../../ito-integral.md). Although these step coefficients are unbounded, clipping them at finite levels first makes them bounded [simple predictable processes](../../../../../simple-predictable-process.md); the [Itô isometry](../../../../../ito-isometry.md) and their finite second [moments](../../../../../moment.md) remove the clipping.

The elementary identity $B_{t_{j+1}}^2-B_{t_j}^2=2B_{t_j}\Delta B_j+(\Delta B_j)^2$ gives

$$
2\sum_jB_{t_j}\Delta B_j=B_t^2-\sum_j(\Delta B_j)^2.
$$

The squared [Brownian increments](../../../../../brownian-increment.md) are [independent](../../../../../independent-random-variables.md), with [means](../../../../../expected-value-split.md) $\Delta t_j$ and [variances](../../../../../variance-split.md) $2(\Delta t_j)^2$, since a centered [normal random variable](../../../../../gaussian-random-variable.md) of [variance](../../../../../variance-split.md) $v$ has fourth [moment](../../../../../moment.md) $3v^2$. Therefore

$$
\mathbb E\left|\sum_j(\Delta B_j)^2-t\right|^2
=2\sum_j(\Delta t_j)^2\leq2t|\pi|\longrightarrow0.
$$

Passing to the [convergence in L2](../../../../../convergence-in-l2.md) limits yields

$$
\boxed{\int_0^tB_s\,dB_s=\frac12(B_t^2-t).}
$$

This holds for each fixed $t$; continuous [sample paths](../../../../../sample-path.md) of both sides extend equality from rational times to all $t$ on one event of [probability](../../../../../probability.md) one.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
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
