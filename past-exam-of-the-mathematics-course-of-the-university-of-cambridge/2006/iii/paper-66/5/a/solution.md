<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The printed diagram is a propagation [subdivision mask](../../../../../../subdivision-mask.md): it shows the influence of one old vertex on several new vertices. Its entries do not all belong to a single averaging stencil. The old vertex is retained, and a new vertex is inserted at each incident face centre. Reading the contributions arriving at a target gives

$$
\boxed{V'=\tfrac12V+\tfrac18(V_1+V_2+V_3+V_4)},\qquad
\boxed{F'=\tfrac14(V_{00}+V_{10}+V_{01}+V_{11})}.
$$

Thus each new vertex-vertex averages its old value and its four edge neighbors, while each new face-vertex is the centroid of its four old corners. Both stencils are [convex combinations](../../../../../../convex-combination.md), reproduce constants and commute with [affine maps](../../../../../../affine-map.md). The neighboring $1/8$ contributions go to old vertices; the diagonal $2/8$ contributions go to face centres. The propagation coefficients sum to two because one refinement doubles the number of lattice vertices, not because either stencil fails to sum to one.

For calculations, describe this [quincunx subdivision](../../../../../../quincunx-subdivision.md) using

$$
D=\begin{pmatrix}1&1\\1&-1\end{pmatrix},\qquad D^2=2I.
$$

The refined square lattice is rotated by $45^\circ$ and its spacing is reduced by $\sqrt2$. In its integer coordinates, the one-step mask is

$$
a_{00}=\tfrac48,\qquad a_{\pm1,0}=a_{0,\pm1}=\tfrac28,\qquad a_{\pm1,\pm1}=\tfrac18.
$$

Indeed, a unit step in these new coordinates is an old face-centre displacement, whereas a diagonal step reaches an old edge neighbor. The even parity class contains the central and four diagonal coefficients and sums to one; the odd class contains the four axial coefficients and also sums to one. This checks the two target stencils independently.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
