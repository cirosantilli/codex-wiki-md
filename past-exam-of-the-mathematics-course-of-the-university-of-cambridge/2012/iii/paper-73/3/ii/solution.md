<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $C(r)=\langle\mathbf u(\mathbf x)\cdot\mathbf u(\mathbf x+\mathbf r)\rangle$ in zero-mean [isotropic turbulence](../../../../../../isotropic-turbulence.md). Define the scalar [Saffman integral](../../../../../../saffman-integral.md) $L=\int_{\mathbb R^3}C(r)\,d^3r=4\pi\int_0^\infty r^2C(r)\,dr$. The spectral transform is

$$
E(k)=\frac1\pi\int_0^\infty C(r)kr\sin(kr)\,dr.
$$

For an integrable $r^2C(r)$, dominated convergence applied to $\sin(kr)/(kr)$ gives

$$
\boxed{E(k)=\frac{L}{4\pi^2}k^2+o(k^2)}\quad(k\to0).
$$

A further $O(k^4)$ expansion requires an additional correlation [moment](../../../../../../moment.md) and is not automatic from finite $L$. The normalization agrees with $\int E\,dk=\langle|\mathbf u|^2\rangle/2$.

For a control volume $V$ put $\mathbf P_V=\int_V\mathbf u\,dV$. [Statistical homogeneity](../../../../../../statistical-homogeneity.md) gives the exact finite-volume identity

$$
\langle|\mathbf P_V|^2\rangle
=\int_V\int_V C(\mathbf y-\mathbf x)\,d^3x\,d^3y
=\int_{\mathbb R^3}C(\mathbf r)|V\cap(V-\mathbf r)|\,d^3r.
$$

For geometrically similar volumes increasing without bound, the overlap fraction $|V\cap(V-\mathbf r)|/|V|$ tends to one at every fixed separation. If $C$ is absolutely integrable, dominated convergence gives

$$
\boxed{L=\lim_{|V|\to\infty}\frac{\langle|\mathbf P_V|^2\rangle}{|V|}}.
$$

The printed finite-large-volume expression is the corresponding asymptotic approximation, not an exact identity for an arbitrary finite volume. For instance, positive nonzero $C$ with a finite correlation length gives an overlap fraction smaller than one and hence a strictly smaller finite-volume value. The limit also shows $L\ge0$; a nonzero [Saffman integral](../../../../../../saffman-integral.md) is positive.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
