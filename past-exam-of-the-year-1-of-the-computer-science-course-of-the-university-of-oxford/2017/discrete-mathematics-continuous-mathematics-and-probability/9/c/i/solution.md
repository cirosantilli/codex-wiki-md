<h1 id="9/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $Z_i=Y_{i-1}Y_i$ for $1\leq i\leq n$. Independence of the underlying exponentials gives $\mathbb EZ_i=1$ and

$$
\operatorname{Var}(Z_i)=\mathbb E[Y_{i-1}^2]\mathbb E[Y_i^2]-1=4-1=3.
$$

By the [covariance of overlapping independent products](../../../../../../covariance-of-overlapping-independent-products.md), adjacent terms have covariance one. Terms separated by at least two indices use disjoint independent factors, so their covariance is zero. There are $n-1$ adjacent pairs. [Linearity of expectation](../../../../../../linearity-of-expectation.md) and the [variance of a sum](../../../../../../variance-of-a-sum.md) formula therefore yield

$$
\boxed{\mathbb ES_n=n,\qquad\operatorname{Var}(S_n)=3n+2(n-1)=5n-2,\qquad n\geq1.}
$$

In particular, the products themselves are not independent merely because the original $Y_i$ are.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
