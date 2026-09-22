<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

All the transformations below fix the origin. A [planar rotation](../../../../../planar-rotation.md) preserves lengths and angles and turns every vector through one common oriented angle. Its [rotation matrix](../../../../../rotation-matrix.md) is

$$
R_\theta=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}.
$$

An [orthogonal reflection](../../../../../reflection-in-a-hyperplane.md) in a line fixes that line and reverses its perpendicular direction; reflection in the horizontal axis has [reflection matrix](../../../../../reflection-matrix.md) $\operatorname{diag}(1,-1)$. A [uniform dilation](../../../../../uniform-dilation.md) multiplies every vector by the same positive scale $s$, represented by $sI$; for example $2I$ doubles lengths. A [shear mapping](../../../../../shear-mapping.md) fixes one line pointwise and shifts vectors parallel to that line by an amount proportional to their transverse coordinate. A horizontal [shear mapping](../../../../../shear-mapping.md) has matrix

$$
S_k=\begin{pmatrix}1&k\\0&1\end{pmatrix},\qquad (x,y)\longmapsto(x+ky,y),
$$

with $S_1$ a nontrivial example.

The first given matrix is **the clockwise [planar rotation](../../../../../planar-rotation.md) through $\pi/4$**, namely $A=R_{-\pi/4}$. Direct multiplication gives

$$
\boxed{C=AB=\begin{pmatrix}1&2\\0&1\end{pmatrix}=S_2.}
$$

Thus **$C$ is a horizontal [shear mapping](../../../../../shear-mapping.md) of strength $2$**. Because $A^{-1}=R_{\pi/4}$,

$$
\boxed{B=R_{\pi/4}S_2.}
$$

So **$B$ is the composition of that [shear mapping](../../../../../shear-mapping.md) followed by an anticlockwise [planar rotation](../../../../../planar-rotation.md) through $\pi/4$**; order matters. It is not individually one of the four elementary types under these definitions. In particular, its [determinant](../../../../../determinant.md) is $1$, but it is not an [orthogonal matrix](../../../../../orthogonal-matrix.md), excluding both a [planar rotation](../../../../../planar-rotation.md) and an [orthogonal reflection](../../../../../reflection-in-a-hyperplane.md). It is not a scalar matrix, excluding a [uniform dilation](../../../../../uniform-dilation.md); its [eigenvalues](../../../../../eigenvalue.md) $\sqrt2+1$ and $\sqrt2-1$ exclude a pure [shear mapping](../../../../../shear-mapping.md), whose [eigenvalues](../../../../../eigenvalue.md) are both $1$. As a symmetric [positive-definite matrix](../../../../../positive-definite-matrix.md), $B$ can also be described as stretching two perpendicular principal directions by these reciprocal factors, preserving area.

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
