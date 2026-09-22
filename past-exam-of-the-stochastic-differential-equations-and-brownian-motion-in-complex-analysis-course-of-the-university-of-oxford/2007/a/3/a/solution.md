<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $A_t=\int_0^th(s)dB_s$ and $v_t=\int_0^th(s)^2ds$. [Itô's lemma](../../../../../ito-s-lemma.md) for the exponential gives

$$
dM(h)_t=h(t)M(h)_t\,dB_t.
$$

To justify that this [local martingale](../../../../../local-martingale.md) is true, note that a deterministic [Itô integral](../../../../../ito-integral.md) is Gaussian: step-function approximations are centered Gaussian sums with variances tending to $v_t$, and [Itô isometry](../../../../../ito-isometry.md) gives their convergence. Thus $A_t\sim N(0,v_t)$ and

$$
\mathbb E M(h)_t=1,\qquad
\mathbb E M(h)_t^2=e^{v_t}.
$$

[Continuity](../../../../../continuous-function.md) of $h$ on the [compact](../../../../../compact-space.md) interval bounds $h$ and $v_t$, so

$$
\mathbb E\int_0^Th(t)^2M(h)_t^2dt
=\int_0^Th(t)^2e^{v_t}dt<\infty.
$$

The differential above is therefore a square-integrable [stochastic integral](../../../../../stochastic-integral.md), proving **the [martingale](../../../../../martingale-split.md) property on $[0,T]$**, with initial value one.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
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
