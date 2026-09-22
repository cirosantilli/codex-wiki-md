<h1 id="8/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [quadratic form of a squared cross product](../../../../../quadratic-form-of-a-squared-cross-product.md), express the two scalar terms as [quadratic forms](../../../../../quadratic-form-split.md) in $\mathbf a$:

$$
\boxed{M=|\mathbf b|^2I-\mathbf b\mathbf b^T,\qquad
M_{ij}=|\mathbf b|^2\delta_{ij}-b_ib_j.}
$$

Then $\mathbf a^TM\mathbf a=|\mathbf b|^2|\mathbf a|^2-(\mathbf a\cdot\mathbf b)^2$. In particular, for $\mathbf b=(b_1,b_2,0)$,

$$
M=\begin{pmatrix}b_2^2&-b_1b_2&0\\-b_1b_2&b_1^2&0\\0&0&b_1^2+b_2^2\end{pmatrix},\qquad\boxed{\det M=0.}
$$

The cancellation is structural: $M\mathbf b=0$, while its action on every vector perpendicular to a nonzero $\mathbf b$ is multiplication by $|\mathbf b|^2$. Its [eigenvalues](../../../../../eigenvalue.md) are therefore $0,|\mathbf b|^2,|\mathbf b|^2$; for $\mathbf b=0$ the whole matrix is zero.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [2017 resit](../../../../2017-resit-split.md)
5. [Past exam of the mathematical methods I course of the University of Oxford](../../../../split.md)
6. [Mathematical methods I course of the University of Oxford](../../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
