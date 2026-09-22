<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a [filtration](../../../../../filtration-probability-theory.md) with respect to which $B$ is Brownian. The process is adapted and continuous because it is a continuous function of $B_t$ and $t$. The [moment-generating function](../../../../../moment-generating-function.md) gives

$$
\mathbb E M_t=1,\qquad
\mathbb E M_t^2
=e^{-\alpha^2t}\mathbb E e^{2\alpha B_t}
=e^{\alpha^2t}<\infty.
$$

For $0\leq s<t$, write

$$
M_t=M_s\exp\{\alpha(B_t-B_s)-\alpha^2(t-s)/2\}.
$$

The increment is independent of $\mathcal F_s$ and normal with variance $t-s$, so the [conditional expectation](../../../../../conditional-expectation.md) of the second factor is one. Thus

$$
\boxed{\mathbb E(M_t\mid\mathcal F_s)=M_s.}
$$

This verifies the [martingale](../../../../../martingale-split.md) property from the definition and proves square integrability at each finite time, as well as [continuity](../../../../../continuous-function.md). It does not assert uniform square integrability over an infinite time horizon.

## ↑ Ancestors (13)

1. [B](../b.md)
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
