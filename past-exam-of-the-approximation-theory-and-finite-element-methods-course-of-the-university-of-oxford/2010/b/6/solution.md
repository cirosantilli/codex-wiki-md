<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [bilinear square finite element](../../../../bilinear-square-finite-element.md) contains the terms $1,x,y,xy$. In anticlockwise corner order beginning at $(0,0)$, its [shape functions](../../../../shape-function.md) are

$$
N_1=(1-x/h)(1-y/h),\quad N_2=(x/h)(1-y/h),\quad
N_3=xy/h^2,\quad N_4=(1-x/h)(y/h).
$$

The [mass matrix](../../../../mass-matrix.md) has entries $M_{ij}=\int_0^h\int_0^hN_iN_j\,dx\,dy$. Each product separates into one-dimensional factors, with $\int_0^1(1-s)^2\,ds=\int_0^1s^2\,ds=1/3$ and $\int_0^1s(1-s)\,ds=1/6$. Diagonal, adjacent-corner and opposite-corner entries are respectively $h^2/9$, $h^2/18$, $h^2/36$. Thus

$$
\boxed{M_E=\frac{h^2}{36}\begin{pmatrix}4&2&1&2\\2&4&2&1\\1&2&4&2\\2&1&2&4\end{pmatrix}.}
$$

Number global grid nodes by $k=i+(n+1)j$, with $x_i=ih$, $y_j=jh$ and $0\leq i,j\leq n$. For an interior node, four elements contribute to its diagonal, two to each axial neighbour and one to each diagonal neighbour. Its global row therefore has the nine-point stencil

$$
\boxed{\frac{h^2}{36}\begin{pmatrix}1&4&1\\4&16&4\\1&4&1\end{pmatrix}.}
$$

In the stated ordering the axial entries occur at columns $k\pm1$ and $k\pm(n+1)$; the four diagonal ones occur at $k\pm(n+1)\pm1$. No boundary degrees of freedom have been removed.

For general valid quadrilaterals, use an [isoparametric finite element](../../../../isoparametric-finite-element.md). Map the unit square to an element by $F(\xi,\eta)=\sum_{i=1}^4\mathbf x_iN_i(\xi,\eta)$ and define physical [shape functions](../../../../shape-function.md) $N_i\circ F^{-1}$. Require a one-to-one nondegenerate map and compatible common edges. On a shared edge the map and the trace of each [shape function](../../../../shape-function.md) are linear between the same endpoints; the neighbouring traces therefore agree. The assembled functions are continuous and lie in $H^1$, giving a [conforming finite element space](../../../../conforming-finite-element-space.md). On a non-parallelogram the pulled-back functions are generally not bilinear polynomials in the physical coordinates themselves.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../split.md)
5. [Approximation theory and finite element methods course of the University of Oxford](../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
