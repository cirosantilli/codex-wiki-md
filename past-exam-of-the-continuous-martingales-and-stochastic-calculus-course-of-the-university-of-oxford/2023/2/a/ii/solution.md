<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a bounded [simple predictable process](../../../../../simple-predictable-process.md) $H$ and a [continuous martingale](../../../../../continuous-martingale.md) $M\in\mathcal H^{2,c}$, the [Itô isometry](../../../../../ito-isometry.md) states

$$
\boxed{\mathbb E\left|\int_0^tH_s\,dM_s\right|^2
=\mathbb E\int_0^tH_s^2\,d\langle M\rangle_s.}
$$

Here $\langle M\rangle$ is the [predictable quadratic variation](../../../../../predictable-quadratic-variation.md), equal to $[M]$ for a [continuous martingale](../../../../../continuous-martingale.md). On the whole half-line, the terminal form is

$$
\mathbb E|(H\mathbin\cdot M)_\infty|^2
=\mathbb E\int_0^\infty H_s^2\,d\langle M\rangle_s.
$$

The [Itô integral](../../../../../ito-integral.md) starts at zero even when $M_0\ne0$. For [Brownian motion](../../../../../brownian-motion-split.md), $d\langle B\rangle_s=ds$.

For completeness, cross terms of the finite increment sum have [expectation](../../../../../expected-value-split.md) zero by conditioning on the earlier endpoint of the later increment. Also $M^2-\langle M\rangle$ is a [martingale](../../../../../martingale-split.md), so the remaining terms satisfy

$$
\mathbb E[\xi_j^2(M_v-M_u)^2]
=\mathbb E[\xi_j^2(\langle M\rangle_v-\langle M\rangle_u)]
\quad(u=t_j<t,\ v=t_{j+1}\wedge t).
$$

This proves the displayed identity without a change-of-variables formula. Completing bounded [simple predictable processes](../../../../../simple-predictable-process.md) in the norm $(\mathbb E\int H^2d\langle M\rangle)^{1/2}$ defines the [Itô integral](../../../../../ito-integral.md) of every [square-integrable stochastic integrand](../../../../../square-integrable-stochastic-integrand.md). This completion will justify the unbounded Brownian integrands below.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
