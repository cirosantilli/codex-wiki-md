<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $X\in\operatorname{SO}_3(\mathbb R)$, the defining identity $X^TX=I$ gives

$$
\|Xv\|^2=v^TX^TXv=v^Tv=\|v\|^2.
$$

Thus an [orthogonal transformation](../../../../../../../orthogonal-transformation.md) preserves the [Euclidean norm](../../../../../../../euclidean-norm.md) and sends the [unit sphere](../../../../../../../unit-sphere.md) to itself. Restricting the given [group action](../../../../../../../group-action-split.md) to this invariant set preserves both action axioms.

If $XN=N$, the first column of $X$ is $N=e_1$. The other columns are [unit vectors](../../../../../../../unit-vector.md) perpendicular to it, so the first row is also $(1,0,0)$. Hence $X=\operatorname{diag}(1,B)$ with $B^TB=I_2$ and $\det B=1$. Conversely, every such [matrix](../../../../../../../matrix.md) lies in $G$ and fixes $N$. Since every element of the [special orthogonal group in two dimensions](../../../../../../../special-orthogonal-group-in-two-dimensions.md) has the planar [rotation matrix](../../../../../../../rotation-matrix.md) form, the [stabilizer subgroup](../../../../../../../stabilizer-subgroup.md) is

$$
\boxed{H=\left\{R_\theta=
\begin{pmatrix}
1&0&0\\
0&\cos\theta&-\sin\theta\\
0&\sin\theta&\cos\theta
\end{pmatrix}:\theta\in\mathbb R\right\}\cong\operatorname{SO}_2(\mathbb R).}
$$

Geometrically these are exactly the [rotations in three dimensions](../../../../../../../rotation-in-three-dimensions.md) about the first coordinate axis.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
