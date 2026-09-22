<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In an [orthonormal basis](../../../../orthonormal-basis.md), every [vector](../../../../vector.md) $w$ has the coordinate expansion $w=\sum_i\langle w,e_i\rangle e_i$. If $\langle Su,v\rangle=\langle u,Rv\rangle$ for all $u,v$, apply it to $u=e_i$, $v=e_j$ and take complex conjugates:

$$
\langle Re_j,e_i\rangle=\langle e_j,Se_i\rangle.
$$

Consequently

$$
\boxed{Re_j=\sum_{i=1}^n\langle e_j,Se_i\rangle e_i.}
$$

Conversely, this formula gives

$$
\langle e_i,Re_j\rangle=\overline{\langle e_j,Se_i\rangle}=\langle Se_i,e_j\rangle.
$$

Linearity in the first argument and conjugate-linearity in the second extend the equality from [basis](../../../../basis.md) [vectors](../../../../vector.md) to all $u,v$. This proves the equivalence.

The displayed formula specifies exactly one image for each [basis](../../../../basis.md) [vector](../../../../vector.md), so it defines a unique [linear transformation](../../../../linear-map.md) $S^*$ and proves the existence and uniqueness of the [adjoint on an inner product space](../../../../adjoint-on-an-inner-product-space.md).

Conjugate symmetry gives

$$
\langle S^*u,v\rangle
=\overline{\langle v,S^*u\rangle}
=\overline{\langle Sv,u\rangle}
=\langle u,Sv\rangle.
$$

By uniqueness of the [adjoint operator](../../../../adjoint-operator.md), $\boxed{(S^*)^*=S}$. Also

$$
\langle STu,v\rangle=\langle Tu,S^*v\rangle
=\langle u,T^*S^*v\rangle,
$$

so uniqueness gives $\boxed{(ST)^*=T^*S^*}$. The reversal of order follows directly from moving the two factors across the [inner product](../../../../inner-product-split.md) one at a time.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
