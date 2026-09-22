<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $K=\sum_i\|A^i\|_{\mathrm{op}}^2$, where the norms are [operator norms](../../../../../operator-norm.md), and $D_m=y^{(m+1)}-y^{(m)}$. Independence of the Brownian coordinates and the vector [Itô isometry](../../../../../ito-isometry.md) give

$$
\mathbb E|D_0(t)|^2\leq |a|^2Kt,\qquad
\mathbb E|D_m(t)|^2\leq K\int_0^t\mathbb E|D_{m-1}(s)|^2ds.
$$

Induction, as in part (b), yields the [Factorial Picard estimate for a linear stochastic differential equation](../../../../../factorial-picard-estimate-for-a-linear-stochastic-differential-equation.md)

$$
\mathbb E|D_m(t)|^2\leq |a|^2\frac{(Kt)^{m+1}}{(m+1)!}.
$$

For $t\leq T$, the [triangle inequality](../../../../../triangle-inequality.md) in $L^2$ therefore bounds any tail of the iterates by the corresponding tail of

$$
|a|\sum_{m\geq0}\frac{(KT)^{(m+1)/2}}{\sqrt{(m+1)!}}.
$$

This numerical series converges by the [ratio test](../../../../../ratio-test.md): successive terms have ratio $\sqrt{KT/(m+2)}\to0$. Thus the iterates are Cauchy in $L^2$, uniformly in the deterministic time parameter on each bounded interval. [Completeness of Lp spaces](../../../../../completeness-of-lp-spaces.md) gives a limit $y_t$. Once its continuous adapted version is chosen in part (d), the [Itô isometry](../../../../../ito-isometry.md) permits passage to the limit in the integral equation: the squared norm of each integral difference is bounded by $K\int_0^T\mathbb E|y_s^{(m)}-y_s|^2ds\to0$. Consequently **the Picard limit solves the stochastic differential equation**.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
