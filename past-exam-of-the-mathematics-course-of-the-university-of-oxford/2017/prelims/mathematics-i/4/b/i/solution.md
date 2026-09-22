<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If $T^2=I$, every $v\in V$ has the decomposition

$$
v=\frac{v+Tv}{2}+\frac{v-Tv}{2},
$$

whose first term belongs to $E_1$ and second to $E_{-1}$. Their intersection is zero by [ii](../../a/ii.md), so $V=E_1\oplus E_{-1}$ is a [direct sum](../../../../../../../direct-sum.md). Choosing [bases](../../../../../../../basis.md) of the two [eigenspaces](../../../../../../../eigenspace.md) gives a diagonal [matrix](../../../../../../../matrix.md) with entries $1$ and $-1$.

Since $T^2\ne T$ while $T^2=I$, we have $T\ne I$. Thus $\dim E_{-1}$ is $1$, $2$, or $3$. Reordering the [basis](../../../../../../../basis.md) gives exactly

$$
\boxed{-I_3,\qquad\operatorname{diag}(1,1,-1),\qquad
\operatorname{diag}(1,-1,-1).}
$$

For $-I_3$, $T$ is **point inversion through the origin**. For $\operatorname{diag}(1,1,-1)$, it fixes the plane $E_1$ pointwise and reverses the complementary line $E_{-1}$: if $v=p+\ell$ in this [direct sum](../../../../../../../direct-sum.md), then $Tv=p-\ell$. For $\operatorname{diag}(1,-1,-1)$, it fixes the line $E_1$ pointwise and reverses the complementary plane $E_{-1}$.

These are instances of [oblique symmetry of complementary subspaces](../../../../../../../oblique-symmetry-of-complementary-subspaces.md), allowing oblique [eigenspaces](../../../../../../../eigenspace.md). They are a Euclidean [reflection in a hyperplane](../../../../../../../reflection-in-a-hyperplane.md) and a [rotation in three dimensions](../../../../../../../rotation-in-three-dimensions.md) through $\pi$ about a line, respectively, when the two [eigenspaces](../../../../../../../eigenspace.md) are perpendicular. The hypotheses do not require an [orthogonal transformation](../../../../../../../orthogonal-transformation.md) or an [orthonormal basis](../../../../../../../orthonormal-basis.md), so that additional metric property cannot be inferred just from the displayed diagonal forms.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
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
