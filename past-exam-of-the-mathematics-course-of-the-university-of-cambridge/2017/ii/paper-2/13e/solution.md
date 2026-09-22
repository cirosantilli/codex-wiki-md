<h1 id="13e/solution">Solution</h1>

↑ **Parent:** [13E](../13e.md)

Let $\mathbf r$ be position relative to the [center of mass](../../../../../center-of-mass.md), and let the new origin have vector $\mathbf c$ relative to it. The [inertia tensor](../../../../../inertia-tensor.md) about this origin is

$$
(I_{\mathbf c})_{ij}=\int\bigl(|\mathbf r-\mathbf c|^2\delta_{ij}-(r_i-c_i)(r_j-c_j)\bigr)\,dm.
$$

Expanding and using $\int\mathbf r\,dm=0$ proves the tensor form of the [parallel axis theorem](../../../../../parallel-axis-theorem.md):

$$
\boxed{I_{\mathbf c}=I_0+M\bigl(|\mathbf c|^2I-\mathbf c\mathbf c^T\bigr).}
$$

For a uniform cube of side $L$ and mass $M$, centered coordinate [integrals](../../../../../integral.md) give $I_0=(ML^2/6)I$. The displacement to a vertex is $(L/2,L/2,L/2)$ up to signs. Using axes along its incident edges gives

$$
\boxed{I_{\rm vertex}=ML^2\begin{pmatrix}2/3&-1/4&-1/4\\-1/4&2/3&-1/4\\-1/4&-1/4&2/3\end{pmatrix}.}
$$

The [principal moments of inertia](../../../../../principal-moment-of-inertia.md) are $\boxed{ML^2/6,\ 11ML^2/12,\ 11ML^2/12}$. The first [principal axis](../../../../../principal-axis.md) is the body diagonal through the vertex; every direction perpendicular to it has the repeated moment.

## ↑ Ancestors (10)

1. [13E](../13e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
