<h1 id="5a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Writing $X=\begin{pmatrix}x&y\\z&w\end{pmatrix}$ and using the [Frobenius inner product](../../../../../../frobenius-inner-product.md), the three [linear equations](../../../../../../linear-equation.md) are

$$
x+y+2z=0,\qquad x+y-2w=0,\qquad z+w=0.
$$

The first two differ by twice the third; equivalently $A-B=2C$. Thus there are only two independent constraints. Substituting $z=-w$ gives $y=2w-x$, so every element of the [vector subspace](../../../../../../vector-subspace.md) has the unique expression

$$
X=x\begin{pmatrix}1&-1\\0&0\end{pmatrix}
+w\begin{pmatrix}0&2\\-1&1\end{pmatrix}.
$$

The two coefficient [matrices](../../../../../../matrix.md) satisfy all three constraints. Their [linear independence](../../../../../../linear-independence.md) follows by looking first at entry $(1,1)$ and then at entry $(2,2)$. Therefore a [basis](../../../../../../basis.md) for this [orthogonal complement](../../../../../../orthogonal-complement.md) is

$$
\boxed{\left\{\begin{pmatrix}1&-1\\0&0\end{pmatrix},
\begin{pmatrix}0&2\\-1&1\end{pmatrix}\right\}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5A](../../5a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
