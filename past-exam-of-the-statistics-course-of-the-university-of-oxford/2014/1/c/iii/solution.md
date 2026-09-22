<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**Prefer Student 2's paired analysis**, because the observational units are matched pairs: two shoes exposed to the same child's activity. A [paired t-test](../../../../../paired-t-test.md) uses $Y_i=A_i-B_i$, so shared child-to-child variation is removed before estimating the [standard error](../../../../../standard-error.md). The independent units are the ten pairs, giving $9$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) under the model of independent normally distributed pair differences.

The role of [covariance](../../../../../covariance.md) is explicit:

$$
\operatorname{Var}(A_i-B_i)=\operatorname{Var}(A_i)+\operatorname{Var}(B_i)-2\operatorname{Cov}(A_i,B_i).
$$

With common marginal [variance](../../../../../variance-split.md) $\sigma^2$ and within-pair [correlation coefficient](../../../../../pearson-correlation-coefficient.md) $\rho$, the true [variance](../../../../../variance-split.md) of the average difference is $2\sigma^2(1-\rho)/10$. The independent-groups calculation ignores the covariance term and uses $2\sigma^2/10$. Positive within-pair association can therefore make the paired [standard error](../../../../../standard-error.md) much smaller, explaining how the reported [p-values](../../../../../p-value.md) can differ without arithmetic mistakes. The preference follows from the paired design, not from selecting the smaller [p-value](../../../../../p-value.md). Marginal normality alone need not imply normally distributed differences; exact paired inference uses the normal-difference assumption, for example justified by a joint [multivariate normal distribution](../../../../../multivariate-normal-distribution.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
