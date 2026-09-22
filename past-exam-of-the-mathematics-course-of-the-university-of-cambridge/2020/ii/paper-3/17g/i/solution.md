<h1 id="17g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Turan theorem](../../../../../../turan-s-theorem.md) states that among all $N$-vertex graphs containing no $K_{r+1}$, the maximum number of [edges](../../../../../../edge-of-a-graph.md) is attained by the [Turán graph](../../../../../../turan-graph.md) $T_r(N)$, the [complete multipartite graph](../../../../../../complete-multipartite-graph.md) whose $r$ part sizes differ by at most one.

Here is the [Zykov symmetrization](../../../../../../zykov-symmetrization.md) proof. Start with an extremal $K_{r+1}$-free graph. If nonadjacent vertices $u,v$ have different neighbourhoods, replace the lower-degree vertex by a clone of the higher-degree one: delete all its incident edges and join it to precisely the neighbours of the other vertex. This does not decrease the number of edges and cannot create a $K_{r+1}$, because a clique using the clone corresponds to one using the original vertex. Repeating the operation, with the standard tie-breaking that merges equal-neighbourhood classes, produces a complete multipartite extremal graph. It has at most $r$ nonempty parts, since choosing one vertex from each part gives a clique.

If two part sizes satisfy $a\geq b+2$, moving one vertex from the larger part to the smaller changes the number of cross-edges by

$$
a-b-1>0.
$$

**Thus an extremal partition has exactly $r$ parts whose sizes differ by at most one. This is $T_r(N)$ and proves the theorem. For $r=2$ it is [Mantel theorem](../../../../../../mantel-theorem.md): a triangle-free graph on $N$ vertices has at most $\lfloor N^2/4\rfloor$ edges.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [17G](../../17g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
