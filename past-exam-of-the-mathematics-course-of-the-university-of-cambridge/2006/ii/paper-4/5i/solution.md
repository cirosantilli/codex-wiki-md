<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

The R command fits a [Poisson regression](../../../../../poisson-regression.md) with the default [log link](../../../../../logarithmic-link-function.md):

$$
Y_i\sim\operatorname{Poisson}(\lambda_i),\qquad
\log\lambda_i=\beta_0+\beta_1T_i,
$$

with independent annual counts conditional on the supplied [temperature](../../../../../temperature.md) index. The fitted mean is $\widehat\lambda(T)=\exp(2.26061+0.48870T)$. The intercept gives about $9.59$ expected named storms at index zero. A one-unit increase in the index multiplies the expected count by $e^{0.48870}\simeq1.63$; a $0.1$ increase multiplies it by about $1.050$.

The reported standard errors estimate the sampling uncertainty of the coefficients. Each displayed $z$ is the estimate divided by its [standard error](../../../../../standard-error.md), compared with a standard [normal distribution](../../../../../normal-distribution.md) under a zero-coefficient null hypothesis. The slope has $z=2.879$ and two-sided $p=0.00399$, evidence of positive association within this model. The intercept test is against mean one at index zero and is not itself a test of a climatic mechanism. Association does not establish causation.

There are $61$ annual observations and two fitted coefficients, giving $59$ residual degrees of freedom. The residual [deviance](../../../../../exponential-family-deviance.md) is

$$
2\sum_i\left[Y_i\log(Y_i/\widehat\lambda_i)-(Y_i-\widehat\lambda_i)\right]=51.499,
$$

with $0\log0=0$. It is not large relative to $59$ and gives no obvious overdispersion signal, although temporal dependence and omitted covariates still require substantive assessment.

For 2005 insert the index into the fitted mean:

$$
\boxed{\widehat\lambda_{2005}=e^{2.26061+0.48870(0.743)}\simeq13.79}.
$$

This is an expected count, approximately fourteen storms, rather than a guarantee of an integer outcome. In R one would use `predict(Mod, newdata=data.frame(Temp=0.743), type="response")`. A predictive distribution must include Poisson variation and, if desired, coefficient-estimation uncertainty; the latter needs the coefficient [covariance matrix](../../../../../covariance-matrix.md), not just the two printed standard errors.

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
