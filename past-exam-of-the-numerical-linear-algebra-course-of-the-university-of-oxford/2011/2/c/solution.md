<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $A=D+L+R$, where $D$ is the [diagonal matrix](../../../../diagonal-matrix.md) of diagonal entries of $A$, and $L,R$ are its strictly lower- and upper-triangular parts. Since $A$ is [symmetric](../../../../symmetric-relation.md), $R=L^T$. Subtract the two factors in the [SOR](../../../../successive-over-relaxation.md) iteration:

$$
(D+\omega L)-[(1-\omega)D-\omega R]=\omega A.
$$

Therefore, for $\omega\ne0$,

$$
C(\omega)=I-\omega(D+\omega L)^{-1}A
=\boxed{I-B(\omega)^{-1}A,\qquad B(\omega)=\omega^{-1}D+L.}
$$

[Positive definiteness](../../../../positive-definiteness.md) makes each $D_{ii}>0$, so the [triangular matrix](../../../../triangular-matrix.md) $B(\omega)$ is an [invertible matrix](../../../../invertible-matrix.md) for every $\omega\ne0$. The original formula gives $C(0)=I$; the expression for $B(\omega)$ itself is undefined there. The affine term ensuring that the desired solution is a [fixed point](../../../../fixed-point.md) is $c=B(\omega)^{-1}b$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the numerical linear algebra course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra course of the University of Oxford](../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
