<h1 id="8c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Under the null hypothesis the three preference probabilities for girls are each $1/3$. Conditional on their total of sixty, the counts have a [multinomial distribution](../../../../../../multinomial-distribution.md), giving expected counts $(20,20,20)$. The [Pearson chi-squared goodness-of-fit test](../../../../../../pearson-chi-squared-goodness-of-fit-test.md) statistic is

$$
\boxed{X^2=\frac{(13-20)^2+(14-20)^2+(33-20)^2}{20}=12.7.}
$$

No probabilities have been fitted, so the asymptotic null distribution is [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $3-1=2$ degrees of freedom. All expected counts are comfortably large for this approximation. For two degrees of freedom its upper-tail probability is $e^{-X^2/2}$, so

$$
\boxed{p=e^{-6.35}\simeq0.00175.}
$$

At the conventional five-percent or one-percent significance level, **reject equal attractiveness**: there is substantial evidence against the null distribution. No level was specified, so reporting the p-value makes the decision rule explicit. The test assumes independent responses and a sampling interpretation appropriate to the children surveyed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8C](../../8c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
