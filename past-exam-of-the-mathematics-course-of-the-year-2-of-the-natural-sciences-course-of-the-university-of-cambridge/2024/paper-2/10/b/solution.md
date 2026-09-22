<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here $a^2=-I$, $a^3=-a$ and $a^4=I$, so $K$ is a [cyclic group of order four](../../../../../cyclic-group-of-order-four.md). Its [multiplication table](../../../../../multiplication-table.md) is

$$
\boxed{\begin{array}{c|rrrr}
\cdot&I&-I&a&-a\\\hline
I&I&-I&a&-a\\
-I&-I&I&-a&a\\
a&a&-a&-I&I\\
-a&-a&a&I&-I
\end{array}}
$$

Write the specified image of $a$ as $A$. Direct matrix multiplication gives

$$
A^2=-I_2,\qquad A^3=-A,\qquad A^4=I_2.
$$

A [group representation](../../../../../group-representation.md) is a [group homomorphism](../../../../../group-homomorphism.md) to a [general linear group](../../../../../general-linear-group.md), so the images of all powers of $a$ are forced:

$$
\boxed{\begin{aligned}
\Phi(I)&=\begin{pmatrix}1&0\\0&1\end{pmatrix},\\
\Phi(-I)&=\begin{pmatrix}-1&0\\0&-1\end{pmatrix},\\
\Phi(-a)&=\begin{pmatrix}0&-i\\-i&0\end{pmatrix}.
\end{aligned}}
$$

All four images are invertible. Defining $\Phi(a^j)=A^j$ is well-defined modulo four because $A^4=I_2$, and $A^{j+\ell}=A^jA^\ell$ verifies every product in the table. These observations prove both existence and uniqueness of this [representation](../../../../../group-representation.md) with the prescribed image.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
