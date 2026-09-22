<h1 id="17i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
P=v_1v_2\cdots v_m
$$

be a longest path. Every neighbour of either endpoint lies on $P$. Among the $m-1$ possible cuts between consecutive vertices, mark a cut $i$ when $v_m v_i$ is an edge and also mark it when $v_1v_{i+1}$ is an edge. There are at least

$$
d(v_m)+d(v_1)\geq n>m-1
$$

marks, so some cut receives both marks. The path edges together with $v_mv_i$ and $v_{i+1}v_1$ form a cycle through all vertices of $P$.

The degree assumption makes $G$ connected: two components would each contain at least $n/2+1$ vertices. If $m<n$, connectedness gives an edge from a vertex outside the cycle to a vertex on it; breaking the cycle there produces a path with $m+1$ vertices, contrary to maximality. Hence $m=n$, so $G$ is Hamiltonian. This proves the [Dirac theorem](../../../../../../dirac-s-theorem.md) in this case.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17I](../../17i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
