<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $Y_i=1$ indicate a depressed outcome and $C_i=1$ indicate the control arm. A [logistic regression](../../../../../../logistic-regression.md) could specify

$$
\log\frac{p_i}{1-p_i}=\beta_0+\beta_C C_i+\gamma^T x_i,
\qquad p_i=\Pr(Y_i=1\mid C_i,x_i),
$$

with $x_i$ containing prespecified baseline characteristics, including the stratification factor. Fit the coefficients by maximizing the [likelihood](../../../../../../likelihood-function.md) for independent [Bernoulli random variables](../../../../../../bernoulli-distribution.md) $\prod_i p_i^{Y_i}(1-p_i)^{1-Y_i}$. For equal [covariate](../../../../../../covariate.md) values the control-to-intervention [odds ratio](../../../../../../odds-ratio.md) is $e^{\beta_C}$. Thus an estimate $\widehat\beta_C=\log(2.1)$ produces the quoted adjusted ratio. An ordinary [Wald confidence interval](../../../../../../wald-confidence-interval.md) is obtained by exponentiating the endpoints of the coefficient's [confidence interval](../../../../../../confidence-interval.md).

The raw control-to-intervention [odds ratio](../../../../../../odds-ratio.md), using the actual counts, is

$$
\boxed{\frac{78/(316-78)}{40/(297-40)}
=\frac{78\cdot257}{238\cdot40}\simeq2.106.}
$$

Using only the quoted percentages gives about $2.05$, so both versions are approximately $2.1$. The printed $14\%$ is not the usual whole-percentage rounding of $40/297\simeq13.47\%$; using the counts avoids that small numerical inconsistency. The reversed intervention-to-control ratio is about $0.475$.

The apparent surprise is a coding issue: with depression as the adverse outcome and intervention relative to control, protection would give an [odds ratio](../../../../../../odds-ratio.md) below one. A ratio above one is favourable if the comparison is control relative to intervention, as above, or if the outcome has been recoded as absence of depression and intervention is compared with control. Both comparison and outcome must be specified. The adjusted ratio need not equal the crude one, even in a randomized trial: [covariate](../../../../../../covariate.md) adjustment and [noncollapsibility of the odds ratio](../../../../../../noncollapsibility-of-the-odds-ratio.md) can change an [odds ratio](../../../../../../odds-ratio.md). Their close numerical values here do not prove that the regression adjustment was unnecessary.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
