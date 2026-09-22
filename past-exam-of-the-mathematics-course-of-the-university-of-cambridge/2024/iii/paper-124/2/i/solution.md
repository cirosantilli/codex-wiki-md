<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A decision problem $B$ is [NL-complete](../../../../../../nl-complete.md) when $B\in\mathbf{NL}$ and every language $A\in\mathbf{NL}$ has a deterministic [logarithmic space](../../../../../../logarithmic-space.md) many-one reduction to $B$.

The [directed graph reachability problem](../../../../../../st-connectivity.md) is the standard example. It lies in NL because a machine stores the current vertex and a counter, nondeterministically guesses at most $|V|-1$ successive edges, and accepts upon reaching $t$; this uses $O(\!\log|V|)$ space. For hardness, given an NL machine $M$ and input $x$, construct its [configuration graph](../../../../../../configuration-graph.md). Its configurations have logarithmic length, adjacency can be computed in logarithmic space, and

$$
M\text{ accepts }x
\quad\Longleftrightarrow\quad
\text{an accepting configuration is reachable from the initial configuration}.
$$

Adding one target joined from every accepting configuration gives the required logarithmic-space reduction.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
