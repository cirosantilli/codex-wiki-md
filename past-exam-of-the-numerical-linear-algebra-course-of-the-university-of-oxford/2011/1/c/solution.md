<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $u_j$ and $v_j$ be the columns of the [orthogonal matrices](../../../../orthogonal-matrix.md) $U$ and $V$ in the [singular value decomposition](../../../../singular-value-decomposition.md). Multiplying by the rectangular [diagonal matrix](../../../../diagonal-matrix.md) retains its $r$ nonzero diagonal entries:

$$
A=U\Sigma V^T=\boxed{\sum_{j=1}^r\sigma_j u_jv_j^T.}
$$

The families $(u_j)$ and $(v_j)$ are [orthonormal](../../../../orthonormal-set.md), hence in particular [orthogonal](../../../../orthogonal-vectors.md). Each summand is a rank-one [outer product](../../../../outer-product.md), and the remaining terms vanish because their [singular values](../../../../singular-value.md) are zero.

## ↑ Ancestors (12)

1. [C](../c.md)
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
