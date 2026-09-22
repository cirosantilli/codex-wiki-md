<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Average the [conditional probability](../../../../../conditional-probability.md) in (i) over $Y\sim q=\widetilde q/Z_q$:

$$
\begin{aligned}
\mathbb P(\mathrm{accept})
&=\int_\Omega\frac{\widetilde q(y)}{Z_q}
\frac{\widetilde p(y)}{M\widetilde q(y)}\,dy\\
&=\frac1{MZ_q}\int_\Omega\widetilde p(y)\,dy
=\boxed{\frac{Z_p}{MZ_q}}.
\end{aligned}
$$

This is exactly the [acceptance mass for an unnormalized rejection envelope](../../../../../acceptance-mass-for-an-unnormalized-rejection-envelope.md). In normalized form the envelope is $p\leq(MZ_q/Z_p)q$, giving the same acceptance [probability](../../../../../probability.md). Here $M$ bounds the ratio of the unnormalized functions, so its value need not equal the envelope constant for the normalized [probability density functions](../../../../../probability-density-function.md).

The squeeze changes the number of expensive target evaluations, while preserving the per-proposal acceptance [probability](../../../../../probability.md). The expected number of proposals per accepted draw is $MZ_q/Z_p$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
