<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [transportation simplex algorithm](../../../../../../transportation-simplex-algorithm.md), with [transportation dual potentials](../../../../../../transportation-dual-potentials.md) $u_i,v_j$ and [reduced costs](../../../../../../reduced-cost.md) $r_{ij}=c_{ij}-u_i-v_j$. On a basic cell choose $u_i+v_j=c_{ij}$. The initial shipment matrix, read from the circled entries in the PDF, is

$$
X^{(0)}=\begin{pmatrix}0&7&5\\5&0&0\\0&7&0\\4&0&8\end{pmatrix},\qquad \operatorname{cost}(X^{(0)})=155.
$$

Its six positive cells form a [transportation spanning tree](../../../../../../transportation-spanning-tree.md). Setting $u_1=0$ gives

$$
u=(0,-8,-4,-3),\qquad v=(11,4,8),\qquad R^{(0)}=\begin{pmatrix}-6&0&0\\0&11&2\\2&0&-1\\0&9&0\end{pmatrix}.
$$

Enter cell $(1,1)$, whose [reduced cost](../../../../../../reduced-cost.md) is $-6$. The [cycle pivot](../../../../../../cycle-pivot.md) has signs

$$
(1,1)^+\to(1,3)^-\to(4,3)^+\to(4,1)^-\to(1,1).
$$

The maximum feasible increment is $\theta=\min(5,4)=4$, so cell $(4,1)$ leaves the basis. The result is

$$
X^{(1)}=\begin{pmatrix}4&7&1\\5&0&0\\0&7&0\\0&0&12\end{pmatrix},\qquad \operatorname{cost}(X^{(1)})=155-6\cdot4=131.
$$

For the new [transportation spanning tree](../../../../../../transportation-spanning-tree.md),

$$
u=(0,-2,-4,-3),\qquad v=(5,4,8),\qquad R^{(1)}=\begin{pmatrix}0&0&0\\0&5&-4\\8&0&-1\\6&9&0\end{pmatrix}.
$$

Enter cell $(2,3)$ with [reduced cost](../../../../../../reduced-cost.md) $-4$. Its [cycle pivot](../../../../../../cycle-pivot.md) is

$$
(2,3)^+\to(2,1)^-\to(1,1)^+\to(1,3)^-\to(2,3).
$$

Now $\theta=\min(5,1)=1$, and cell $(1,3)$ leaves. We obtain

$$
\boxed{X^*=\begin{pmatrix}5&7&0\\4&0&1\\0&7&0\\0&0&12\end{pmatrix},\qquad \operatorname{cost}(X^*)=127.}
$$

Its row sums are $(12,5,7,12)$ and its column sums $(9,14,13)$, as required. The final [transportation dual potentials](../../../../../../transportation-dual-potentials.md) are

$$
u=(0,-2,-4,1),\qquad v=(5,4,4),\qquad R^*=\begin{pmatrix}0&0&4\\0&5&0\\8&0&3\\2&5&0\end{pmatrix}.
$$

All reduced costs are nonnegative, proving optimality. More explicitly, for any feasible shipment matrix $X$,

$$
\sum_{i,j}c_{ij}x_{ij}\geq\sum_i u_i\,\operatorname{supply}_i+\sum_jv_j\,\operatorname{demand}_j=-10-28+12+45+56+52=127.
$$

Our shipments use only zero-reduced-cost cells and attain this lower bound. This supplies an independent [weak duality](../../../../../../weak-duality.md) certificate for the transportation optimum.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
