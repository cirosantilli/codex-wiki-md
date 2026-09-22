<h1 id="13i/solution">Solution</h1>

↑ **Parent:** [13I](../13i.md)

The first fit is [grouped-binomial logistic regression](../../../../../grouped-binomial-logistic-regression.md): independently, $Y_i\sim\operatorname{Bin}(N_i,\pi_i)$, with the observed group sizes $N_i$ and

$$
\log\frac{\pi_i}{1-\pi_i}=\beta_0+\beta_1 I_{50\text{--}69,i}+\beta_2 I_{70+,i}+\beta_3 I_{\mathrm{malignant},i}.
$$

The reference group is under 50 with a nonmalignant initial tumour. The weights specify binomial numbers of trials, not six equally weighted individual observations. There is no age-by-malignancy interaction. Each age coefficient compares that age group with the reference age at fixed malignancy; $\exp\beta_3$ is the common malignancy odds ratio.

The [maximum-likelihood estimates](../../../../../maximum-likelihood-estimator.md) are obtained by maximizing the [binomial likelihood](../../../../../binomial-likelihood.md). The reported standard errors come from the inverse fitted [Fisher information](../../../../../fisher-information-matrix.md). Each displayed [Wald test](../../../../../wald-test.md) tests a coefficient equal to zero, using $z=\widehat\beta/\operatorname{se}(\widehat\beta)$ and the approximate standard [normal distribution](../../../../../normal-distribution.md); its two-sided probability is $2\Phi(-|z|)$. At the 5% level the middle age coefficient and the malignancy coefficient are significant, with negative signs; the oldest age coefficient is not, although its 9.17% probability is weaker evidence in the same direction. The oldest group has only 19 observations and its larger standard error does not establish absence of an age effect. The intercept tests reference log-odds zero, equivalently reference survival probability $1/2$, rather than an age contrast. The reference fitted probability is about $0.888$; the fitted malignancy odds ratio is about $0.481$.

The [binomial deviance](../../../../../binomial-deviance.md) is twice the saturated-minus-fitted [log-likelihood](../../../../../log-likelihood.md). The null fit has one parameter, hence $6-1=5$ residual degrees of freedom; the first fit has four parameters, hence $6-4=2$. The improvement $12.65585-0.49409=12.16176$ is an approximate [likelihood-ratio test](../../../../../likelihood-ratio-test.md) on three degrees of freedom, with probability about $0.0069$. The residual deviance $0.49409$, compared with $\chi^2_2$, gives about $0.781$, so there is no evidence of lack of fit. These are asymptotic comparisons, especially approximate for the small oldest strata. The [Akaike information criterion](../../../../../akaike-information-criterion.md) is $-2\ell+2p$, here with $p=4$.

Pooling the two older age groups gives a [grouped-binomial logistic regression](../../../../../grouped-binomial-logistic-regression.md) with a common coefficient for age at least 50 and three parameters in total. The similar older-age estimates and the sparse oldest group motivate examining this restriction, but the significance of either coefficient separately is not a test of their equality. The actual [analysis of deviance](../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md) for pooling compares the nested fits: the deviance increases by only $0.784-0.49409\simeq0.28991$ for one lost parameter, giving a $\chi^2_1$ probability about $0.590$. The pooled model also has smaller [Akaike information criterion](../../../../../akaike-information-criterion.md), $28.723$ rather than $30.433$. **Prefer the pooled model for its simpler adequate fit.** Its common age and malignancy coefficients are negative and significant at 5% in the reported [Wald tests](../../../../../wald-test.md).

There is a literal parenthesis error in the printed final R fragment: the first sum is not closed before subtracting the second sum. As printed, the expression is incomplete. Closing that sum gives twice the saturated-minus-fitted [log-likelihood](../../../../../log-likelihood.md), including the binomial constants which cancel. Its intended final value is therefore the second fit's [binomial deviance](../../../../../binomial-deviance.md), **$\boxed{0.784\text{ approximately}}$**.

## ↑ Ancestors (10)

1. [13I](../13i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
