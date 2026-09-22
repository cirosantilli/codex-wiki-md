<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The first three output components equal $x_1,x_2,x_3$, while the fourth is $x_4-\sum_{k=1}^4x_k=-x_1-x_2-x_3$. Hence

$$
\boxed{P=\begin{pmatrix}1&0&0&0\\0&1&0&0\\0&0&1&0\\-1&-1&-1&0\end{pmatrix}.}
$$

Its outputs have component sum zero, and applying $P$ to any such output leaves it fixed. Thus

$$
\boxed{P^2=P,\qquad\det P=0,\qquad\operatorname{tr}P=3.}
$$

The first three columns give a [basis](../../../../../basis.md) of the [image of a linear map](../../../../../image-of-a-linear-map.md):

$$
v_1=(1,0,0,-1)^T,\quad v_2=(0,1,0,-1)^T,\quad v_3=(0,0,1,-1)^T.
$$

They are [linearly independent](../../../../../linear-independence.md) because their first three coordinates are the standard [basis](../../../../../basis.md). Their [span](../../../../../linear-span.md) is precisely the three-dimensional hyperplane $y_1+y_2+y_3+y_4=0$.

Apply the [Gram-Schmidt process](../../../../../gram-schmidt-process.md). First $q_1=v_1/\sqrt2$. Subtracting the $q_1$ projection from $v_2$ gives $(-1,2,0,-1)^T/2$, of length $\sqrt{3/2}$. Subtracting both preceding projections from $v_3$ gives $(-1,-1,3,-1)^T/3$, of length $2/\sqrt3$. Therefore an [orthonormal basis](../../../../../orthonormal-basis.md) is

$$
\boxed{q_1=\frac{(1,0,0,-1)^T}{\sqrt2},\qquad q_2=\frac{(-1,2,0,-1)^T}{\sqrt6},\qquad q_3=\frac{(-1,-1,3,-1)^T}{\sqrt{12}}.}
$$

Their pairwise [dot products](../../../../../dot-product.md) vanish and each has length one. Although this image admits an [orthonormal basis](../../../../../orthonormal-basis.md), $P$ itself is an [oblique projection](../../../../../oblique-projection.md): its [kernel](../../../../../kernel-of-a-linear-map-split.md) is the fourth coordinate axis, which is not perpendicular to the image, and $P\ne P^T$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
