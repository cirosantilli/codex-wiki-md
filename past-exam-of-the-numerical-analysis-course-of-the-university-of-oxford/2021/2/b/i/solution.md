<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Retain the first $r$ terms in the [singular value decomposition](../../../../../singular-value-decomposition.md):

$$
\boxed{A_r=\sum_{j=1}^r\sigma_ju_jv_j^T
=U\operatorname{diag}(\sigma_1,\ldots,\sigma_r,0,\ldots,0)V^T.}
$$

The [Eckart-Young-Mirsky theorem](../../../../../eckart-young-mirsky-theorem.md) says that this [truncated singular value decomposition](../../../../../truncated-singular-value-decomposition.md) is a best [low-rank approximation](../../../../../low-rank-approximation.md) in the [spectral norm](../../../../../matrix-2-norm.md). The remaining [singular values](../../../../../singular-value.md) of the difference are $\sigma_{r+1},\ldots,\sigma_n$, together with zeros, so

$$
\boxed{\|A-A_r\|_2=\sigma_{r+1}.}
$$

For $r\geq1$ the displayed [matrix](../../../../../matrix.md) has [matrix rank](../../../../../matrix-rank.md) exactly $r$, since every retained [singular value](../../../../../singular-value.md) is positive. For $r=0$, the only [matrix](../../../../../matrix.md) of [matrix rank](../../../../../matrix-rank.md) zero is the zero [matrix](../../../../../matrix.md), and the same formula gives error $\sigma_1$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
