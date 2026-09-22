<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [singular value decomposition](../../../../singular-value-decomposition.md) $A=U\Sigma V^T$ gives

$$
A^TA=V\Sigma^2V^T.
$$

Therefore $\boxed{\sigma_i(A)=\sqrt{\lambda_i(A^TA)}}$, counting multiplicities. These are the nonnegative square roots: zero singular values must be included if $A$ is singular. Strict positivity requires full rank, which the question does not assume.

Write the lower [bidiagonal matrix](../../../../bidiagonal-matrix.md) entries as $B_{ii}=d_i$ and $B_{i+1,i}=e_i$. Its columns $i$ and $j$ have disjoint supports if $|i-j|>1$, so $T=B^TB$ has no entries outside the three central diagonals. More explicitly,

$$
\boxed{T_{ii}=d_i^2+e_i^2\ (i<n),\quad T_{nn}=d_n^2,\quad T_{i,i+1}=T_{i+1,i}=e_id_{i+1}.}
$$

This proves both symmetry and the [tridiagonal matrix](../../../../tridiagonal-matrix.md) structure.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the numerical linear algebra and approximation course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and approximation course of the University of Oxford](../../../../numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
