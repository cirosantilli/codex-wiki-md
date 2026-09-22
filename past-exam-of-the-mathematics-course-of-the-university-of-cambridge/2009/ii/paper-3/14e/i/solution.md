<h1 id="14e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $s=\sqrt b$. The two [fixed points](../../../../../../fixed-point.md) on the invariant line $x=0$ are $P_+=(0,s)$ and $P_-=(0,-s)$. There are also $Q_\pm=(\pm\sqrt{b-a^2/4},-a/2)$ when $a^2<4b$. At equality they coalesce with $P_-$.

The [Jacobian matrix](../../../../../../jacobian-matrix.md) is

$$
J(x,y)=\begin{pmatrix}-a-2y&-2x\\2x&2y\end{pmatrix}.
$$

At $P_+$ its [eigenvalues](../../../../../../eigenvalue.md) are $-a-2s$ and $2s$, so it is always a [saddle equilibrium](../../../../../../saddle-equilibrium.md). At $P_-$ they are $2s-a$ and $-2s$, so it is a [saddle equilibrium](../../../../../../saddle-equilibrium.md) for $a<2s$ and a [stable node](../../../../../../stable-node.md) for $a>2s$, with a zero [eigenvalue](../../../../../../eigenvalue.md) at $a=2s$.

At $Q_\pm$ the characteristic equation is $\lambda^2+a\lambda+4b-a^2=0$, giving

$$
\lambda=\frac{-a\pm\sqrt{5a^2-16b}}2.
$$

For $0<a^2<16b/5$ these points are [stable spirals](../../../../../../stable-spiral.md); for $16b/5<a^2<4b$ they are [stable nodes](../../../../../../stable-node.md). At $a^2=16b/5$ the double negative [eigenvalue](../../../../../../eigenvalue.md) has only one independent eigenvector, so these are improper [stable nodes](../../../../../../stable-node.md). When $a=0$ they are [center equilibria](../../../../../../center-equilibrium.md), as established in part (iii). Thus the collision at $\boxed{a^2=4b>0}$ changes both the number and stability of [fixed points](../../../../../../fixed-point.md); it is the [bifurcation](../../../../../../bifurcation.md) classified below.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [14E](../../14e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
