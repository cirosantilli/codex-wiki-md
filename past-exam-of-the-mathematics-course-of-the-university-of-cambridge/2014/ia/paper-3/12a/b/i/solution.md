<h1 id="12a/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Under a proper [rotation matrix](../../../../../../../rotation-matrix.md) $R$, invariance of a [Cartesian second-rank tensor](../../../../../../../cartesian-second-rank-tensor.md) reads $T=RTR^T$, equivalently $TR=RT$. The half-turn $R_z(\pi)=\operatorname{diag}(-1,-1,1)$ forces all entries mixing the $z$ direction with the $xy$ plane to vanish. Thus $T$ consists of a planar $2\times2$ block $B$ and the entry $T_{33}=c$.

Commutation with the planar quarter-turn $J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ gives $B=aI+bJ$. This block already commutes with every planar rotation. Now use the half-turn $R_x(\pi)=\operatorname{diag}(1,-1,-1)$: on the planar block its conjugation fixes $I$ and sends $J$ to $-J$, so invariance forces $b=0$. Therefore

$$
\boxed{T=\operatorname{diag}(a,a,c),\qquad
t_{ij}=\alpha\delta_{ij}+\beta\delta_{i3}\delta_{j3},\quad
\alpha=a,\ \beta=c-a.}
$$

The formula uses the [Kronecker delta](../../../../../../../kronecker-delta.md) and is sufficient as well as necessary: rotations preserving the unoriented $z$-axis fix both $I$ and $e_3e_3^T$. This is an [axially invariant second-rank tensor](../../../../../../../axially-invariant-second-rank-tensor.md) with the planar antisymmetric part removed by the horizontal half-turn.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [12A](../../../12a.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ia](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
