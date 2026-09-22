<h1 id="19h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [extreme point](../../../../../../extreme-point.md) of a [convex set](../../../../../../convex-set.md) $C$ is a point $x\in C$ that cannot be written as $x=(1-t)y+tz$ with $y\ne z$ in $C$ and $0<t<1$.

Start with the eight vertices of the unit cube. The constraint $x_1+x_2+x_3\leq5/2$ removes $(1,1,1)$ and retains the other seven. The cutting plane meets the three cube edges incident to the removed vertex at

$$
A=(1/2,1,1),\qquad
B=(1,1/2,1),\qquad
C=(1,1,1/2).
$$

These are new vertices. No others occur: at a vertex in three dimensions, three linearly independent bounding planes are active, and choosing triples from the six cube faces and the cutting plane yields precisely the listed points. Hence the ten extreme points are

$$
\boxed{(0,0,0),(1,0,0),(0,1,0),(0,0,1),
(1,1,0),(1,0,1),(0,1,1),A,B,C}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19H](../../19h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
