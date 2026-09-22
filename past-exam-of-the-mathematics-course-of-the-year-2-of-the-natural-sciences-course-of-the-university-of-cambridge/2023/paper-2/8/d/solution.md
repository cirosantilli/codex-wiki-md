<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write a matrix in the set as $M(a,b)$. The zero matrix $M(0,0)$ has no multiplicative [inverse matrix](../../../../../matrix-inverse-split.md), so $S$ is **not a group**. Its [determinant](../../../../../determinant.md) is

$$
\det M(a,b)=|a|^2+|b|^2,
$$

which vanishes only at that zero matrix. It is therefore the only element that needs to be removed.

For closure, direct [matrix multiplication](../../../../../matrix-multiplication.md) gives

$$
M(a,b)M(c,d)=M(ac-bd^*,\ ad+bc^*).
$$

The product of nonzero determinants is nonzero, so two nonzero elements never multiply to zero. The [identity matrix](../../../../../identity-matrix.md) is $M(1,0)$, [associativity](../../../../../associative-property.md) is inherited from matrix multiplication, and

$$
\boxed{M(a,b)^{-1}=\frac1{|a|^2+|b|^2}\begin{pmatrix}a^*&-b\\b^*&a\end{pmatrix}
=M\left(\frac{a^*}{|a|^2+|b|^2},\frac{-b}{|a|^2+|b|^2}\right).}
$$

Thus $\boxed{S\setminus\{0_{2\times2}\}\text{ is a group}}$. It is the multiplicative group of nonzero [quaternions](../../../../../quaternion.md) in the [complex matrix representation of quaternions](../../../../../complex-matrix-representation-of-quaternions.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [8](../../8.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
