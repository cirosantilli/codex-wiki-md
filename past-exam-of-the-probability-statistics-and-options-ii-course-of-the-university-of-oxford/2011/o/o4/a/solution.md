<h1 id="o/o4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Ignoring the multinomial coefficient, the likelihood is $L(\theta)=\prod_{i,j}\theta_{ij}^{n_{ij}}$. Maximize $\ell=\sum_{i,j}n_{ij}\log\theta_{ij}$ with $\sum\theta_{ij}=1$. A [Lagrange multiplier](../../../../../lagrange-multiplier.md) gives $n_{ij}/\theta_{ij}=\lambda$; summing the resulting $\theta_{ij}=n_{ij}/\lambda$ gives $\lambda=N$. Thus

$$
\boxed{\widehat\theta_{ij}=\frac{n_{ij}}N.}
$$

Because every count is positive, the [log-likelihood](../../../../../log-likelihood.md) is strictly concave on the interior simplex and this solution is its unique maximum.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [O4](../../o4.md)
3. [O](../../../o.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
