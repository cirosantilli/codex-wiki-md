<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Taking the adjoint of $U=M+iN$ gives $U^\dagger=M-iN$. In particular, the [Hermitian parts of a unitary matrix](../../../../../hermitian-parts-of-a-unitary-matrix.md) are uniquely determined:

$$
M=\frac{U+U^\dagger}{2},\qquad N=\frac{U-U^\dagger}{2i}.
$$

Expanding both unitary identities gives

$$
U^\dagger U=M^2+N^2+i(MN-NM)=I,\qquad UU^\dagger=M^2+N^2-i(MN-NM)=I.
$$

Subtracting shows $MN=NM$, and adding gives $M^2+N^2=I$. If $Mv=\mu v$, commutation implies $M(Nv)=\mu Nv$. The assumed simple spectrum makes the [eigenspace](../../../../../eigenspace.md) one-dimensional, so $Nv=\nu v$. Thus $M,N$ have a common [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md).

On such a [vector](../../../../../vector.md), $Uv=(\mu+i\nu)v$. If the corresponding unitary [eigenvalue](../../../../../eigenvalue.md) is $u=e^{i\theta}$, then

$$
\boxed{\mu=\operatorname{Re}u=\cos\theta,\qquad\nu=\operatorname{Im}u=\sin\theta.}
$$

The formulas for $M,N$ also show the same [eigenvalue](../../../../../eigenvalue.md) correspondence directly from $Uv=uv$ and $U^\dagger v=u^*v$. Degeneracies do not prevent existence of a common basis, although the simple-spectrum assumption makes the elementary proof immediate.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
