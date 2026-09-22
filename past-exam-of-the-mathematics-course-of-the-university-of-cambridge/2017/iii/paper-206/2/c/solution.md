<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Using the smaller [logistic regression](../../../../../../logistic-regression.md), approximate pointwise [Wald confidence intervals](../../../../../../wald-confidence-interval.md) are an estimate plus or minus $1.96$ times its [standard error](../../../../../../standard-error.md):

$$
\boxed{\widehat\beta_0=5.16258,\quad \beta_0\in[2.94717,7.37799];\qquad \widehat\beta_1=-0.08207,\quad \beta_1\in[-0.113332,-0.050808].}
$$

Both intervals rely on the large-sample [normal approximation](../../../../../../normal-approximation.md) and correct model assumptions. The negative slope indicates decreasing purchase probability as price rises. A one-unit price increase multiplies the [odds](../../../../../../odds.md) by $e^{-0.08207}\simeq0.9212$; it does not subtract a fixed amount from the probability. There is no significant additional layout effect in the previous [likelihood-ratio test](../../../../../../likelihood-ratio-test.md), rather than a demonstration of no effect.

In the selected model layout B has the same prediction rule as the other layouts. At price 100 the [linear predictor](../../../../../../linear-predictor.md) is $5.16258-0.08207(100)=-3.04442$. Applying the inverse [logit link](../../../../../../logit.md) gives

$$
\boxed{\widehat p(100,B)=\frac{1}{1+e^{3.04442}}\simeq0.04546.}
$$

The intercept refers to price zero; if that lies outside the observed price range, its direct substantive interpretation would require extrapolation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
