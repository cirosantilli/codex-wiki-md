<h1 id="6/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

In [statistical decision theory](../../../../../../statistical-decision-theory.md), the [statistical invariance principle](../../../../../../statistical-invariance-principle.md) says that a procedure should respect transformations that leave the inferential problem unchanged. If a [group action](../../../../../../group-action.md) preserves the model and carries each of the null and alternative parameter sets into itself, an invariant test has rejection probability function $\varphi(gy)=\varphi(y)$. A [maximal invariant](../../../../../../maximal-invariant.md) identifies its orbits, so every invariant test factors through that statistic: define its value at an orbit using any representative; invariance makes the definition [independent](../../../../../../independent-random-variables.md) of the representative. If the [group](../../../../../../group-split.md) is transitive on the null parameter set, the null law of any invariant statistic is free of that [nuisance parameter](../../../../../../nuisance-parameter.md).

For example, testing a normal mean $\mu=\mu_0$ with unknown scale, positive transformations $y_i-\mu_0\mapsto b(y_i-\mu_0)$ preserve a one-sided mean alternative. The statistic $\sqrt n(\bar Y-\mu_0)/s$, with the usual unbiased sample-[variance](../../../../../../variance-split.md) scale $s$, is invariant and has the [Student t-distribution](../../../../../../student-s-t-distribution.md) with $n-1$ degrees of freedom under the null. For estimation the corresponding requirement is an [equivariant estimator](../../../../../../equivariant-estimator.md), together with a [loss function](../../../../../../loss-function.md) invariant under simultaneous transformation of decision and parameter. Invariance alone does not prove unrestricted optimality or supply a unique best procedure.

There is a distinct probabilistic use of the term: the [Donsker invariance principle](../../../../../../donsker-s-theorem.md) states that centred iid partial sums, normalized by $\sigma\sqrt n$, converge as processes on $[0,1]$ to [Brownian motion](../../../../../../brownian-motion-split.md). Its empirical-process version gives a [Brownian bridge](../../../../../../brownian-bridge.md), used by goodness-of-fit tests in the next note. These functional limit theorems should be distinguished from the [group](../../../../../../group-split.md)-based inferential principle.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [6](../../6.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
