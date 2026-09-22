<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [nilpotent matrix](../../../../../../nilpotent-matrix.md) $T$, define the polynomial $E(z)=\sum_{k=0}^{m-1}z^kT^k/k!$. Because $T^m=0$, differentiating gives $E'(z)=TE(z)=E(z)T$. The derivative of the preserved [bilinear form](../../../../../../bilinear-form.md) matrix is therefore

$$
\frac{d}{dz}\bigl(E(z)^{\mathsf T}AE(z)\bigr)
=E(z)^{\mathsf T}(T^{\mathsf T}A+AT)E(z)=0.
$$

It is a constant matrix polynomial, equal to $A$ at $z=0$. Evaluation at one proves

$$
\boxed{(\exp T)^{\mathsf T}A\exp T=A.}
$$

Also $E(-1)$ is the inverse of $E(1)$ by the finite exponential product identity, so this really is an invertible isometry, even when $A$ is degenerate.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
