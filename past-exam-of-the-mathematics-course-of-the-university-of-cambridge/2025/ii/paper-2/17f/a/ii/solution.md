<h1 id="17f/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $M$ be a maximum matching and put $m=|M|$. The $n-2m$ unmatched vertices form an independent set, since an edge between two of them could be added to $M$. Because $G$ is $k$-regular, exactly $k(n-2m)$ edges run from unmatched vertices to vertices covered by $M$.

Each endpoint of a matched edge has one incident edge in $M$, and hence at most $k-1$ incident edges from unmatched vertices. The two endpoints of each of the $m$ matched edges therefore receive at most $2k-2$ such edges. Thus

$$
k(n-2m)\leq(2k-2)m.
$$

Rearranging gives

$$
\boxed{\nu(G)=m\geq\frac{k}{4k-2}n.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [17F](../../../17f.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
