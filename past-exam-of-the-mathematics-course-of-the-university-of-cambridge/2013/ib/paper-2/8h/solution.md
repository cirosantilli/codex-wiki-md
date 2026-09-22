<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

The [Rao-Blackwell theorem](../../../../../rao-blackwell-theorem.md) says that if $S$ is a [sufficient statistic](../../../../../sufficient-statistic.md) and $\delta$ a finite-variance [estimator](../../../../../estimator.md), then $\delta^*=\mathbb E(\delta\mid S)$ is an [estimator](../../../../../estimator.md) with the same expectation and no larger [variance](../../../../../variance-split.md). Sufficiency ensures the conditional distribution, and hence this formula as a function of the data, does not involve the unknown parameter. The [tower property of conditional expectation](../../../../../law-of-total-expectation.md) gives $\mathbb E\delta^*=\mathbb E\delta$, while the [law of total variance](../../../../../law-of-total-variance.md) gives

$$
\operatorname{Var}(\delta)=\operatorname{Var}(\delta^*)+\mathbb E\operatorname{Var}(\delta\mid S).
$$

This proves the theorem and shows that equality holds exactly when $\delta$ is already determined by $S$, almost surely. In particular, unbiasedness is preserved.

Assume $n\geq3$. Independence gives $\mathbb E\hat\theta=p_0p_1p_2=\theta$, so the proposed indicator is unbiased and has [variance](../../../../../variance-split.md) $\theta(1-\theta)$. The type counts $S=(n_0,n_1,n_2)$ are a [sufficient statistic](../../../../../sufficient-statistic.md): conditional on them, every ordering of the labels is equally likely. Consequently,

$$
\boxed{\theta^*=\mathbb E(\hat\theta\mid S)=\frac{n_0n_1n_2}{n(n-1)(n-2)}.}
$$

For example, the conditional probability of the ordered first three labels is $(n_0/n)(n_1/(n-1))(n_2/(n-2))$. This is [Rao-Blackwellization of a multinomial probability product](../../../../../rao-blackwellization-of-a-multinomial-probability-product.md).

If all three $p_i$ are positive, there is positive probability that all three counts are positive. On such an event the conditional indicator has probability strictly between zero and one, so its [conditional variance](../../../../../conditional-variance.md) is positive. Thus **$\operatorname{Var}(\theta^*)<\theta(1-\theta)$ for interior parameter values**. If any $p_i=0$, then $\theta=0$ and both [estimators](../../../../../estimator.md) have zero [variance](../../../../../variance-split.md); the printed strict inequality is impossible at those boundary parameters. The valid unrestricted statement is the non-strict inequality.

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
