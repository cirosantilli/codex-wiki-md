<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume $EX>0$, as required by the denominators. Since each indicator has [variance](../../../../../variance-split.md) at most its expectation, and independent event pairs have zero [covariance](../../../../../covariance.md),

$$
\operatorname{Var}X=\sum_i\operatorname{Var}X_i+\sum_{i\ne j}\operatorname{Cov}(X_i,X_j)
\le EX+\sum_{i\sim j}P(A_i\cap A_j)=EX+D.
$$

The sum uses ordered pairs, [matching](../../../../../matching-graph-theory-split.md) the [covariance](../../../../../covariance.md) expansion. [Chebyshev's inequality](../../../../../chebyshev-s-inequality.md) now gives

$$
\boxed{P(X=0)\le\frac{\operatorname{Var}X}{(EX)^2}\le\frac1{EX}+\frac D{(EX)^2}}.
$$

If $EX=0$, $X=0$ almost surely and the divided expression is not the useful form of the bound.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
