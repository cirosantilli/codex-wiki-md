<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Summing the exact cubic increment identity gives

$$
B_t^3=\sum_j(\Delta B_j)^3
+3\sum_jB_j(\Delta B_j)^2
+3\sum_jB_j^2\Delta B_j.
$$

The first sum tends to zero in [L2 space](../../../../../l2-space-is-a-hilbert-space.md). Indeed, odd [moments](../../../../../moment.md) of centered [normal random variables](../../../../../gaussian-random-variable.md) vanish, a centered [normal random variable](../../../../../gaussian-random-variable.md) of [variance](../../../../../variance-split.md) $v$ has sixth [moment](../../../../../moment.md) $15v^3$, and [independence](../../../../../independent-random-variables.md) of the [Brownian increments](../../../../../brownian-increment.md) gives

$$
\mathbb E\left|\sum_j(\Delta B_j)^3\right|^2
=15\sum_j(\Delta t_j)^3\leq15t|\pi|^2\longrightarrow0.
$$

The second sum converges in [L2 space](../../../../../l2-space-is-a-hilbert-space.md) to $3\int_0^tB_sds$ by (i).

For the last sum, first note that $\mathbb E\int_0^tB_s^4ds=\int_0^t3s^2ds=t^3$, so $B_s^2$ is a [square-integrable stochastic integrand](../../../../../square-integrable-stochastic-integrand.md). If $s=t_j+u$ and $D=B_s-B_j$, then $D$ is [independent](../../../../../independent-random-variables.md) of $B_j$, with $D\sim N(0,u)$. Hence

$$
\mathbb E|B_s^2-B_j^2|^2
=\mathbb E|2B_jD+D^2|^2=4t_ju+3u^2.
$$

It follows that

$$
\mathbb E\int_0^t|B_s^2-B_{\eta(s)}^2|^2ds
\leq2t^2|\pi|+t|\pi|^2\longrightarrow0.
$$

The [Itô isometry](../../../../../ito-isometry.md) therefore makes $\sum_jB_j^2\Delta B_j$ converge in [L2 space](../../../../../l2-space-is-a-hilbert-space.md) to $\int_0^tB_s^2dB_s$, with bounded truncations supplying the initial [simple predictable processes](../../../../../simple-predictable-process.md) if needed. Taking limits in the cubic identity proves

$$
\boxed{\int_0^tB_s^2\,dB_s=\frac13B_t^3-\int_0^tB_s\,ds.}
$$

The proof uses only increment algebra, [moments](../../../../../moment.md) of [normal random variables](../../../../../gaussian-random-variable.md) and the definition of the [Itô integral](../../../../../ito-integral.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
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
