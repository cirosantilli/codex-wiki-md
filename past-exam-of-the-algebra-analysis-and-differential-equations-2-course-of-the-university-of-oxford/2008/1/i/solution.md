<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Proceed by induction on $n=\dim V$. The zero-dimensional case is immediate. Over $\mathbb C$, the [fundamental theorem of algebra](../../../../fundamental-theorem-of-algebra.md) supplies a root $\lambda$ of the [characteristic polynomial](../../../../characteristic-polynomial.md). Since $\det(T-\lambda I)=0$, there is a nonzero vector $v_1$ with $Tv_1=\lambda v_1$. The line $W=\mathbb Cv_1$ is invariant, so $T$ induces a [linear map](../../../../linear-map.md) $\overline T$ on $V/W$. By induction, choose an upper triangular [basis](../../../../basis.md) for that quotient and lift its vectors to $v_2,\ldots,v_n$. Then $Tv_j\in\operatorname{span}(v_1,\ldots,v_j)$ for every $j$. Thus $v_1,\ldots,v_n$ is the required [basis](../../../../basis.md) and $\boxed{T\text{ is triangularizable}}$.

The same conclusion holds over $F$ when the [characteristic polynomial](../../../../characteristic-polynomial.md) splits over $F$. Indeed an [eigenvalue](../../../../eigenvalue.md) then lies in $F$, and the [block matrix](../../../../block-matrix.md) arising from the invariant line gives $\chi_T(X)=(X-\lambda)\chi_{\overline T}(X)$. The quotient [characteristic polynomial](../../../../characteristic-polynomial.md) therefore also splits, so the induction works over $F$ without requiring [algebraic closure](../../../../algebraic-closure.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [1](../../1.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
