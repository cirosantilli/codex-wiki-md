<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the [logistic regression](../../../../../../logistic-regression.md) as

$$
\operatorname{logit}\{p(A,x)\}=\alpha+\beta A+\gamma^Tx,
$$

where $A=1$ denotes elective exposure and $x$ contains the measured background predictors. At fixed $x$, changing $A$ from zero to one changes the [log odds](../../../../../../log-odds.md) by $\beta$, so the adjusted [odds ratio](../../../../../../odds-ratio.md) is $e^\beta$. If $\widehat V$ is the estimated coefficient [covariance matrix](../../../../../../covariance-matrix.md), then

$$
\boxed{\widehat{\mathrm{OR}}_{\rm adjusted}=e^{\widehat\beta},\qquad
\mathrm{CI}_{95\%}=\left[e^{\widehat\beta-1.96\sqrt{\widehat V_{\beta\beta}}},\ e^{\widehat\beta+1.96\sqrt{\widehat V_{\beta\beta}}}\right].}
$$

Use the clinic-cluster [sandwich covariance matrix](../../../../../../sandwich-covariance-matrix.md) if that is how within-clinic dependence is allowed for. The interval is first calculated on the coefficient scale and then exponentiated; one does not add and subtract a standard error directly from the [odds ratio](../../../../../../odds-ratio.md). This is a large-sample [Wald confidence interval](../../../../../../wald-confidence-interval.md); profile-likelihood limits are another option when the likelihood shape warrants them. If exposure interacts with background variables, there is no single common conditional [odds ratio](../../../../../../odds-ratio.md): its logarithm includes the corresponding interaction terms.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
