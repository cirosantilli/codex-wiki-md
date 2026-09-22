<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose a complement $W$ to the fixed $k$-dimensional [vector subspace](../../../../../../vector-subspace.md) $U$. With column [vectors](../../../../../../vector.md) and the decomposition $V=U\oplus W$, its [parabolic stabilizer of a subspace](../../../../../../parabolic-stabilizer-of-a-subspace.md) is

$$
P_k=\left\{\begin{pmatrix}A&B\\0&D\end{pmatrix}:
A\in GL_k(q),\ D\in GL_{n-k}(q),\
B\in\operatorname{Hom}(W,U)\right\}.
$$

The arbitrary upper-right block forms a normal [elementary abelian group](../../../../../../elementary-abelian-group.md). The block-diagonal [matrices](../../../../../../matrix.md) form a complement, acting on it by $B\mapsto ABD^{-1}$. Thus

$$
\boxed{P_k\cong \operatorname{Hom}(W,U)\rtimes
(GL_k(q)\times GL_{n-k}(q)),\qquad
|P_k|=q^{k(n-k)}|GL_k(q)||GL_{n-k}(q)|.}
$$

With row [vectors](../../../../../../vector.md) the off-diagonal block is transposed; the [subgroup](../../../../../../subgroup.md) description is the same after the convention change.

The [rank of a transitive permutation group](../../../../../../rank-of-a-transitive-permutation-group.md) is the number of orbits of a [stabilizer subgroup](../../../../../../stabilizer-subgroup.md), not the rank of a [matrix](../../../../../../matrix.md). For $Y\in X_k$, the invariant of its $P_k$-orbit is $r=\dim(U\cap Y)$. This invariant is complete. Choose a [basis](../../../../../../basis.md) of $U\cap Y$, extend it to a [basis](../../../../../../basis.md) of $U$, then add a [basis](../../../../../../basis.md) of a complement of $U\cap Y$ in $Y$, and extend the resulting independent [vectors](../../../../../../vector.md) to a [basis](../../../../../../basis.md) of $V$. For $Y'$ with the same intersection [dimension](../../../../../../dimension-vector-space.md) $r$, do the same. The map between these adapted [bases](../../../../../../basis.md) preserves $U$ and sends $Y$ to $Y'$.

Each value $r=0,1,\ldots,k$ occurs: in a [basis](../../../../../../basis.md) $e_1,\ldots,e_n$ with $U=\langle e_1,\ldots,e_k\rangle$, take

$$
Y_r=\langle e_1,\ldots,e_r,e_{k+1},\ldots,e_{2k-r}\rangle.
$$

The hypothesis $2k\le n$ guarantees all these [vectors](../../../../../../vector.md) exist. Hence

$$
\boxed{\operatorname{rank}(GL_n(q)\curvearrowright X_k)=k+1.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
