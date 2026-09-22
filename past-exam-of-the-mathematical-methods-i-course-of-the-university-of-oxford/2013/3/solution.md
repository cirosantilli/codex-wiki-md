<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write all [vectors](../../../vector.md) in Cartesian components. The first component of the nested [cross product](../../../cross-product.md) is

$$
\begin{aligned}
[\mathbf a\times(\mathbf b\times\mathbf c)]_x
&=a_y(b_xc_y-b_yc_x)-a_z(b_zc_x-b_xc_z)\\
&=b_x(a_yc_y+a_zc_z)-c_x(a_yb_y+a_zb_z)\\
&=b_x(\mathbf a\cdot\mathbf c)-c_x(\mathbf a\cdot\mathbf b).
\end{aligned}
$$

The missing $a_x$ terms cancel as $-b_xa_xc_x+c_xa_xb_x=0$. Computing the $y$ and $z$ components by cyclic permutation gives the same form, proving the [vector triple product identity](../../../vector-triple-product.md)

$$
\boxed{\mathbf a\times(\mathbf b\times\mathbf c)
=(\mathbf a\cdot\mathbf c)\mathbf b-(\mathbf a\cdot\mathbf b)\mathbf c.}
$$

Apply this expression to the three cyclic terms. Their sum is

$$
(\mathbf a\cdot\mathbf c)\mathbf b-(\mathbf a\cdot\mathbf b)\mathbf c
+(\mathbf b\cdot\mathbf a)\mathbf c-(\mathbf b\cdot\mathbf c)\mathbf a
+(\mathbf c\cdot\mathbf b)\mathbf a-(\mathbf c\cdot\mathbf a)\mathbf b=0.
$$

Each coefficient cancels because the [dot product](../../../dot-product.md) is symmetric. This is the [Jacobi identity](../../../jacobi-identity.md) for the [cross product](../../../cross-product.md).

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2013](../../2013-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
