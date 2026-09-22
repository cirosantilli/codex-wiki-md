<h1 id="1d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the cube with vertices $(\pm1,\pm1,\pm1)$, and choose the edge $E=\{(1,1,z):-1\leq z\leq1\}$. Here the [symmetry group of a cube](../../../../../../symmetry-group-of-a-cube.md) consists of all rigid symmetries, including reflections. A symmetry fixes the centre and permutes the three pairs of opposite faces, so its matrix is a [signed permutation matrix](../../../../../../signed-permutation-matrix.md).

A symmetry in the [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) of $E$ must preserve its midpoint $(1,1,0)$ and send its direction $(0,0,1)$ to itself or its negative. In this [cube symmetry action on edges](../../../../../../cube-symmetry-action-on-edges.md), its only choices are to interchange the first two coordinates and to reverse the third coordinate. Thus the [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) consists of

$$
(x,y,z)\mapsto(x,y,z),\quad(y,x,z),\quad(x,y,-z),\quad(y,x,-z).
$$

The two generating reflections commute and have order two, so this [subgroup](../../../../../../subgroup.md) is a [Klein four-group](../../../../../../klein-four-group.md), isomorphic to $C_2\times C_2$ and has order four. Permuting coordinates and changing signs carries $E$ to any edge. Its [orbit of a group action](../../../../../../orbit-of-a-group-action.md) is therefore the set of all twelve edges. The [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) gives

$$
\boxed{|G|=12\cdot4=48.}
$$

If one restricts to orientation-preserving symmetries, only two of the four stabilizer elements remain, giving the [rotational symmetry group of a cube](../../../../../../rotational-symmetry-group-of-a-cube.md) of order $24$; the full symmetry [group](../../../../../../group-split.md) asked for here has order $48$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1D](../../1d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
