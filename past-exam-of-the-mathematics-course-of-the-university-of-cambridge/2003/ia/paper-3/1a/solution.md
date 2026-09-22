<h1 id="1a/solution">Solution</h1>

↑ **Parent:** [1A](../1a.md)

Use the standard ordered [basis](../../../../../basis.md) $(\mathbf e_1,\mathbf e_2,\mathbf e_3)$ for both maps. The [reflection in a hyperplane](../../../../../reflection-in-a-hyperplane.md) interchanges the second and third coordinates, so its [matrix](../../../../../matrix.md) is

$$
\boxed{A=\begin{pmatrix}1&0&0\\0&0&1\\0&1&0\end{pmatrix}}.
$$

Orient the rotation axis along $\mathbf n=(1,1,1)/\sqrt3$ and use the right-hand convention. The [rotation matrix](../../../../../rotation-matrix.md) for angle $2\pi/3$ sends $\mathbf e_1$ to $\mathbf e_2$, $\mathbf e_2$ to $\mathbf e_3$, and $\mathbf e_3$ to $\mathbf e_1$. For example, the [Rodrigues rotation formula](../../../../../rodrigues-rotation-formula.md) gives

$$
R\mathbf e_1=\cos\frac{2\pi}{3}\,\mathbf e_1+\sin\frac{2\pi}{3}(\mathbf n\times\mathbf e_1)+\left(1-\cos\frac{2\pi}{3}\right)(\mathbf n\cdot\mathbf e_1)\mathbf n=\mathbf e_2.
$$

Multiplying the [rotation matrix](../../../../../rotation-matrix.md) by the dilation factor gives

$$
\boxed{B=2R=\begin{pmatrix}0&0&2\\2&0&0\\0&2&0\end{pmatrix}}.
$$

Direct multiplication gives $A^2=I$, $B^2=4\begin{pmatrix}0&1&0\\0&0&1\\1&0&0\end{pmatrix}$ and $B^3=8I$. Hence **$B^3=8A^2$**. If the opposite axis orientation is chosen, $B=2R^T$ also has cube $8I$. Independently of coordinates, two applications of the [reflection](../../../../../reflection-mathematics.md) give the identity, while three applications of the rotation-dilation give a full turn and dilation by $2^3$. Every [basis](../../../../../basis.md) represents these resulting maps by $I$ and $8I$. Thus the equality even holds when the two [matrices](../../../../../matrix.md) are expressed in different [bases](../../../../../basis.md).

## ↑ Ancestors (10)

1. [1A](../1a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
