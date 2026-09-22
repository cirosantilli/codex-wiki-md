<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For [independent](../../../../../independent-random-variables.md) [binomial distributions](../../../../../binomial-distribution.md), the [log-likelihood](../../../../../log-likelihood.md), up to known binomial coefficients, is

$$
\ell(p)=\sum_{i=1}^m\{y_i\log p_i+(n_i-y_i)\log(1-p_i)\}.
$$

The [saturated statistical model](../../../../../saturated-statistical-model.md) maximizes each term at $\widetilde p_i=y_i/n_i$. Under the [logit link](../../../../../logit.md), the fitted probabilities are $\widehat p_i=(1+e^{-x_i^T\widehat\beta})^{-1}$. Subtracting the fitted [log-likelihood](../../../../../log-likelihood.md) from the saturated [log-likelihood](../../../../../log-likelihood.md) gives the [binomial deviance](../../../../../binomial-deviance.md)

$$
\boxed{D_1=2\sum_{i=1}^m\left[y_i\log\frac{y_i}{n_i\widehat p_i}
+(n_i-y_i)\log\frac{n_i-y_i}{n_i(1-\widehat p_i)}\right].}
$$

A zero-count summand uses the continuous convention $0\log0=0$. For the restricted model, replace $\widehat p_i$ by $\widehat p_i^{(0)}=(1+e^{-\widetilde x_i^T\widehat{\widetilde\beta}})^{-1}$ to obtain $D_0$. Since the saturated likelihood cancels, $D_0-D_1=2(\widehat\ell_1-\widehat\ell_0)$ is the [likelihood-ratio test statistic](../../../../../likelihood-ratio-test-statistic.md). For the nested restriction setting $p-k$ coefficients to zero, [Wilks theorem](../../../../../wilks-theorem.md) gives the asymptotic [chi-squared distribution](../../../../../chi-squared-distribution.md) $\chi^2_{p-k}$ under regularity and an interior true parameter; reject for a large difference.

For the six anther cells, $\omega_0$ gives a common success probability, $\omega_1$ gives a separate probability for each storage condition, $\omega_2$ gives a common intercept and a log-force slope, and $\omega_3$ gives storage-specific intercepts with a common log-force slope. Their parameter counts are $1,2,2,3$, so their residual [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) are $5,4,4,3$. In $\omega_3$, storage has a constant effect on [log odds](../../../../../log-odds.md); multiplying force by $r$ multiplies the [odds](../../../../../odds.md) by $r^\beta$ in either storage group.

The relevant nested [likelihood-ratio tests](../../../../../likelihood-ratio-test.md) at the $5\%$ level are:

- Adding storage to $\omega_0$ gives $D_0-D_1=5.279>3.84$ on one [statistical degree of freedom](../../../../../statistical-degrees-of-freedom.md), with $p\simeq0.0216$.
- Adding log-force to $\omega_0$ gives $D_0-D_2=2.360<3.84$ on one [statistical degree of freedom](../../../../../statistical-degrees-of-freedom.md), with $p\simeq0.1245$.
- Adding log-force to the storage model gives $D_1-D_3=2.554<3.84$ on one [statistical degree of freedom](../../../../../statistical-degrees-of-freedom.md), with $p\simeq0.1100$.
- Adding storage to the log-force model gives $D_2-D_3=5.473>3.84$ on one [statistical degree of freedom](../../../../../statistical-degrees-of-freedom.md), with $p\simeq0.0193$.
- Adding both terms to $\omega_0$ gives $D_0-D_3=7.833>5.99$ on two [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md), with $p\simeq0.0199$.

The two two-parameter models $\omega_1$ and $\omega_2$ are not nested, so their [deviance](../../../../../exponential-family-deviance.md) difference has no ordinary nested [chi-squared distribution](../../../../../chi-squared-distribution.md) calibration. **The preferred parsimonious model is $\omega_1$, with a storage effect and no log-force effect.** Its [deviance goodness-of-fit test](../../../../../deviance-goodness-of-fit-test.md) is acceptable: $D_1=5.173<9.49$ on four [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). The common-probability model also passes its separate goodness-of-fit comparison, $10.452<11.07$, but this does not contradict the relative evidence for adding storage: the two tests assess different null hypotheses. These are large-sample approximations; sufficiently large expected successes and failures, not merely the number of anthers, underpin their calibration.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
