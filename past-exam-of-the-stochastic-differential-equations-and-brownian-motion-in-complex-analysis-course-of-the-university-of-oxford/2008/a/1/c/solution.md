<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Lévy's characterization of Brownian motion](../../../../../levy-characterization-of-brownian-motion.md) states that a real continuous [local martingale](../../../../../local-martingale.md) $M$ with $M_0=0$ and [quadratic variation](../../../../../quadratic-variation.md) $\langle M\rangle_t=t$ is a standard [Brownian motion](../../../../../brownian-motion-split.md) with respect to its [filtration](../../../../../filtration-probability-theory.md). Equivalently, its increments are independent of the past and have centered [normal distribution](../../../../../normal-distribution.md) with variances equal to elapsed times.

Let $H_s=\operatorname{sgn}(\sup_{r\leq s}B_r-1)$. The running maximum is continuous and adapted, so $H$ is bounded and [progressively measurable process](../../../../../progressive-measurability.md). It has a predictable version for integration; changing its value at the single switching time does not change its [stochastic integral](../../../../../stochastic-integral.md). Thus $X=\int H\,dB$ is a continuous [local martingale](../../../../../local-martingale.md) starting at zero. Since $H_s^2=1$,

$$
\langle X\rangle_t=\int_0^tH_s^2ds=t.
$$

[Lévy's characterization of Brownian motion](../../../../../levy-characterization-of-brownian-motion.md) yields **$X$ is standard [Brownian motion](../../../../../brownian-motion-split.md)**. The sign depends on the entire past through the running maximum, but the unit quadratic-variation rate is exactly what the characterization needs.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
