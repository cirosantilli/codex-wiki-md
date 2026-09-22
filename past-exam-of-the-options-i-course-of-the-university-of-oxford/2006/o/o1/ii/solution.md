<h1 id="o/o1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fit the [Poisson distribution](../../../../../poisson-distribution.md) using the estimated daily mean. For $k=0,\ldots,8$, its expected frequency is

$$
E_k=N e^{-\widehat\mu}\frac{\widehat\mu^k}{k!},
$$

and $E_{\geq9}=N\left(1-\sum_{k=0}^8e^{-\widehat\mu}\widehat\mu^k/k!\right)$. Each row's contribution to the [Pearson chi-squared statistic](../../../../../pearson-chi-squared-statistic.md) is $(O_k-E_k)^2/E_k$. For example the zero-count class contributes $(162-126.784)^2/126.784\approx9.781$. Summing the class contributions gives the test statistic; expected frequencies depend on the fitted model, while observed frequencies come directly from counting days.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [O1](../../o1.md)
3. [O](../../../o.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
