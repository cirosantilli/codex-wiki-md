<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md) identifies the sum of the $k$th powers of the [eigenvalues](../../../../../eigenvalue.md) with the [trace](../../../../../matrix-trace.md) of the $k$th [matrix](../../../../../matrix.md) power. Therefore the [moment](../../../../../moment.md) of the [empirical spectral measure](../../../../../empirical-spectral-measure.md) is

$$
\boxed{m_k(n)=n^{-1-k/2}\operatorname{tr}(M^k)
=n^{-1-k/2}\sum_{i_1,\ldots,i_k=1}^n
M_{i_1i_2}M_{i_2i_3}\cdots M_{i_ki_1}.}
$$

For odd $k$, every summand has zero [expectation](../../../../../expected-value-split.md) by part (a)(ii), so $\boxed{\mathbb E[m_k(n)]=0}$ for every $n$.

For the second [moment](../../../../../moment.md), use $M_{ji}=M_{ij}$. There are $n$ diagonal entries with [variance](../../../../../variance-split.md) two and $n(n-1)$ ordered off-diagonal entries with [variance](../../../../../variance-split.md) one. Their [means](../../../../../expected-value-split.md) vanish, giving

$$
\mathbb E[m_2(n)]
=n^{-2}\sum_{i,j}\mathbb E[M_{ij}^2]
=\frac{2n+n(n-1)}{n^2}
=1+\frac1n.
$$

Hence $\boxed{\lim_{n\to\infty}\mathbb E[m_2(n)]=1}$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
