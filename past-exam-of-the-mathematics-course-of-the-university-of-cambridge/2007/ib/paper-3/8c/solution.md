<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

Under the null hypothesis, the defect count in each packet has a [binomial distribution](../../../../../binomial-distribution.md) with parameters $3,\theta$. The [likelihood](../../../../../likelihood-function.md), apart from factors independent of $\theta$, is

$$
L(\theta)\propto\theta^{94+2(40)+3(6)}(1-\theta)^{3(116)+2(94)+40}=\theta^{192}(1-\theta)^{576}.
$$

The [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) is therefore

$$
\boxed{\widehat\theta=\frac{192}{768}=\frac14.}
$$

The fitted [binomial distribution](../../../../../binomial-distribution.md) probabilities for counts $0,1,2,3$ are $27/64,27/64,9/64,1/64$, yielding expected packet counts $108,108,36,4$. The [Pearson chi-squared goodness-of-fit test](../../../../../pearson-chi-squared-goodness-of-fit-test.md) uses

$$
X^2=\frac{(116-108)^2}{108}+\frac{(94-108)^2}{108}+\frac{(40-36)^2}{36}+\frac{(6-4)^2}{4}=\boxed{\frac{104}{27}\simeq3.852}.
$$

For [binomial goodness-of-fit with an estimated parameter](../../../../../binomial-goodness-of-fit-with-an-estimated-parameter.md), there are $4-1-1=2$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md): the category counts have a fixed total, and one parameter was estimated. At the conventional $5\%$ level the [chi-squared distribution](../../../../../chi-squared-distribution.md) with two [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) has upper critical value $5.99$, so **the data do not reject the independent common-defect-probability model**. The approximate [p-value](../../../../../p-value.md) is $e^{-X^2/2}\simeq0.146$; even at $10\%$, the critical value $4.61$ exceeds the observed statistic.

This is a goodness-of-fit conclusion rather than proof that individual bulbs are independent. The last expected count is only $4$, so the [chi-squared asymptotic approximation](../../../../../chi-squared-asymptotic-approximation.md) is somewhat marginal in that cell. The stated calibration is the usual asymptotic test with all four cells retained; if more accurate small-count inference is required, calibrate the fitted statistic under the [binomial distribution](../../../../../binomial-distribution.md) model. Pooling cells would require a corresponding treatment of parameter fitting and test calibration.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
