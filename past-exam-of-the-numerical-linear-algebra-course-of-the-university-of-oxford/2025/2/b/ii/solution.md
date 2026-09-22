<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [orthogonal projection](../../../../../orthogonal-projection.md) $P=QQ^T$ gives

$$
QM-A=Q(M-Q^TA)-(I_m-P)A.
$$

The first summand has every column in the [column space](../../../../../column-space.md) of $Q$, and the second has every column in its [orthogonal complement](../../../../../orthogonal-complement.md). They therefore have zero [Frobenius inner product](../../../../../frobenius-inner-product.md). The [Pythagorean identity](../../../../../pythagorean-theorem-in-an-inner-product-space.md), together with $Q^TQ=I_r$, gives the stronger exact formula

$$
\|QM-A\|_F^2=\|M-Q^TA\|_F^2+\|(I_m-P)A\|_F^2.
$$

Consequently

$$
\boxed{\|QQ^TA-A\|_F\leq\|QM-A\|_F},
$$

with equality exactly when $M=Q^TA$. Thus solving the [linear least-squares problem](../../../../../linear-least-squares-problem.md) for each column chooses the best coefficients in the prescribed [column space](../../../../../column-space.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
