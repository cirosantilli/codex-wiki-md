<h1 id="9c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $R_\theta$ be rotation about the third axis, so invariance means $R_\theta T R_\theta^T=T$. At $\theta=\pi$, its diagonal signs are $(-1,-1,1)$; each mixed entry $T_{13},T_{23},T_{31},T_{32}$ changes sign and must vanish.

For the remaining planar block $M=\begin{pmatrix}p&q\\r&s\end{pmatrix}$, the quarter-turn $J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ gives

$$
JMJ^T=\begin{pmatrix}s&-r\\-q&p\end{pmatrix}=M.
$$

Hence $s=p$ and $r=-q$. Writing the constants as $\alpha,\omega,\beta$ gives

$$
\boxed{T=\begin{pmatrix}\alpha&\omega&0\\-\omega&\alpha&0\\0&0&\beta\end{pmatrix}.}
$$

Conversely, $M=\alpha I-\omega J$ commutes with every planar rotation, so every displayed matrix is invariant under every rotation about the axis. This is an [oriented-axis invariant Cartesian tensor](../../../../../../oriented-axis-invariant-cartesian-tensor.md). Symmetry was not assumed, so the antisymmetric parameter $\omega$ need not vanish.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9C](../../9c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
