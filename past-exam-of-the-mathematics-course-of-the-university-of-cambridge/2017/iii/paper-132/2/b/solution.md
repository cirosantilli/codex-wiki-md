<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The analogous flat-coordinate construction does not define a full $\mathrm{SL}_2(\mathbb R)$ action on arbitrary cubic differentials.** Away from zeros, a nonzero [holomorphic cubic differential](../../../../../../holomorphic-cubic-differential.md) has [flat coordinates](../../../../../../natural-coordinate-of-a-holomorphic-differential.md)

$$
w=\int c^{1/3},\qquad c=dw^3.
$$

Their changes of coordinate are $w_j=\zeta w_i+b_{ij}$ with $\zeta^3=1$. A branch change is therefore a rotation through $2\pi/3$, not merely a sign. Applying a real-linear map $A$ changes its linear part to $ARA^{-1}$, where $R$ is that rotation. In general this is not a [complex-linear map](../../../../../../complex-linear-map.md), so the proposed changes of coordinate are not [holomorphic](../../../../../../complex-differentiability-at-a-point.md) and cannot define the required deformed [complex structure](../../../../../../complex-structure.md).

For example, take $A=\operatorname{diag}(2,1/2)$ and $R=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}$ with $\theta=2\pi/3$. Then

$$
ARA^{-1}=
\begin{pmatrix}\cos\theta&-4\sin\theta\\\frac14\sin\theta&\cos\theta\end{pmatrix},
$$

whose off-diagonal entries fail the condition for a [complex-linear map](../../../../../../complex-linear-map.md). This dependence on the choice of cube-root coordinate is the obstruction even when considering descent from the locus $c=\omega^3$: the three possible roots need not lead to the same deformation of the cubic pair.

The real matrices preserving [orientation](../../../../../../orientation-of-a-simplex.md) that normalize the order-three rotations are precisely the matrices of [complex-linear maps](../../../../../../complex-linear-map.md); intersecting with $\mathrm{SL}_2(\mathbb R)$ leaves $\mathrm{SO}(2)$. Indeed a nonreal rotation determines its [complex structure](../../../../../../complex-structure.md), and conjugation to its inverse would reverse that structure's [orientation](../../../../../../orientation-of-a-simplex.md). Thus there is a natural rotation action,

$$
\boxed{R_\theta\cdot(X,c)=(X,e^{3i\theta}c).}
$$

The conclusion concerns the geometric [group action](../../../../../../group-action.md) analogous to that for [translation surfaces](../../../../../../translation-surface.md) and [half-translation surfaces](../../../../../../half-translation-surface.md); it does not rule out artificial group actions unrelated to these atlases.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
