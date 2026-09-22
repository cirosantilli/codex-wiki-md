<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $S=A+B$ and $E(t)=F(t)-e^{tS}$. Since $F(0)=I$, $E(0)=0$. Differentiate the ordered exponential products, using that each [matrix](../../../../../../matrix.md) commutes with its own exponential:

$$
F'(t)-SF(t)
=\frac12\left\{[e^{tB},A]e^{tA}+[e^{tA},B]e^{tB}\right\}
=:D(t).
$$

Here the [commutator](../../../../../../commutator.md) convention is $[X,Y]=XY-YX$; this fixes both signs. The error satisfies $E'=SE+D$, so the [variation-of-constants formula](../../../../../../variation-of-constants-formula.md) gives

$$
\boxed{E(t)=\frac12\int_0^t e^{(t-x)S}
\left\{[e^{xB},A]e^{xA}+[e^{xA},B]e^{xB}\right\}\,dx.}
$$

This is the [symmetrized exponential-splitting defect identity](../../../../../../symmetrized-exponential-splitting-defect-identity.md). Symmetry of $A,B$ was not needed for the identity itself; it will be used to bound their exponentials in part (c).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
