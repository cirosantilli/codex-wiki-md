<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the matrix's Euclidean [operator norm](../../../../operator-norm.md), [orthogonal invariance of the Euclidean norm](../../../../orthogonal-invariance-of-the-euclidean-norm.md) gives

$$
\|Ax\|_2=\|\Sigma V^Tx\|_2\leq\sigma_1\|x\|_2.
$$

Taking $x=v_1$ gives equality, so $\|A\|_2=\sigma_1$. For the [Frobenius norm](../../../../frobenius-norm.md), the [trace](../../../../matrix-trace.md) identity and the [singular value decomposition](../../../../singular-value-decomposition.md) give

$$
\|A\|_F^2=\operatorname{tr}(A^TA)=\operatorname{tr}(V\Sigma^T\Sigma V^T)=\sum_j\sigma_j^2.
$$

Consequently

$$
\boxed{\|A\|_2=\sigma_1,\qquad\|A\|_F=\left(\sum_{j=1}^r\sigma_j^2\right)^{1/2}.}
$$

Here the Euclidean matrix norm means the [operator norm](../../../../operator-norm.md) induced by the vector [Euclidean norm](../../../../euclidean-norm.md), rather than the entrywise Euclidean length, which is the [Frobenius norm](../../../../frobenius-norm.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the numerical linear algebra course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra course of the University of Oxford](../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
