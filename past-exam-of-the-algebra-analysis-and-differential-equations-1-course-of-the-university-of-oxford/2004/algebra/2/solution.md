<h1 id="algebra/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Self-adjointness](../../../../self-adjoint-operator.md) means $\langle Tv,w\rangle=\langle v,Tw\rangle$ for all $v,w\in V$, or $T=T^*$. Take the [inner product](../../../../inner-product-split.md) linear in its first variable. If $Tv=\lambda v$ with $v\ne0$, then

$$
\lambda\|v\|^2=\langle Tv,v\rangle=\langle v,Tv\rangle=\overline\lambda\|v\|^2.
$$

Therefore **every [eigenvalue](../../../../eigenvalue.md) is real**.

If $U$ is invariant and $w\in U^\perp$, then for every $u\in U$, $Tu\in U$ and $\langle Tw,u\rangle=\langle w,Tu\rangle=0$. Hence $Tw\in U^\perp$, proving invariance of the [orthogonal complement](../../../../orthogonal-complement.md).

Induct on $d=\dim V$. The zero-dimensional case is empty. For $d>0$, choose an [eigenvector](../../../../eigenvector.md) and normalize it to a unit vector $e$. Its span is invariant, so its [orthogonal complement](../../../../orthogonal-complement.md) is invariant as just proved. The restriction of $T$ to that complement is again [self-adjoint](../../../../self-adjoint-operator.md). Its [dimension](../../../../dimension-vector-space.md) is $d-1$, so [induction](../../../../mathematical-induction.md) supplies an [orthonormal basis](../../../../orthonormal-basis.md) of [eigenvectors](../../../../eigenvector.md) there. Adjoining $e$ gives **an orthonormal [eigenbasis](../../../../eigenbasis.md) of $V$**. This proves the [finite-dimensional spectral theorem](../../../../finite-dimensional-spectral-theorem.md) without assuming it in the argument.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Algebra](../../algebra.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
