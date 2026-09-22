<h1 id="o/o5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The normal-error [log-likelihood](../../../../../log-likelihood.md), for fixed [variance](../../../../../variance-split.md), is a constant minus $\|Y-X\theta\|^2/(2\sigma^2)$. Differentiating the squared residual gives the normal equations $X^TX\widehat\theta=X^TY$. Since $X$ has full column rank, $X^TX$ is positive definite and the squared residual is strictly convex in $\theta$. Hence the unique minimizer, and thus the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md), is

$$
\boxed{\widehat\theta=(X^TX)^{-1}X^TY.}
$$

Profiling over the unknown positive [variance](../../../../../variance-split.md) does not change the residual-minimizing value of $\theta$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [O5](../../o5.md)
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
