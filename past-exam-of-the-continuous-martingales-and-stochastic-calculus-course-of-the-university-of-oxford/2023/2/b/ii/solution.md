<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the exact discrete product identity

$$
t_{j+1}B_{j+1}-t_jB_j=t_j\Delta B_j+B_{j+1}\Delta t_j
$$

and sum over the deterministic [partition of an interval](../../../../../partition-of-an-interval.md). Since $B_0=0$,

$$
\sum_jt_j\Delta B_j=tB_t-\sum_jB_{j+1}\Delta t_j.
$$

The left side converges in [L2 space](../../../../../l2-space-is-a-hilbert-space.md) to $\int_0^ts\,dB_s$ by the definition and [Itô isometry](../../../../../ito-isometry.md), since

$$
\int_0^t|s-\eta(s)|^2ds
=\frac13\sum_j(\Delta t_j)^3\leq\frac{t|\pi|^2}{3}.
$$

The right-endpoint [Riemann sum](../../../../../riemann-sum.md) converges in [L2 space](../../../../../l2-space-is-a-hilbert-space.md) to $\int_0^tB_sds$: its squared error is at most

$$
t\sum_j\int_{t_j}^{t_{j+1}}\mathbb E|B_{j+1}-B_s|^2ds
=\frac t2\sum_j(\Delta t_j)^2\longrightarrow0.
$$

Consequently,

$$
\boxed{\int_0^ts\,dB_s=tB_t-\int_0^tB_s\,ds.}
$$

As in (a)(iii), continuity extends fixed-time equality to equality of the continuous processes.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
