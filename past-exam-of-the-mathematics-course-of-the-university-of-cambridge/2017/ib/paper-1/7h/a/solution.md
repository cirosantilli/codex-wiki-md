<h1 id="7h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Rao-Blackwell theorem](../../../../../../rao-blackwell-theorem.md) applies to an [estimator](../../../../../../estimator.md) $Y$ with finite second moment and a [sufficient statistic](../../../../../../sufficient-statistic.md) $T$. The conditional [estimator](../../../../../../estimator.md) $Y^*=\mathbb E_\theta[Y\mid T]$ can be chosen as a function of the observed $T$ that does not depend on the unknown parameter: this uses the parameter-independent conditional data distribution in the definition of [sufficient statistic](../../../../../../sufficient-statistic.md). The [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives $\mathbb E_\theta Y^*=\mathbb E_\theta Y$, so their [bias](../../../../../../bias-of-an-estimator.md) agrees. The [law of total variance](../../../../../../law-of-total-variance.md) gives

$$
\operatorname{Var}_\theta Y=\operatorname{Var}_\theta Y^*+\mathbb E_\theta\operatorname{Var}_\theta(Y\mid T).
$$

For any target $a(\theta)$ it follows that

$$
\boxed{\mathbb E_\theta[(Y^*-a(\theta))^2]\le\mathbb E_\theta[(Y-a(\theta))^2]}.
$$

Equality holds exactly when $Y=Y^*$ almost surely under that parameter value. This proves variance reduction and reduction of [mean squared error](../../../../../../mean-squared-error.md), whether or not the original [estimator](../../../../../../estimator.md) is an [unbiased estimator](../../../../../../unbiased-estimator.md). More generally, [conditional Jensen inequality](../../../../../../conditional-jensen-inequality.md) proves the corresponding inequality for any convex loss in the estimate, whenever the expectations exist.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7H](../../7h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
