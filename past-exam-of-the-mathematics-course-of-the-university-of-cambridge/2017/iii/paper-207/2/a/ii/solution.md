<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Under the intended additional assumption of mutually [independent](../../../../../../../independent-random-variables.md), continuously calibrated null [p-values](../../../../../../../p-value.md), each test fails to reject with [probability](../../../../../../../probability.md) $0.95$. The [familywise error rate](../../../../../../../familywise-error-rate.md) is therefore

$$
\boxed{\mathbb P(\text{at least one false rejection})=1-0.95^{10}\simeq0.4013.}
$$

There is a qualification to the printed use of “not correlated”: zero pairwise [correlation coefficients](../../../../../../../pearson-correlation-coefficient.md) do not generally imply mutual [independence](../../../../../../../independent-random-variables.md). A [multivariate normal distribution](../../../../../../../multivariate-normal-distribution.md) with zero off-diagonal [covariances](../../../../../../../covariance.md) does give [independence](../../../../../../../independent-random-variables.md), but an arbitrary biomarker distribution need not. The formula above requires [independent](../../../../../../../independent-random-variables.md) rejection events, not just uncorrelated measurements.

The usual intuition for positively dependent tests is that they reject together, reducing the effective number of opportunities for a false positive. A rigorous sufficient assumption is [positive association of random variables](../../../../../../../positive-association-of-random-variables.md) for the rejection indicators $I_1,\ldots,I_{10}$. Products of their non-rejection indicators are decreasing functions; association and induction give

$$
\mathbb P(I_1=\cdots=I_{10}=0)\geq\prod_i\mathbb P(I_i=0)=0.95^{10}.
$$

Thus **under this stronger positive-dependence assumption the [probability](../../../../../../../probability.md) is no larger**, and perfect dependence gives $0.05$ instead of $0.4013$. Strict inequality is not forced by every form of positive dependence.

Pairwise positive [correlation coefficients](../../../../../../../pearson-correlation-coefficient.md) alone, as printed, is insufficient. For a counterexample choose a vector of ten [exchangeable random variables](../../../../../../../exchangeable-random-variables.md) that are rejection indicators as follows: with [probabilities](../../../../../../../probability.md) $0.545,0.450,0.005$, respectively, reject none, reject one uniformly selected test, or reject all ten. Then

$$
\mathbb P(I_i=1)=0.05,\qquad \mathbb P(I_i=I_j=1)=0.005>0.05^2\quad(i\ne j),
$$

but the [familywise error rate](../../../../../../../familywise-error-rate.md) is $0.455>1-0.95^{10}$. This can be realized with valid null [p-values](../../../../../../../p-value.md): conditional on the indicators, independently draw $p_i$ uniformly on $(0,0.05)$ if $I_i=1$ and on $(0.05,1)$ otherwise. Every $p_i$ is uniform on $(0,1)$, and $\operatorname{Cov}(p_i,p_j)=0.25\operatorname{Cov}(I_i,I_j)>0$. Taking biomarker statistics $X_i=1-p_i$ gives pairwise positively correlated null statistics with exactly these one-sided tests. Therefore the unconditional larger-or-smaller claim needs a specified dependence model.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
