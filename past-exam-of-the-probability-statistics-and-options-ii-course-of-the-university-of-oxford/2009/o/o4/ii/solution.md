<h1 id="o/o4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $D^*=D-A$. By (i), $D^*X=0$. Thus $D^*A^T=D^*X(X^TX)^{-1}=0$, and its transpose vanishes too. Expanding $DD^T=(D^*+A)(D^*+A)^T$ yields

$$
\boxed{\operatorname{Var}(\tilde\theta)=\sigma^2\left(D^*D^{*T}+(X^TX)^{-1}\right).}
$$

The [covariance](../../../../../covariance.md) difference is [positive semidefinite](../../../../../positive-semidefinite-matrix.md). In particular its $i$th diagonal entry is $\sigma^2\sum_j(D^*_{ij})^2\ge0$, proving the requested componentwise [variance](../../../../../variance-split.md) inequalities. Prefer $\boxed{\hat\theta_1}$ within the class of linear unbiased estimators, since it has the least [variance](../../../../../variance-split.md) and the same [expectation](../../../../../expected-value-split.md). A tie is possible if the first row of $D^*$ is zero. This is the [Gauss-Markov theorem](../../../../../gauss-markov-theorem.md) conclusion; no normal-distribution assumption on the errors is required.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [O4](../../o4.md)
3. [O](../../../o.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
