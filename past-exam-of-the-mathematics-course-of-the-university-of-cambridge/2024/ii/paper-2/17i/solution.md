<h1 id="17i/solution">Solution</h1>

↑ **Parent:** [17I](../17i.md)

The [Turan theorem](../../../../../turan-s-theorem.md) states that every $n$-vertex graph with no $K_{r+1}$ has at most $e(T_r(n))$ edges, where $T_r(n)$ is the complete $r$-partite graph with part sizes differing by at most one.

Here is an induction on $n$ and $r$. If a $K_{r+1}$-free graph $G$ contains no $K_r$, induction on $r$ gives

$$
e(G)\leq e(T_{r-1}(n))\leq e(T_r(n)).
$$

Otherwise choose a copy $S$ of $K_r$. Every vertex outside $S$ has at most $r-1$ neighbors in $S$, and induction on $n$ gives

$$
e(G)\leq e(T_r(n-r))+\binom r2+(r-1)(n-r)=e(T_r(n)).
$$

The last identity is obtained by removing one vertex from every part of $T_r(n)$. This proves the theorem; the standard equality analysis forces the balanced complete $r$-partite graph.

Now suppose $G$ is rhombus-free. If it is triangle-free, the $r=2$ case just proved gives  
$e(G)\leq e(T_2(n))$. Otherwise remove the three vertices of a triangle. No remaining vertex can be adjacent to two vertices of that triangle, since those two triangle vertices and the outside vertex would form a second triangle sharing an edge with the first. Induction therefore gives

$$
e(G)\leq
\left\lfloor\frac{(n-3)^2}{4}\right\rfloor+3+(n-3)
\leq\left\lfloor\frac{n^2}{4}\right\rfloor
=e(T_2(n)).
$$

This proves the [rhombus-free edge bound](../../../../../rhombus-free-edge-bound.md) and hence the requested strict contrapositive.

For equality at $n=6$, take the [triangular prism graph](../../../../../triangular-prism-graph.md): two disjoint triangles joined by a matching. It has $6+3=9=e(T_2(6))$ edges. Every edge belongs to at most one triangle, so there is no rhombus, while the presence of triangles proves that it is not isomorphic to $T_2(6)=K_{3,3}$.

## ↑ Ancestors (10)

1. [17I](../17i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
