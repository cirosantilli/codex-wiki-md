<h1 id="o/o1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For equal one-second observation windows, the [sample mean](../../../../../sample-mean.md) estimates the [Poisson distribution](../../../../../poisson-distribution.md) mean:

$$
\boxed{\widehat\lambda=10192/12169\simeq0.83754.}
$$

This matches the expected mean count; it is also the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) for independent [Poisson distribution](../../../../../poisson-distribution.md) observations. With $N=12169$ windows, fitted expected frequencies are $E_j=N e^{-\widehat\lambda}\widehat\lambda^j/j!$ for $j=0,\ldots,4$, and $E_{\geq5}=N[1-\sum_{j=0}^4e^{-\widehat\lambda}\widehat\lambda^j/j!]$.

Each last-column entry is $(O_j-E_j)^2/E_j$, and the Pearson statistic is $\boxed{X^2=\sum_{j\in\{0,1,2,3,4,\geq5\}}(O_j-E_j)^2/E_j}$. The displayed expected frequencies and contributions are rounded, so their printed values need not reproduce every final digit of a calculation using unrounded probabilities.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [O1](../../o1.md)
3. [O](../../../o.md)
4. [2004](../../../../2004-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
