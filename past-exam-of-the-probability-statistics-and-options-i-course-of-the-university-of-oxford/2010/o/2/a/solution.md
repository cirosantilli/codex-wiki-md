<h1 id="o/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The full column rank makes $X^{\mathsf T}X$ invertible. The [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md) from minimizing squared residuals give

$$
\boxed{\widehat\theta=(X^{\mathsf T}X)^{-1}X^{\mathsf T}Y.}
$$

The errors have [covariance matrix](../../../../../covariance-matrix.md) $\sigma^2I_n$ by [independence](../../../../../independent-random-variables.md) and equal [variance](../../../../../variance-split.md). Applying the [covariance](../../../../../covariance.md) transformation rule to this linear estimator yields

$$
\operatorname{Var}(\widehat\theta)
=(X^{\mathsf T}X)^{-1}X^{\mathsf T}(\sigma^2I)X(X^{\mathsf T}X)^{-1}
=\boxed{\sigma^2(X^{\mathsf T}X)^{-1}.}
$$

The parameter estimator is unbiased because $\mathbb EY=X\theta$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
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
