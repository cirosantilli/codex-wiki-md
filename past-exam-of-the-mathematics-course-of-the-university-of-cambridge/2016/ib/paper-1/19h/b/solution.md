<h1 id="19h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Rao-Blackwell theorem](../../../../../../rao-blackwell-theorem.md) says that an unbiased finite-variance [estimator](../../../../../../estimator.md) $\delta(X)$ of a parameter function $\tau(\theta)$ can be improved using a [sufficient statistic](../../../../../../sufficient-statistic.md) $T$. Define

$$
\delta^*(T)=\mathbb E[\delta(X)\mid T].
$$

Because the conditional [distribution](../../../../../../distribution-mathematical-analysis.md) given $T$ is parameter-independent, this is a statistic computable without knowing $\theta$. The [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives $\mathbb E_\theta\delta^*=\mathbb E_\theta\delta=\tau(\theta)$, so it remains unbiased. The [law of total variance](../../../../../../law-of-total-variance.md) gives

$$
\operatorname{Var}_\theta(\delta)=\operatorname{Var}_\theta(\delta^*)+\mathbb E_\theta[\operatorname{Var}_\theta(\delta\mid T)].
$$

Hence **the improved estimator has no larger variance or mean squared error**:

$$
\boxed{\operatorname{Var}_\theta(\delta^*)\leq\operatorname{Var}_\theta(\delta),\qquad \mathbb E_\theta[(\delta^*-\tau(\theta))^2]\leq\mathbb E_\theta[(\delta-\tau(\theta))^2].}
$$

Equality holds precisely when $\delta=\delta^*(T)$ almost surely under the relevant parameter. More generally, even without unbiasedness, [conditional Jensen inequality](../../../../../../conditional-jensen-inequality.md) shows that conditioning on a sufficient statistic cannot increase risk for any convex loss in the estimate, provided the expectations exist. The squared-loss result above is the usual variance form of the theorem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
