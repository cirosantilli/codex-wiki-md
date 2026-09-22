<h1 id="17f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Menger theorem](../../../../../../menger-theorem.md) says that the maximum number of pairwise vertex-disjoint $A$--$B$ paths equals the minimum size of an $A$--$B$ separating vertex set, with the standard convention that the path endpoints lie in $A\cup B$. The connectivity $\kappa(G)$ is the minimum number of vertices whose deletion disconnects $G$ or leaves a single vertex; $\kappa(K_n)=n-1$.

The vertex form says that for distinct nonadjacent vertices $x,y$, the maximum number of internally vertex-disjoint $x$--$y$ paths equals the minimum size of an $x$--$y$ separator disjoint from $\{x,y\}$. It follows from the set form by splitting off the endpoints, or by applying it to their neighbor sets after deleting $x,y$.

Now let $C$ be a longest cycle. If $|C|<2k\leq|G|$, some component $H$ of $G-C$ exists. Its neighbor set $N_C(H)$ is a vertex separator, so it contains at least $k$ vertices. No two of these attachment vertices can be consecutive on $C$: a path through the connected component $H$ between consecutive attachments would replace their edge by a path of at least two edges and create a longer cycle. Thus $C$ contains at least one nonattachment between each of at least $k$ attachments, and $|C|\geq2k$, a contradiction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17F](../../17f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
