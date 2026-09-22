<h1 id="14e/solution">Solution</h1>

↑ **Parent:** [14E](../14e.md)

Let $b=f(0)$ and $g(x)=f(x)-b$. Distance preservation and polarization give $\langle g(x),g(y)\rangle=\langle x,y\rangle$. The vectors $g(e_1),g(e_2),g(e_3)$ form an orthonormal [basis](../../../../../basis.md), and $\langle g(x),g(e_i)\rangle=x_i$. Hence $g(x)=\sum_i x_i g(e_i)=Qx$ for an orthogonal [matrix](../../../../../matrix.md) $Q$. Every [Euclidean isometry](../../../../../euclidean-isometry.md) is therefore $f(x)=Qx+b$.

To decompose $Q$, if $Qe_1\ne e_1$ reflect in the origin plane normal to $Qe_1-e_1$. This reflection sends $Qe_1$ to $e_1$. The remaining orthogonal transformation fixes $e_1$ and acts on its two-dimensional orthogonal complement; repeat with $e_2$, and then on the last one-dimensional complement. At most three plane [reflections](../../../../../reflection-mathematics.md) are needed. A translation $x\mapsto x+b$ is itself a product of two reflections in parallel planes: for $\mathbf n=b/|b|$, reflecting first in $\mathbf n\cdot x=0$ and then in $\mathbf n\cdot x=|b|/2$ gives that translation. Thus every isometry is a finite composition of plane reflections, the [finite reflection decomposition of a Euclidean isometry](../../../../../finite-reflection-decomposition-of-a-euclidean-isometry.md).

For an isometry fixing zero, the preceding construction gives $N\le3$. A plane reflection's linear part has $\operatorname{rank}(I-R)=1$. The identity $I-AB=(I-A)+A(I-B)$ implies that a product of $m$ such linear parts has rank of $I-Q$ at most $m$, even if the reflecting planes are affine. For central inversion $Q=-I$, this rank is three. The [reflection length of a Euclidean orthogonal map](../../../../../reflection-length-of-a-euclidean-orthogonal-map.md) therefore gives

$$
\boxed{N=3,\qquad x\mapsto-x\text{ requires three reflections}}.
$$

For the regular tetrahedron, center it at zero. Every permutation of its four vertices determines an isometry, and the orientation-reversing ones correspond to odd permutations in $S_4$: six transpositions and six four-cycles. Each transposition is a plane reflection fixing the two unswapped vertices; its plane contains their edge and the midpoint of the opposite edge. These give six distinct mirror planes.

The other six are rotoreflections: rotate by $+\pi/2$ or $-\pi/2$ about an axis through the midpoints of a pair of opposite edges, and then reflect in the plane through the center perpendicular to that axis. There are three axes and two senses. For vertices $(1,1,1),(1,-1,-1),(-1,1,-1),(-1,-1,1)$, the map $(x,y,z)\mapsto(-y,x,-z)$ is one such four-cycle; the other axes and inverse rotations give all six. Hence the complete orientation-reversing [tetrahedral symmetry](../../../../../tetrahedral-symmetry.md) list is **six mirror reflections and six quarter-turn rotoreflections**.

## ↑ Ancestors (10)

1. [14E](../14e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
