<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take

$$
\boxed{\mathcal D(\Delta/2)=C_c^\infty(\mathbb R^d).}
$$

Part (i) proves that [Brownian motion](../../../../../brownian-motion-split.md) solves this [martingale problem](../../../../../martingale-problem.md). For the converse, let $X$ be any continuous [adapted process](../../../../../adapted-process.md) satisfying this [martingale problem](../../../../../martingale-problem.md) and $X_0=0$.

Set $\tau_n=\inf\{t\geq0:|X_t|\geq n\}$. Choose a [smooth cutoff function](../../../../../smooth-cutoff-function.md) $\chi_n$ equal to one on a neighbourhood of the closed ball of radius $n$. Apply the [martingale problem](../../../../../martingale-problem.md) to $\chi_n(x)x_i$ and $\chi_n(x)x_ix_j$, and stop at $\tau_n$. Inside that ball, their [Laplace operators](../../../../../laplace-operator.md) are respectively $0$ and $2\delta_{ij}$. The [optional sampling theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) therefore shows that

$$
X^i_{t\wedge\tau_n},\qquad
X^i_{t\wedge\tau_n}X^j_{t\wedge\tau_n}-\delta_{ij}(t\wedge\tau_n)
$$

are [martingales](../../../../../martingale-split.md). Continuity makes $\tau_n\uparrow\infty$ [almost surely](../../../../../almost-sure-convergence.md). Hence every $X^i$ is a [continuous local martingale](../../../../../continuous-local-martingale.md). The [Itô product rule](../../../../../ito-product-rule.md) and the fact that a [continuous finite-variation local martingale is constant](../../../../../continuous-finite-variation-local-martingale-is-constant.md) identify its [quadratic covariations](../../../../../quadratic-covariation.md):

$$
[X^i,X^j]_t=\delta_{ij}t.
$$

Here $\delta_{ij}$ is the [Kronecker delta](../../../../../kronecker-delta.md).

The [Lévy characterization of multidimensional Brownian motion](../../../../../levy-characterization-of-multidimensional-brownian-motion.md) now applies. To see explicitly why it identifies the entire law, for $\xi\in\mathbb R^d$ the [Itô formula](../../../../../ito-s-lemma.md) makes

$$
E_t(\xi)=\exp\!\left(i\xi\cdot X_t+\frac12|\xi|^2t\right)
$$

a complex [local martingale](../../../../../local-martingale.md). Its absolute value on $[0,T]$ is at most $e^{|\xi|^2T/2}$, so the [bounded local martingale criterion](../../../../../bounded-local-martingale-criterion.md) makes it a true [martingale](../../../../../martingale-split.md) there. For $0\leq s\leq t$,

$$
\boxed{\mathbb E\!\left[e^{i\xi\cdot(X_t-X_s)}\mid\mathcal F_s\right]
=e^{-|\xi|^2(t-s)/2}.}
$$

This conditional [characteristic function](../../../../../characteristic-function-split.md) identifies $X_t-X_s$ as having a centered [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) with [covariance matrix](../../../../../covariance-matrix.md) $(t-s)I$, [independent](../../../../../independent-random-variables.md) of $\mathcal F_s$. Together with continuity and $X_0=0$, these are exactly the defining properties of standard $d$-dimensional [Brownian motion](../../../../../brownian-motion-split.md). Thus the [martingale problem for Brownian motion](../../../../../martingale-problem-for-brownian-motion.md) has a unique law.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
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
