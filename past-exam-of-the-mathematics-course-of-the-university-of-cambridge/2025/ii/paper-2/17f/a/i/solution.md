<h1 id="17f/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let the bipartition be $X\sqcup Y$. Counting edges from each side gives

$$
k|X|=|E(G)|=k|Y|,
$$

so $|X|=|Y|=n/2$. For $S\subseteq X$, the $k|S|$ edges leaving $S$ all end in $N(S)$, while each vertex of $N(S)$ receives at most $k$ of them. Therefore

$$
k|S|\leq k|N(S)|,
$$

and Hall's condition holds. There is a matching covering $X$, of size $n/2$. No matching can use more than one edge at each vertex, so this is maximal and

$$
\boxed{\nu(G)=\frac n2.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
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
