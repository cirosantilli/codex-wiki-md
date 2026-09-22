<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $ij$ for the undirected edge $\{i,j\}$. At the root of the [branch and bound](../../../../branch-and-bound.md) search, the [minimum spanning tree](../../../../minimum-spanning-tree.md) on $\{2,3,4\}$ is $\{24,34\}$ of cost $6+4=10$. The cheapest edges incident to vertex one are $12,14$, of cost $3+7=10$. The root [lower bound](../../../../lower-bound-in-a-partially-ordered-set.md) is therefore twenty, attained by

$$
T_0=\{12,14,24,34\}.
$$

It is not a tour: vertex four has degree three and vertex three degree one.

A tour must omit at least one edge from $\{14,24,34\}$, since its degree at vertex four is two. Partition tours according to the first omitted edge in that ordered list. This gives three disjoint, exhaustive children, retaining included and excluded edges when recomputing the [one-tree](../../../../1-tree.md) relaxation:

- Exclude $14$. The incident pair is now $12,13$ of cost twelve, and the other [spanning tree](../../../../spanning-tree.md) still costs ten. The resulting [one-tree](../../../../1-tree.md) $\{12,13,24,34\}$ is a tour, so it supplies an [incumbent solution](../../../../incumbent-solution.md) of cost $22$.
- Include $14$ and exclude $24$. The other [spanning tree](../../../../spanning-tree.md) must be $\{23,34\}$ of cost fourteen; the cheapest permitted incident pair costs ten. The [lower bound](../../../../lower-bound-in-a-partially-ordered-set.md) is $24\geq22$, so prune this child.
- Include $14,24$ and exclude $34$. The [spanning tree](../../../../spanning-tree.md) must be $\{23,24\}$ of cost sixteen; the incident pair again costs ten. The [lower bound](../../../../lower-bound-in-a-partially-ordered-set.md) is $26\geq22$, so prune this child too.

All tours belong to one of the three children, and no remaining child can improve the incumbent. Therefore

$$
\boxed{1\to2\to4\to3\to1\text{ is optimal, with cost }3+6+4+9=22.}
$$

The branching rule is motivated by a violated tour degree equation, rather than by an arbitrary costly edge. This is [degree branching with a one-tree bound](../../../../degree-branching-with-a-one-tree-bound.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
