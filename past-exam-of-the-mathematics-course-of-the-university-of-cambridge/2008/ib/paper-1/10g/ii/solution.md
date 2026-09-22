<h1 id="10g/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $G=\operatorname{Rot}(D)$ for the [rotational symmetry group of a regular dodecahedron](../../../../../../rotational-symmetry-group-of-a-regular-dodecahedron.md). Centre the solid at the origin. A [rotation in three dimensions](../../../../../../rotation-in-three-dimensions.md) is determined by the image of a chosen face and one of its vertices, so there are at most $12\cdot5=60$ rotations. All these choices occur. The outward unit normal to a face and the direction from its centre to the chosen vertex determine an oriented orthonormal frame. The proper rotation mapping one such frame to another maps the whole regular pentagonal face. At each edge, the common dihedral angle and convexity then determine the adjacent face uniquely; propagating across the connected face-adjacency graph shows that the rotation maps the entire solid to itself. Hence $|G|=60$, and the action is transitive on faces, vertices and edges.

Its rotations can be counted geometrically. There are six axes joining opposite face centres, each allowing four nonidentity rotations of order five; ten axes joining opposite vertices, each allowing two of order three; and fifteen axes joining opposite edge midpoints, each allowing a half-turn. The [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) also verifies these possibilities: vertex stabilizers have order $60/20=3$ and edge stabilizers have order $60/30=2$, and their nonidentity elements rotate about the corresponding vertex or edge-midpoint axis. Together with the identity this accounts for all $1+24+20+15=60$ elements. In particular there are no elements of order four.

We now determine the [conjugacy classes](../../../../../../conjugacy-class.md). The group is transitive on edges, so all fifteen edge half-turns are conjugate. For a rotation whose angle is neither zero nor $\pi$, a commuting rotation must preserve its oriented axis: conjugation carries the axis and its rotation angle to their images, and reversing the axis would reverse a non-half-turn angle. Thus its [centralizer](../../../../../../centralizer.md) consists of rotations about the same axis. For a face rotation this [centralizer](../../../../../../centralizer.md) has order five, and for a vertex rotation it has order three. The [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) for conjugation therefore gives class sizes $60/5=12$ and $60/3=20$. The twenty vertex rotations form one class, and the twenty-four face rotations form two classes. **The class sizes are $1,15,20,12,12$.**

A [normal subgroup](../../../../../../normal-subgroup.md) is a union of these classes and contains the identity. Its possible orders are

$$
1,13,16,21,25,28,33,36,40,45,48,60.
$$

By [Lagrange's theorem](../../../../../../lagrange-s-theorem.md) its order must divide $60$. Only $1$ and $60$ in this list do so. Therefore $\boxed{G\text{ is simple of order }60}$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10G](../../10g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
