# Cartesian basis under rotation

↑ **Parent:** [Cartesian basis](cartesian-basis.md)

Rotate the [standard basis](standard-basis.md) through $30^\circ$ using the [rotation matrix](rotation-matrix.md) whose columns are the new [basis vectors](basis-vector.md):

$$
u=\begin{pmatrix}\sqrt3/2\\1/2\end{pmatrix},\quad v=\begin{pmatrix}-1/2\\\sqrt3/2\end{pmatrix},\quad Q=[\,u\ v\,]=\begin{pmatrix}\sqrt3/2&-1/2\\1/2&\sqrt3/2\end{pmatrix},\quad \mathcal U=(u,v).
$$

Here $u\cdot v=0$ and $u\cdot u=v\cdot v=1$, so $Q$ is an [orthogonal matrix](orthogonal-matrix.md) with $Q^TQ=I$, where $T$ denotes [transpose](transpose.md) and $I$ is the [identity matrix](identity-matrix.md). For the same [vector](vector.md) $p=(2,1)^T$, its [coordinate vector](coordinate-vector.md) in this [Cartesian basis](cartesian-basis.md) is

$$
[p]_{\mathcal U}=Q^Tp=\begin{pmatrix}p\cdot u\\p\cdot v\end{pmatrix}=\begin{pmatrix}\sqrt3+1/2\\-1+\sqrt3/2\end{pmatrix}=\begin{pmatrix}\alpha\\\beta\end{pmatrix}.
$$

Thus $\alpha\approx2.232$ and $\beta\approx-0.134$: travel forwards along $u$ and a little backwards along $v$ to reconstruct $p=\alpha u+\beta v$. The [orthogonal projections](orthogonal-projection.md) onto the two axes give these signed [coordinates](coordinate-linear-algebra.md) because the measuring [vectors](vector.md) are both perpendicular and of unit length.

<a id="image-the-vector-p-2-1-t-reconstructed-from-its-orthogonal-projections-onto-a-rotated-cartesian-basis"></a>
![](cartesian-rotated-orthonormal-coordinates.png)

**[Figure 1](#image-the-vector-p-2-1-t-reconstructed-from-its-orthogonal-projections-onto-a-rotated-cartesian-basis). The vector $p=(2,1)^T$ reconstructed from its orthogonal projections onto a rotated Cartesian basis**.

The squared [norm](norm.md) remains

$$
\alpha^2+\beta^2=(\sqrt3+1/2)^2+(-1+\sqrt3/2)^2=(13/4+\sqrt3)+(7/4-\sqrt3)=5=2^2+1^2.
$$

This is useful when choosing axes aligned with a geometric feature: the [coordinates](coordinate-linear-algebra.md) change but distances and [dot products](dot-product.md) retain the same sum-of-products formula. The two directions of the [change of basis](change-of-basis.md) must be kept straight: $Q$ reconstructs the [vector](vector.md) in old [coordinates](coordinate-linear-algebra.md), $p=Q[p]_{\mathcal U}$, and $Q^T$ extracts its new [coordinates](coordinate-linear-algebra.md). Applying $Q$ to the old [coordinate vector](coordinate-vector.md) $p$ instead would actively rotate the [vector](vector.md).

A short proof explains both formulas. If $p=Qc$, multiplication by $Q^T$ gives $c=Q^Tp$. Then $\|p\|^2=c^TQ^TQc=c^Tc$. Perpendicular unit-length columns make the [matrix inverse](matrix-inverse-split.md) equal the [transpose](transpose.md); this is the computational convenience supplied by a [Cartesian basis](cartesian-basis.md).

## ↑ Ancestors (6)

1. [Cartesian basis](cartesian-basis.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
