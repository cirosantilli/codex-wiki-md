<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A sufficient condition is that $x\mapsto\sqrt{2\theta(x)}$ is [globally Lipschitz](../../../../../globally-lipschitz-function.md). A more familiar, stronger condition implying this is that $\theta$ is [globally Lipschitz](../../../../../globally-lipschitz-function.md) and $\theta\geq\varepsilon>0$. Both conditions repair the existence issue in part (i).

To connect this to the suggested [stochastic differential equation](../../../../../stochastic-differential-equation.md), apply the coordinate and coordinate-product cutoff tests to any solution of the [martingale problem](../../../../../martingale-problem.md). As before they give

$$
[X^i,X^j]_t=2\delta_{ij}\int_0^t\theta(X_s)\,ds.
$$

Define, using [stochastic integrals](../../../../../stochastic-integral.md) against the coordinates of $X$,

$$
W_t^i=\int_0^t\frac{1}{\sqrt{2\theta(X_s)}}\,dX_s^i.
$$

These integrals exist even without a global positive lower bound: their [quadratic variations](../../../../../quadratic-variation.md) are exactly $t$. Indeed,

$$
[W^i,W^j]_t
=\int_0^t\frac{1}{2\theta(X_s)}\,d[X^i,X^j]_s
=\delta_{ij}t.
$$

The [Lévy characterization of multidimensional Brownian motion](../../../../../levy-characterization-of-multidimensional-brownian-motion.md) identifies $W$ as standard $d$-dimensional [Brownian motion](../../../../../brownian-motion-split.md). By [associativity of stochastic integration](../../../../../associativity-of-stochastic-integration.md),

$$
\boxed{dX_t=\sqrt{2\theta(X_t)}\,dW_t,\qquad X_0=0.}
$$

The diffusion matrix $\sqrt{2\theta(x)}I$ is [globally Lipschitz](../../../../../globally-lipschitz-function.md) under the stated condition, and boundedness of $\theta$ gives bounded growth. The [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../../../global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients.md) gives a unique [strong solution of a stochastic differential equation](../../../../../strong-solution-of-a-stochastic-differential-equation.md) and [uniqueness in law](../../../../../uniqueness-in-law.md). Every solution to the [martingale problem](../../../../../martingale-problem.md) has just been represented as a [weak solution of a stochastic differential equation](../../../../../weak-solution-of-a-stochastic-differential-equation.md) of this form, so they all have the same law. Conversely, the [Itô formula](../../../../../ito-s-lemma.md) applied to any $f\in C_c^\infty$ gives a true [martingale](../../../../../martingale-split.md), since its stochastic integrand is bounded. Thus the [martingale problem](../../../../../martingale-problem.md) is well posed under this sufficient condition.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
