<h1 id="o/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $N_{ij}$ be the observed cell counts, $N_{i+}$ the row totals, $N_{+j}$ the column totals and $N=33009$. The fitted [expected frequencies](../../../../../expected-frequency.md) under [independence](../../../../../independent-random-variables.md) are $E_{ij}=N_{i+}N_{+j}/N$. For example the three-child, one-boy cell has expected count $7541\cdot16472/33009=3763.1$.

The [Pearson chi-squared statistic](../../../../../pearson-chi-squared-statistic.md) is

$$
\boxed{X^2=\sum_{i=1}^2\sum_{j=1}^3\frac{(N_{ij}-E_{ij})^2}{E_{ij}}.}
$$

Under $H_0$ it has asymptotically a [chi-squared distribution](../../../../../chi-squared-distribution.md) with $(2-1)(3-1)=2$ degrees of freedom, assuming the multinomial sampling model and sufficiently large expected counts. All expected counts here are large. The distribution is an asymptotic approximation, rather than an exact finite-sample identity.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [O](../../../o.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
