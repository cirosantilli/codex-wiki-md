<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a partition $0=t_0<\cdots<t_n=1$, approximate the integral by $X_\pi=\sum_jt_j(B_{t_{j+1}}-B_{t_j})$, using left endpoints. The defining independent [Brownian increment](../../../../../brownian-increment.md) of [Brownian motion](../../../../../brownian-motion-split.md) make this a centered Gaussian variable with variance $\sum_jt_j^2(t_{j+1}-t_j)$. As the mesh tends to zero, that variance tends to $\int_0^1t^2dt=1/3$.

The [stochastic integral](../../../../../stochastic-integral.md) is the [mean-square convergence](../../../../../convergence-in-l2.md) of these sums. [mean-square convergence](../../../../../convergence-in-l2.md) implies [convergence in distribution](../../../../../convergence-in-distribution.md), while the [characteristic function](../../../../../characteristic-function-split.md) converge to $e^{-u^2/6}$. Hence

$$
\boxed{X\sim N(0,1/3),\qquad\mathbb P(X>0)=\frac12.}
$$

The [probability](../../../../../probability.md) is exactly one half because this centered nondegenerate [normal distribution](../../../../../normal-distribution.md) is symmetric and has no atom at zero.

## ↑ Ancestors (13)

1. [A](../a.md)
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
