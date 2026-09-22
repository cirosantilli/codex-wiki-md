<h1 id="6a/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define

$$
P(A)=(-1)^{n-1}A^{n-1}
-c_{n-1}A^{n-2}-\cdots-c_2A-c_1I.
$$

The [Cayley-Hamilton theorem](../../../../../../cayley-hamilton-theorem.md) for

$$
\chi_A(z)=(-1)^nz^n+c_{n-1}z^{n-1}
+\cdots+c_1z+c_0
$$

gives

$$
AP(A)=P(A)A=c_0I=\det(A)I.
$$

If $A$ is nonsingular, multiplication by $A^{-1}$ shows $P(A)=\det(A)A^{-1}=\operatorname{adj}(A)$.

For arbitrary $A$, apply the nonsingular result to $A-tI$ for a sequence of nonzero $t\to0$ avoiding the finitely many singular values. Both the characteristic coefficients and the adjugate entries depend polynomially on the matrix entries, so the limit gives

$$
\boxed{
\operatorname{adj}(A)
=(-1)^{n-1}A^{n-1}
-c_{n-1}A^{n-2}-\cdots-c_2A-c_1I}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6A](../../6a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
