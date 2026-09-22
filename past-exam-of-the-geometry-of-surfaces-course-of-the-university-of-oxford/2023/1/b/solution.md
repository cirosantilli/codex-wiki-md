<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Number the [polygon vertices](../../../../vertex-of-a-polygon.md) $v_0,\ldots,v_9$ in the order of the given [polygonal schema](../../../../polygonal-schema.md), with its $i$th [polygon edge](../../../../side-of-a-polygon.md) going from $v_i$ to $v_{i+1}$, and subscripts interpreted modulo ten. Equal labels identify equal arrow endpoints. The five pairings give

$$
\begin{array}{c|cc}
\text{label}&\text{first endpoints}&\text{second endpoints}\\
a_1&v_0\sim v_4&v_1\sim v_3\\
a_2&v_2\sim v_7&v_3\sim v_6\\
a_3&v_5\sim v_9&v_6\sim v_8\\
a_4&v_2\sim v_9&v_1\sim v_0\\
a_5&v_5\sim v_7&v_4\sim v_8
\end{array}
$$

Consequently there are two vertex [equivalence classes](../../../../equivalence-class.md),

$$
\{v_0,v_1,v_3,v_4,v_6,v_8\},\qquad\{v_2,v_5,v_7,v_9\}.
$$

The [quotient space](../../../../quotient-topological-space.md) has one face, five edges and two vertices, so the [polygonal-schema Euler count](../../../../polygonal-schema-euler-count.md) gives

$$
\boxed{\chi(X)=2-5+1=-2.}
$$

Each label occurs once with each sign. Hence every pairing reverses the direction induced by traversing the [boundary](../../../../boundary-of-a-set.md) of the [polygon](../../../../polygon.md), so an [orientation of a surface](../../../../orientation-of-a-surface.md) on its interior extends consistently across every glued edge. Thus $X$ is [orientable](../../../../orientable-surface.md). The [classification of compact surfaces](../../../../classification-of-compact-surfaces.md) now gives $2-2g=-2$, or **a closed [orientable surface](../../../../orientable-surface.md) of [genus](../../../../genus-of-a-surface.md) two**, equivalently the [connected sum of surfaces](../../../../connected-sum-of-surfaces.md) of two [tori](../../../../torus.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the geometry of surfaces course of the University of Oxford](../../../split.md)
5. [Geometry of surfaces course of the University of Oxford](../../../../geometry-of-surfaces-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
