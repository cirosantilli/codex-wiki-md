<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

By the [spectral theorem](../../../../spectral-theorem.md), the [Hermitian matrix](../../../../hermitian-operator.md) $A$ has a complete [orthonormal eigenbasis](../../../../orthonormal-eigenbasis.md). If $Av=\lambda v$, idempotence gives $\lambda^2=\lambda$, so every [eigenvalue](../../../../eigenvalue.md) is zero or one. Since $\det A\ne1$, at least one is zero. Therefore

$$
\boxed{\det A=0,\qquad\operatorname{tr}A=m=\operatorname{rank}A\in\{0,1,\ldots,n-1\}.}
$$

The [trace of an idempotent equals its rank](../../../../trace-of-an-idempotent-equals-its-rank.md); here Hermiticity further identifies $A$ as an [orthogonal projection matrix](../../../../orthogonal-projection-matrix.md).

A complex [inner product](../../../../inner-product-split.md) $\langle u,v\rangle$ is conjugate-linear in its first argument, linear in its second, conjugate symmetric and positive definite: $\langle v,u\rangle=\overline{\langle u,v\rangle}$ and $\langle u,u\rangle>0$ for nonzero $u$. An [orthonormal basis](../../../../orthonormal-basis.md) is a spanning linearly independent family $e_i$ with $\langle e_i,e_j\rangle=\delta_{ij}$. The associated [norm](../../../../norm.md) is $\|u\|=\sqrt{\langle u,u\rangle}$.

For two distinct basis elements $x,y$, their [orthogonality](../../../../orthogonal-vectors.md) and unit norms give $\|x-y\|^2=\langle x,x\rangle+\langle y,y\rangle-\langle x,y\rangle-\langle y,x\rangle=2$. Hence **their distance is $\sqrt2$**; if the same element is selected twice, it is zero.

Finally, for $B^\dagger=B$, the scalar quadratic form obeys $(x^\dagger Bx)^*=x^\dagger B^\dagger x=x^\dagger Bx$, proving **$x^\dagger Bx$ is real**.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
