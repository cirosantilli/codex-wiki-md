<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose one grid-edge vector $a$ as the extrusion direction and an independent edge vector $b$. Label grid points $r_{i,j}=ia+jb$, so extruded height data have $z_{i,j}=g_j$, independent of $i$. The [Loop subdivision](../../../../../../loop-subdivision-surface.md) stencils are affine-exact in the $x,y$ coordinates, so the refined horizontal grid has spacing one-half and the same row structure.

At an old vertex, two neighbors lie in its own row, two in the row above and two in the row below. Its refined height is therefore

$$
g'_{2j}=\frac{10g_j+2g_j+2g_{j-1}+2g_{j+1}}{16}=\frac{g_{j-1}+6g_j+g_{j+1}}8.
$$

A new vertex on an edge parallel to $a$ has both endpoints in row $j$ and its opposite vertices in rows $j-1,j+1$, giving exactly the same value $g'_{2j}$. A new vertex on either of the other edge directions has endpoints in rows $j,j+1$; its two opposite vertices are also one in each of these rows. Its height is

$$
g'_{2j+1}=\frac{3(g_j+g_{j+1})+(g_j+g_{j+1})}{8}=\frac{g_j+g_{j+1}}2.
$$

Every refined vertex in a given row consequently has the same height. Induction proves this at every refinement level. The piecewise planar interpolating mesh is also constant along $a$ between rows, since adjacent rows have constant heights and form parallel straight lines. Taking its convergent limit preserves this invariance. Thus

$$
\boxed{z_\infty(r+\lambda a)=z_\infty(r)}
$$

where the points lie in the domain. The limit [subdivision surface](../../../../../../subdivision-surface.md) is an extrusion of the univariate limit curve. This is a statement about functional data on the regular grid, not about an arbitrary spatial mesh with extraordinary vertices or independently imposed boundary stencils.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
