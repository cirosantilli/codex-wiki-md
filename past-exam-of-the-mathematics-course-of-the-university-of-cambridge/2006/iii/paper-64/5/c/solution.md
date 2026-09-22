<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The space of real $2\times2$ [matrices](../../../../../../matrix.md) has a [determinant](../../../../../../determinant.md) form of signature $(2,2)$: write

$$
X=\begin{pmatrix}u+x&y+v\\y-v&u-x\end{pmatrix},
\qquad \det X=u^2+v^2-x^2-y^2.
$$

The action $(A,B):X\mapsto AXB^{-1}$ of $SL(2,\mathbb R)\times SL(2,\mathbb R)$ preserves this [determinant](../../../../../../determinant.md). Each factor is connected by [polar decomposition of an invertible real matrix](../../../../../../polar-decomposition-of-an-invertible-real-matrix.md): its orthogonal factor lies in connected $SO(2)$ and its positive factor is an exponential of a symmetric [traceless matrix](../../../../../../traceless-matrix.md). Thus the image is contained in $SO_0(2,2)$.

If the action is trivial, $X=I$ gives $A=B$, and fixing every $X$ makes $A$ a scalar [matrix](../../../../../../matrix.md). [Determinant](../../../../../../determinant.md) one gives $A=B=\pm I$. The kernel is therefore the diagonal $\mathbb Z_2$. Its discreteness makes the differential injective; domain and target both have dimension six. An open subgroup of connected $SO_0(2,2)$ is the whole group, so

$$
\boxed{SO_0(2,2)\cong\bigl(SL(2,\mathbb R)\times SL(2,\mathbb R)\bigr)/\mathbb Z_2.}
$$

Again the kernel is diagonal, and the target is the [identity component](../../../../../../identity-component.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
