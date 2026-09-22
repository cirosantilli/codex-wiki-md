<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\Delta=v_1\cdot(v_2\times v_3)\ne0$, since the original vectors form a [basis](../../../../basis.md). The [reciprocal basis](../../../../reciprocal-basis.md) is

$$
\boxed{u^1=\frac{v_2\times v_3}{\Delta},\qquad
u^2=\frac{v_3\times v_1}{\Delta},\qquad
u^3=\frac{v_1\times v_2}{\Delta}.}
$$

Taking the [dot product](../../../../dot-product.md) with each $v_j$ gives $u^i\cdot v_j=\delta_{ij}$, using orthogonality of a [cross product](../../../../cross-product.md) and cyclic symmetry of the [scalar triple product](../../../../scalar-triple-product.md). If $\sum_i a_i u^i=0$, taking its [dot product](../../../../dot-product.md) with $v_j$ yields $a_j=0$. The three reciprocal vectors are therefore [linearly independent](../../../../linear-independence.md) and form a [basis](../../../../basis.md) of $\mathbb R^3$.

Equivalently, if $V$ has columns $v_j$ and $U$ columns $u^i$, then $U^TV=I$, so $U=V^{-T}$. In particular any vector has coordinates $r=\sum_i(r\cdot u^i)v_i$, even when the original basis is not orthonormal.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
