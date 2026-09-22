<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The supplied [subdivision mask](../../../../../../subdivision-mask.md) describes the regular, valence-six triangular grid. Its coefficients split into four parity classes after binary refinement: one class for old vertices and three classes for the three edge directions. For an old vertex $V$ with cyclic neighbors $V_1,\ldots,V_6$, the even stencil is

$$
\boxed{V'=\frac{10V+V_1+\cdots+V_6}{16}=\frac58V+\frac1{16}\sum_{r=1}^6V_r.}
$$

For an edge with endpoints $A,B$ and opposite vertices $C,D$ in its two incident [triangles](../../../../../../triangle.md), the new odd vertex is

$$
\boxed{M'=\frac{6A+6B+2C+2D}{16}=\frac38(A+B)+\frac18(C+D).}
$$

Rotating this edge stencil supplies the other two odd parity classes. All stencil weights sum to one, giving affine invariance; their first moments place an affine regular grid at the old positions and edge midpoints. Apply the same weights separately to $x,y,z$. Boundary edges and extraordinary vertices need additional rules, which are not specified by this uniform mask. The subsequent arguments concern the regular interior grid and compatible extruded boundary treatment.

## ↑ Ancestors (11)

1. [I](../i.md)
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
