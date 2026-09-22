<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The geometry of a strictly convex [normed space](../../../../../normed-vector-space-split.md) proves [uniqueness](../../../../../uniqueness.md) whenever a [best approximation](../../../../../best-approximation-in-a-normed-space.md) exists. If distinct $p_1,p_2$ both have best error $E>0$, then their two residuals have [norm](../../../../../norm.md) $E$. The defining midpoint inequality gives

$$
\left\|u-\frac{p_1+p_2}{2}\right\|
=\left\|\frac{(u-p_1)+(u-p_2)}2\right\|<E,
$$

contradicting [best approximation](../../../../../best-approximation-in-a-normed-space.md) because the midpoint lies in $A$. If $E=0$, both approximants equal $u$.

The printed [existence](../../../../../existence.md) assertion is false for an arbitrary [vector subspace](../../../../../vector-subspace.md). For a concrete counterexample take $B=\ell^2$ with its strictly convex Hilbert [norm](../../../../../norm.md), let $A=c_{00}$ be its finite-support sequences, and take $u=(2^{-j})_{j\geq1}$. Truncations in $A$ tend to $u$, so the best-error [infimum](../../../../../infimum.md) is zero, but $u\notin A$ and that [infimum](../../../../../infimum.md) is not attained. If the finite-dimensional assumption of part (b) is retained, it supplies [existence](../../../../../existence.md) and the argument above supplies [uniqueness](../../../../../uniqueness.md).

For the estimate, suppose $Y$ is a [projection operator](../../../../../projection-linear-algebra.md) onto $A$, as needed for a finite [operator norm](../../../../../operator-norm.md). Since $Yp=p$,

$$
u-Yu=(u-p)-Y(u-p).
$$

The [triangle inequality](../../../../../triangle-inequality.md) and [operator norm](../../../../../operator-norm.md) give

$$
\boxed{\|u-Yu\|\leq(1+\|Y\|)\|u-p\|
=(1+\|Y\|)E.}
$$

The estimate actually holds without attainment: apply it with any $q\in A$ instead of $p$ and take the [infimum](../../../../../infimum.md). Its proof applies in every [normed space](../../../../../normed-vector-space-split.md). This is [strict convexity separates uniqueness from existence in best approximation](../../../../../strict-convexity-separates-uniqueness-from-existence-in-best-approximation.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
