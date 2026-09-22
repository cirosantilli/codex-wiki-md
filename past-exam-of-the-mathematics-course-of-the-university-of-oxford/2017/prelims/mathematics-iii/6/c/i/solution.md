<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $A_i=Y_{i-1}Y_i$, so $S_n=\sum_{i=1}^nA_i$. Each product has [mean](../../../../../../../expected-value-split.md) one, and its [variance](../../../../../../../variance-split.md) is

$$
\operatorname{Var}(A_i)=\mathbb E(Y_{i-1}^2)\mathbb E(Y_i^2)-1=2\cdot2-1=3.
$$

Adjacent products share one factor, giving [covariance](../../../../../../../covariance.md) one by part (a)(iii). Products whose indices differ by at least two involve disjoint [independent random variables](../../../../../../../independent-random-variables.md), so their [covariance](../../../../../../../covariance.md) is zero. There are $n-1$ adjacent pairs. By the [variance of a sum](../../../../../../../variance-of-a-sum.md),

$$
\boxed{\mathbb E S_n=n,\qquad\operatorname{Var}(S_n)=3n+2(n-1)=5n-2,\qquad n\ge1.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
