<h1 id="11g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First, the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) applied to a face gives $|G|=20\cdot3=60$: its [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) consists of the identity and the two [rotations](../../../../../../rotation-mathematics.md) through $120^\circ$ about the axis through the centres of that face and its opposite. A [rotation](../../../../../../rotation-mathematics.md) preserving a face must preserve its outward normal and cyclically permute its three vertices, so there are no further stabilizing [rotations](../../../../../../rotation-mathematics.md).

The [conjugacy classes](../../../../../../conjugacy-class.md) are as follows:

- The identity: **size $1$**.
- Half-turns about axes through midpoints of opposite edges: **size $15$**.
- [Rotations](../../../../../../rotation-mathematics.md) through $\pm2\pi/3$ about opposite-face axes: **size $20$**.
- [Rotations](../../../../../../rotation-mathematics.md) through $\pm2\pi/5$ about opposite-vertex axes: **size $12$**.
- [Rotations](../../../../../../rotation-mathematics.md) through $\pm4\pi/5$ about opposite-vertex axes: **size $12$**.

There are $30/2=15$ edge axes, $20/2=10$ face axes, and $12/2=6$ vertex axes. They give respectively $15$, $2\cdot10=20$, and $4\cdot6=24$ distinct nonidentity [rotations](../../../../../../rotation-mathematics.md), already accounting for all $59$ nonidentity elements.

To justify the class assertions, conjugation by a [rotation](../../../../../../rotation-mathematics.md) carries the [rotation](../../../../../../rotation-mathematics.md) axis to its image and preserves the [rotation](../../../../../../rotation-mathematics.md) angle about the transported oriented axis. The [transitive group action](../../../../../../transitive-group-action.md) on edges puts all half-turns in one [conjugacy class](../../../../../../conjugacy-class.md). The [transitive group action](../../../../../../transitive-group-action.md) on faces puts the $120^\circ$ [rotations](../../../../../../rotation-mathematics.md) defined using outward face normals in one [conjugacy class](../../../../../../conjugacy-class.md); opposite faces encode opposite signs about the same unoriented axis. The same reasoning with outward vertex directions gives a class of twelve $72^\circ$ [rotations](../../../../../../rotation-mathematics.md) and a class of twelve $144^\circ$ [rotations](../../../../../../rotation-mathematics.md), including their inverses. These last classes cannot merge: the [matrix trace](../../../../../../matrix-trace.md) of a three-dimensional [rotation](../../../../../../rotation-mathematics.md) is $1+2\cos\theta$, which differs for $\theta=2\pi/5$ and $4\pi/5$. Thus the list is complete.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11G](../../11g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
