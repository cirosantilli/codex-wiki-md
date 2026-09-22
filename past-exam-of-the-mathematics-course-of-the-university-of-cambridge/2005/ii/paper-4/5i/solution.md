<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

The first two commands create [vectors](../../../../../vector.md) of observed successes and corresponding numbers of trials. The next two create the class labels and convert them into an R [factor](../../../../../regression-factor.md), so the labels are treated categorically. The final command fits a [grouped-binomial logistic regression](../../../../../grouped-binomial-logistic-regression.md), using the proportions as responses and trial totals as binomial weights, and prints its summary. The model is $\log[\pi_i/(1-\pi_i)]=\beta_0+\beta_b\mathbf1_{\{S_i=b\}}$, with class a as reference.

The intercept estimates the [log odds](../../../../../log-odds.md) in class a. Its value corresponds to [probability](../../../../../probability.md) $39/287\approx0.1359$. The class-b coefficient is the estimated increase in [log odds](../../../../../log-odds.md), about $0.4999$, so the fitted [probability](../../../../../probability.md) in class b is $35/170\approx0.2059$ and the estimated [odds ratio](../../../../../odds-ratio.md) is $e^{0.4999}\approx1.6485$. The printed [standard errors](../../../../../standard-error.md) measure uncertainty in these estimated coefficients. The z values are estimate divided by [standard error](../../../../../standard-error.md): the intercept tests whether the class-a [probability](../../../../../probability.md) is $1/2$, while the class-b z value tests equal class [probabilities](../../../../../probability.md). The two-sided normal-reference [P-value](../../../../../p-value.md) for the latter is about $0.051$, so it is just above a conventional $5\%$ threshold; this is a borderline result rather than strong evidence of a class effect.

The residual [deviance](../../../../../exponential-family-deviance.md) compares the fitted two-parameter model with the four-probability saturated model. Its value $1.9369$ on $4-2=2$ residual degrees of freedom is small relative to a $\chi_2^2$ reference, with approximate tail [probability](../../../../../probability.md) $e^{-1.9369/2}\approx0.380$. There is no evidence of lack of fit by that check. Four [Fisher scoring](../../../../../scoring-algorithm.md) iterations were needed for numerical fitting. These interpretations presume independent binomial counts and the usual large-sample approximations; weights here encode trial counts, not extra independent observations.

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
