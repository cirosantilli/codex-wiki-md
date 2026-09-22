<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [cyclic group](../../../../../cyclic-group.md) of order $p$ contains an element of order two if and only if $2$ divides $p$. Necessity follows from [Lagrange's theorem](../../../../../lagrange-s-theorem.md); for even $p$, the unique such element is $c=g_1^{p/2}$. Hence

$$
\boxed{p\text{ is even},\qquad C=\{I,g_1^{p/2}\}.}
$$

Because $g_1$ has order $p>2$ and the representation is faithful, $D(g_1)$ cannot be a reflection, which has order two. It is therefore a rotation through a primitive angle $\vartheta=2\pi q/p$, with $\gcd(q,p)=1$. The condition on the greatest common divisor is exactly what makes its order $p$ rather than a proper divisor. Since $p$ is even, $q$ is odd, so $D(c)$ is the half-turn:

$$
\boxed{D(c)=-I_2,\qquad D(g_i)=\begin{pmatrix}\cos(i\vartheta)&-\sin(i\vartheta)\\\sin(i\vartheta)&\cos(i\vartheta)\end{pmatrix},\quad\vartheta=\frac{2\pi q}{p},\quad\gcd(q,p)=1.}
$$

The [character](../../../../../character-of-a-representation.md) is the trace:

$$
\boxed{\chi(g_i)=2\cos\frac{2\pi qi}{p},\qquad\chi(I)=2.}
$$

Choosing the primitive generator with $q=1$ gives the customary rotation representation. The general coprime value is included because faithfulness alone does not select that generator. These are the two-dimensional cases in the [irreducible real representations of a finite cyclic group](../../../../../irreducible-real-representations-of-a-finite-cyclic-group.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
