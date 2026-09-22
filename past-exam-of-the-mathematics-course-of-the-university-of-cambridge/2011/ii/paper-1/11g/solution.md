<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

Identify the [Möbius group](../../../../../mobius-group.md) with $\operatorname{PSL}_2(\mathbb C)$, the orientation-preserving [isometry group](../../../../../isometry-group.md) of three-dimensional [hyperbolic space](../../../../../hyperbolic-space.md). Here a [properly discontinuous group action](../../../../../properly-discontinuous-group-action.md) permits finite stabilizers: for each compact set $K$, only finitely many $g$ satisfy $gK\cap K\ne\varnothing$.

Fix $o\in\mathbb H^3$. The set of isometries with $d(o,go)\leq R$ is compact. To see this, an orientation-preserving isometry is uniquely determined by the image of an oriented orthonormal frame at $o$. The image point lies in a compact closed hyperbolic ball and its frame lies in a compact rotation-group fiber. These choices parametrize the indicated set of isometries continuously.

A [discrete subgroup](../../../../../discrete-subgroup.md) of a [topological group](../../../../../topological-group-split.md) is closed: otherwise distinct subgroup elements accumulating at the same point would have quotients tending to the identity, contradicting isolation of the identity. Its intersection with a compact set is therefore finite. If $K\subseteq B(o,R)$ and $gK\cap K\ne\varnothing$, choosing $x,gx\in K$ gives $d(o,go)\leq d(o,gx)+d(gx,go)\leq2R$. Hence discreteness implies a [properly discontinuous group action](../../../../../properly-discontinuous-group-action.md). Conversely, if the subgroup is not discrete, distinct $g_n$ tend to the identity. For a compact ball $K$ with $o$ in its interior, eventually $g_no\in K$, so infinitely many $g_nK$ meet $K$, contradicting proper discontinuity. This proves the equivalence.

Matrices of determinant one over the [Gaussian integers](../../../../../gaussian-integer.md) are closed under multiplication and inversion, with inverse $\left(\begin{smallmatrix}d&-b\\-c&a\end{smallmatrix}\right)$. Quotienting by $\{\pm I\}$ gives the specified group of [Möbius transformations](../../../../../mobius-transformation.md). The Gaussian integers form a [discrete set](../../../../../discrete-subset.md) in the complex plane, so these matrices form a [discrete subgroup](../../../../../discrete-subgroup.md) of $\operatorname{SL}_2(\mathbb C)$, and the finite quotient remains discrete. Thus this group acts properly discontinuously on $\mathbb H^3$.

Explicit representatives of all four types are

$$
\boxed{
\begin{array}{c|c|c}
\text{type}&\text{matrix}&\text{trace}\\\hline
\text{elliptic}&\begin{pmatrix}0&-1\\1&0\end{pmatrix}&0\\
\text{parabolic}&\begin{pmatrix}1&1\\0&1\end{pmatrix}&2\\
\text{hyperbolic}&\begin{pmatrix}2&1\\1&1\end{pmatrix}&3\\
\text{loxodromic}&\begin{pmatrix}1+i&1\\i&1\end{pmatrix}&2+i
\end{array}}
$$

The first is $z\mapsto-1/z$ and has order two; the second is the nonidentity translation $z\mapsto z+1$. The third has positive real reciprocal [eigenvalues](../../../../../eigenvalue.md) $(3\pm\sqrt5)/2$, giving translation along an axis without rotation. For the last, a nonreal trace excludes both unit-modulus and real eigenvalues. Its multiplier therefore has modulus different from one and a nonzero rotation angle: it is a [loxodromic Möbius transformation](../../../../../loxodromic-mobius-transformation.md).

## ↑ Ancestors (11)

1. [11G](../11g.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
