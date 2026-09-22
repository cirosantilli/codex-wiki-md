<h1 id="17f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Colour every [vertex of a graph](../../../../../../vertex-graph-theory.md) independently and uniformly with three colours, and retain precisely the [edges](../../../../../../edge-of-a-graph.md) whose endpoints have different colours. Each edge is retained with probability $2/3$, so [linearity of expectation](../../../../../../linearity-of-expectation.md) gives expected retained edge count

$$
\frac23e(G).
$$

Some colouring therefore retains at least $2e(G)/3$ edges. Its retained [subgraph](../../../../../../subgraph.md) is three-colourable, and deleting edges if necessary leaves exactly

$$
\boxed{\left\lfloor\frac23e(G)\right\rfloor}
$$

edges without increasing its [chromatic number](../../../../../../chromatic-number.md). This is the [three-colourable two-thirds subgraph lemma](../../../../../../three-colourable-two-thirds-subgraph-lemma.md).

To prove sharpness, take $G=K_n$. If $H\subseteq K_n$ is three-colourable and its colour classes have sizes $n_1,n_2,n_3$, then they are [independent sets](../../../../../../independent-set-graph-theory.md), so

$$
e(H)\leq n_1n_2+n_1n_3+n_2n_3
=\frac12\left(n^2-\sum_i n_i^2\right)
\leq\frac{n^2}{3},
$$

where the final inequality follows from [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Since $e(K_n)=n(n-1)/2$,

$$
\frac{e(H)}{e(K_n)}\leq\frac{2n}{3(n-1)}
=\frac23+\frac{2}{3(n-1)}.
$$

Given $\varepsilon>0$, choose $n$ with $2/[3(n-1)]\leq\varepsilon$. Then every three-colourable subgraph has at most $(2/3+\varepsilon)e(G)$ edges.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17F](../../17f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
