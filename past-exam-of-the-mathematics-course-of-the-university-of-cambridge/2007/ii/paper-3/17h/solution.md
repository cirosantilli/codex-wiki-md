<h1 id="17h/solution">Solution</h1>

↑ **Parent:** [17H](../17h.md)

[Hall marriage theorem](../../../../../hall-s-marriage-theorem.md) says that a [bipartite graph](../../../../../bipartite-graph.md) with equal finite vertex-class sizes has a [perfect matching](../../../../../perfect-matching.md) exactly when $|\Gamma(A)|\geq|A|$ for every $A\subseteq X$. Necessity follows because distinct matched partners of vertices of $A$ belong to $\Gamma(A)$.

For sufficiency, induct on $n$, the case $n=1$ being immediate. If a nonempty proper $A$ is tight, $|\Gamma(A)|=|A|$, the induced graph between $A$ and $\Gamma(A)$ satisfies Hall's condition and has a matching by induction. The remaining graph also satisfies it: for $B\subseteq X\setminus A$, the condition on $A\cup B$ gives $|\Gamma(B)\setminus\Gamma(A)|\geq|B|$. Induction gives the second matching, and their union is perfect. Otherwise every nonempty proper subset has strictly more neighbours. Choose an edge $xy$ and remove its ends. Every remaining nonempty subset loses at most one neighbour and originally had at least one spare neighbour, so Hall's condition survives. Induction matches the remaining graph, and restoring $xy$ completes the proof.

The last argument also proves flexibility under the strict condition: it works for every selected edge, so **every vertex is flexible**. The case $n=1$ is again immediate.

Now suppose only that a [perfect matching](../../../../../perfect-matching.md) exists. Choose a minimal nonempty tight set $A\subseteq X$; such a set exists since $X$ is tight. Every nonempty proper subset of $A$ satisfies the strict condition in the induced graph on $A,\Gamma(A)$. Hence every edge from a vertex of $A$ extends to a matching of that induced graph. There are no edges from $A$ to the complement of $\Gamma(A)$. Restrict the original [perfect matching](../../../../../perfect-matching.md) to the complementary vertex classes and append it to this new induced matching. This makes every vertex of $A$ flexible in the whole graph, proving that **at least one flexible vertex exists**.

For the requested counterexample, take $X=\{x_1,x_2,x_3,x_4\}$ and $Y=\{y_1,y_2,y_3,y_4\}$. Join $x_1$ only to $y_1,y_2$, and join each of $x_2,x_3,x_4$ to all of $y_2,y_3,y_4$. There is a [perfect matching](../../../../../perfect-matching.md) using $x_1y_1$ and a matching of the remaining complete [bipartite graph](../../../../../bipartite-graph.md). The unique minimum-degree vertex is $x_1$, of degree two, but $x_1y_2$ cannot occur in a [perfect matching](../../../../../perfect-matching.md) because $y_1$ has no other neighbour. Thus **no minimum-degree vertex is flexible**, while the other three vertices are flexible.

## ↑ Ancestors (10)

1. [17H](../17h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
