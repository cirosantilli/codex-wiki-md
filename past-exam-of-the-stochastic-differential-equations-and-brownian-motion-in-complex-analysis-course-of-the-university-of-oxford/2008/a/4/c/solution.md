<h1 id="a/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A finite-horizon form of [Girsanov theorem](../../../../../girsanov-theorem.md) is as follows. If $\theta$ is predictable, $\int_0^T\theta_s^2ds<\infty$ almost surely, and its [stochastic exponential](../../../../../doleans-dade-exponential.md) $M$ is a true [martingale](../../../../../martingale-split.md) of mean one, then under the [probability](../../../../../probability.md) $d\mathbb Q=M_Td\mathbb P$ the process

$$
B_t-\int_0^t\theta_sds,\qquad0\leq t\leq T,
$$

is [Brownian motion](../../../../../brownian-motion-split.md). The same conclusion holds on the completed natural [filtration](../../../../../filtration-probability-theory.md), since a strictly positive density gives equivalent probabilities.

Part (b) establishes precisely the required density [martingale](../../../../../martingale-split.md) and integrand $\theta_s=\partial_x\log p(1-s,B_s,y)$. Therefore

$$
\boxed{X_t=B_t-\int_0^t\frac{y-B_s}{1-s}\,ds
\text{ is }\mathbb Q\text{-Brownian on }[0,T].}
$$

In particular it is the requested [local martingale](../../../../../local-martingale.md). Equivalently, under $\mathbb Q$, $B$ solves $dB_t=(y-B_t)(1-t)^{-1}dt+dX_t$, the [Brownian bridge](../../../../../brownian-bridge.md) [drift coefficient](../../../../../drift-coefficient.md) toward $y$ at time one. Keeping $T<1$ avoids the singular endpoint in this density change.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
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
