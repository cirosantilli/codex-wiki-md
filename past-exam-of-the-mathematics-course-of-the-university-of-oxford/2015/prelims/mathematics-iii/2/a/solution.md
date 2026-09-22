<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a [partial derivative](../../../../../../partial-derivative.md), the variable held fixed matters. Holding $u$ fixed gives $x_v=-v$. To find $v_y$, hold $x$ fixed and invert the [Jacobian matrix](../../../../../../jacobian-matrix.md):

$$
\begin{pmatrix}dx\\dy\end{pmatrix}=\begin{pmatrix}u&-v\\v&u\end{pmatrix}\begin{pmatrix}du\\dv\end{pmatrix},\qquad \begin{pmatrix}du\\dv\end{pmatrix}=\frac1{u^2+v^2}\begin{pmatrix}u&v\\-v&u\end{pmatrix}\begin{pmatrix}dx\\dy\end{pmatrix}.
$$

Thus

$$
\boxed{\left.\frac{\partial x}{\partial v}\right|_u=-v,\qquad \left.\frac{\partial v}{\partial y}\right|_x=\frac{u}{u^2+v^2}.}
$$

The second formula holds on each local inverse branch away from $(u,v)=(0,0)$, where the [Jacobian determinant](../../../../../../jacobian-determinant.md) vanishes. These are [planar parabolic coordinates](../../../../../../parabolic-polar-coordinates.md); the pairs $(u,v)$ and $(-u,-v)$ represent the same $(x,y)$, so no global choice of inverse is implicit.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
