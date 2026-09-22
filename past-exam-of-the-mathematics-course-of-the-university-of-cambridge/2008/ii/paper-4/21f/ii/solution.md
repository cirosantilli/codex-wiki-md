<h1 id="21f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take a [homotopy equivalence](../../../../../../homotopy-equivalence.md) $f:X\to Y$ with inverse $g$, and universal covering maps $p_X,p_Y$. Since the covering spaces are simply connected, the [path lifting theorem](../../../../../../path-lifting-theorem.md) constructs lifts $\widetilde f$ of $fp_X$ and $\widetilde g$ of $gp_Y$, after specifying one value in the appropriate fiber. Explicitly, define the lift at a point by lifting the image of a path from the chosen base point; [independence](../../../../../../independent-random-variables.md) from the path follows from simple connectedness and [homotopy](../../../../../../homotopy.md) lifting.

Lift a [homotopy](../../../../../../homotopy.md) $gf\simeq1_X$ starting at $\widetilde g\widetilde f$. The [homotopy lifting theorem for a covering map](../../../../../../homotopy-lifting-theorem-for-a-covering-map.md) makes its endpoint a map $d_X:\widetilde X\to\widetilde X$ with $p_Xd_X=p_X$. Such a lift of the identity is a [deck transformation](../../../../../../deck-transformation.md) and is a homeomorphism: lift the identity again with the base point image reversed, and uniqueness of path lifts makes the two compositions identities. Likewise $\widetilde f\widetilde g\simeq d_Y$ for a [deck transformation](../../../../../../deck-transformation.md) of $\widetilde Y$.

Thus both compositions are [homotopy](../../../../../../homotopy.md) equivalences, even though the lifted homotopies need not end at the particular identity lift. Part (i) then proves

$$
\boxed{X\simeq Y\quad\Longrightarrow\quad\widetilde X\simeq\widetilde Y.}
$$

Keeping the possible deck transformations is essential when the original homotopies do not fix base points.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [21F](../../21f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
