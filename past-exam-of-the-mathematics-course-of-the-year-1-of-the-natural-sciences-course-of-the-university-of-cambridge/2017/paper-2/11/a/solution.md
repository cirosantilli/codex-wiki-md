<h1 id="11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Expand the [vector triple product](../../../../../vector-triple-product.md) in Cartesian components. Its first component is

$$
\begin{aligned}
[\mathbf a\times(\mathbf b\times\mathbf c)]_x
&=a_y(b_xc_y-b_yc_x)-a_z(b_zc_x-b_xc_z)\\
&=b_x(a_yc_y+a_zc_z)-c_x(a_yb_y+a_zb_z)\\
&=b_x(\mathbf a\cdot\mathbf c)-c_x(\mathbf a\cdot\mathbf b),
\end{aligned}
$$

where adding $a_xb_xc_x$ to both products introduces cancelling terms. Likewise the other two components are

$$
\begin{aligned}
[\mathbf a\times(\mathbf b\times\mathbf c)]_y
&=a_z(b_yc_z-b_zc_y)-a_x(b_xc_y-b_yc_x)
=b_y(\mathbf a\cdot\mathbf c)-c_y(\mathbf a\cdot\mathbf b),\\
[\mathbf a\times(\mathbf b\times\mathbf c)]_z
&=a_x(b_zc_x-b_xc_z)-a_y(b_yc_z-b_zc_y)
=b_z(\mathbf a\cdot\mathbf c)-c_z(\mathbf a\cdot\mathbf b).
\end{aligned}
$$

Together these prove

$$
\boxed{\mathbf a\times(\mathbf b\times\mathbf c)
=(\mathbf a\cdot\mathbf c)\mathbf b-(\mathbf a\cdot\mathbf b)\mathbf c}.
$$

Now use the cyclic property of the [scalar triple product](../../../../../scalar-triple-product.md) and the just-proved identity:

$$
\begin{aligned}
(\mathbf a\times\mathbf b)\cdot(\mathbf c\times\mathbf d)
&=\mathbf a\cdot[\mathbf b\times(\mathbf c\times\mathbf d)]\\
&=\mathbf a\cdot[(\mathbf b\cdot\mathbf d)\mathbf c-(\mathbf b\cdot\mathbf c)\mathbf d].
\end{aligned}
$$

This proves [Lagrange's identity](../../../../../lagrange-identity-for-the-cross-product.md) in the requested form,

$$
\boxed{(\mathbf a\times\mathbf b)\cdot(\mathbf c\times\mathbf d)
=(\mathbf a\cdot\mathbf c)(\mathbf b\cdot\mathbf d)
-(\mathbf a\cdot\mathbf d)(\mathbf b\cdot\mathbf c)}.
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [11](../../11.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
