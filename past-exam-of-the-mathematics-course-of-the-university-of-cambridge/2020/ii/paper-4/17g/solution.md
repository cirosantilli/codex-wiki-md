<h1 id="17g/solution">Solution</h1>

↑ **Parent:** [17G](../17g.md)

[Vizing theorem](../../../../../vizing-s-theorem.md) states that every finite simple [graph](../../../../../graph-split.md) of [maximum degree](../../../../../maximum-degree-of-a-graph.md) $\Delta$ has

$$
\Delta\leq\chi'(G)\leq\Delta+1,
$$

where $\chi'(G)$ is its [edge chromatic number](../../../../../edge-chromatic-number.md). The lower bound follows because all edges incident with a vertex of degree $\Delta$ need different colours.

For the upper bound, induct on the number of edges. Delete an edge $xy$ and colour the remaining graph with the palette $\{1,\ldots,\Delta+1\}$. We use the [Vizing fan lemma](../../../../../vizing-fan-lemma.md): in a partial proper edge colouring with one uncoloured edge $xy$, if the palette has one more colour than the maximum degree, a sequence of fan rotations and two-colour [Kempe-chain](../../../../../kempe-chain.md) interchanges makes some colour missing at both ends of the uncoloured edge.

Here is the fan argument. Build a maximal sequence $y_0=y,y_1,\ldots,y_k$ of distinct neighbours of $x$ such that, for $i\geq1$, the colour on $xy_i$ is missing at an earlier fan vertex. Rotating an initial fan segment means moving each colour on $xy_i$ to the preceding edge where it is missing; this preserves properness and moves the uncoloured edge to the end of that segment. Choose a colour $\alpha$ missing at $x$ and a colour $\beta$ missing at $y_k$. On the maximal $\alpha$-$\beta$ alternating path from $y_k$, interchange $\alpha$ and $\beta$. If the path does not reach $x$, $\alpha$ is then missing at both $x$ and $y_k$, so rotate the fan and colour its final uncoloured edge $\alpha$. If it reaches $x$, its last edge at $x$ has colour $\beta$. Maximality of the fan forces the other endpoint of that edge to be a fan vertex; rotate up to that vertex first. This breaks the alternating path before $x$, reducing to the preceding case. This proves the fan lemma and extends the colouring to $xy$, completing the induction.

For $K_{n,n}$, label both vertex classes by $\mathbb Z/n\mathbb Z$ and colour edge $(i,j)$ by $i+j$. Each colour is a [perfect matching](../../../../../perfect-matching.md), so this is an $n$-edge-colouring. Since $\Delta(K_{n,n})=n$, $\chi'(K_{n,n})=n$. If $r=\max\{m,n\}$, embed $K_{m,n}$ into $K_{r,r}$ and restrict its $r$-edge-colouring. The degree lower bound then gives

$$
\boxed{\chi'(K_{m,n})=\max\{m,n\}}.
$$

Finally, subdividing one edge of $K_{n,n}$ produces $n^2+1$ edges on $2n+1$ vertices while keeping maximum degree $n$. In any proper edge colouring, each colour class is a [matching](../../../../../matching-graph-theory.md) of size at most $n$. An $n$-edge-colouring could therefore colour at most $n^2$ edges, a contradiction. Thus $\chi'(G)>n$, while [Vizing theorem](../../../../../vizing-s-theorem.md) gives $\chi'(G)\leq n+1$, so

$$
\boxed{\chi'(G)=\Delta(G)+1=n+1}.
$$

## ↑ Ancestors (10)

1. [17G](../17g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
