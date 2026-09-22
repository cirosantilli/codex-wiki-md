<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The increment $B_t-B_s$ is independent of $\mathcal F_s$, with [characteristic function](../../../../../characteristic-function-split.md) $e^{-\xi^2(t-s)/2}$. Since $B_s$ is [measurable](../../../../../measurability.md) at time $s$,

$$
\mathbb E(e^{i\xi B_t}\mid\mathcal F_s)
=e^{i\xi B_s}e^{-\xi^2(t-s)/2}.
$$

The [heat kernel](../../../../../heat-kernel.md) identity in the hint gives $(P_uf)(x)=e^{i\xi x}e^{-\xi^2u/2}$, so this is exactly $(P_{t-s}f)(B_s)$. Multiplying by the deterministic factor $e^{\xi^2t/2}$ gives

$$
\boxed{\mathbb E(M_t\mid\mathcal F_s)=M_s.}
$$

The process is [adapted](../../../../../adapted-process.md), and $|M_t|=e^{\xi^2t/2}$ is finite at each fixed time. Thus it is a complex [martingale](../../../../../martingale-split.md), meaning that its real and imaginary parts are integrable [martingales](../../../../../martingale-split.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
