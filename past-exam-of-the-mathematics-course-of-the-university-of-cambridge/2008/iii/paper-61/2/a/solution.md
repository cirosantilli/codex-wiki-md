<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

From $A^2=I$, induction gives $A^{2n}=I$ and $A^{2n+1}=A$. The [matrix exponential](../../../../../../matrix-exponential.md) converges absolutely in finite dimension, so its even and odd terms may be separated:

$$
e^{-i\theta A}
=\left[\sum_{n\geq0}\frac{(-1)^n\theta^{2n}}{(2n)!}\right]I
-i\left[\sum_{n\geq0}\frac{(-1)^n\theta^{2n+1}}{(2n+1)!}\right]A
=\boxed{\cos\theta\,I-i\sin\theta\,A}.
$$

This [involution exponential formula](../../../../../../involution-exponential-formula.md) requires no Hermiticity assumption on $A$. Hermiticity is needed if the exponential is additionally asserted to be unitary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
