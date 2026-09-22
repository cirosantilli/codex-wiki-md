<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Since both real [matrices](../../../../../matrix.md) are antisymmetric, $A^\dagger=-A$ and $B^\dagger=-B$. Thus $U^\dagger=-A+iB$. Expand the two unitary identities:

$$
UU^\dagger=-A^2-B^2+i(AB-BA)=I,\qquad U^\dagger U=-A^2-B^2-i(AB-BA)=I.
$$

Subtracting and adding give $\boxed{AB=BA,\qquad A^2+B^2=-I}$. Because $A$ has simple [eigenvalues](../../../../../eigenvalue.md), each of its complex [eigenspaces](../../../../../eigenspace.md) is one-dimensional. Commutation makes each one invariant under $B$: if $Av=av$, then $A(Bv)=a(Bv)$. Hence $Bv=bv$ for some scalar $b$. The complete [eigenbasis](../../../../../eigenbasis.md) of $A$ is therefore a common [eigenbasis](../../../../../eigenbasis.md), which also diagonalizes $U$.

The [skew-Hermitian decomposition of a unitary matrix](../../../../../skew-hermitian-decomposition-of-a-unitary-matrix.md) is explicit:

$$
A=\frac{U-U^\dagger}{2},\qquad B=\frac{U+U^\dagger}{2i}.
$$

If $Uv=uv$, unitarity gives $U^\dagger v=u^{-1}v=\overline u\,v$. Consequently

$$
\boxed{a=\frac{u-\overline u}{2}=i\operatorname{Im}u,\qquad b=\frac{u+\overline u}{2i}=-i\operatorname{Re}u.}
$$

Equivalently, for $u=e^{i\theta}$ the paired [eigenvalues](../../../../../eigenvalue.md) are $\boxed{a=i\sin\theta,\ b=-i\cos\theta}$. The hypotheses can only occur in even dimension: $U^T=-U$ and $U$ is invertible, whereas an odd-dimensional [skew-symmetric matrix](../../../../../skew-symmetric-matrix.md) has zero [determinant](../../../../../determinant.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
