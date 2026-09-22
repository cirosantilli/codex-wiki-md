<h1 id="17i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $N=(100\delta)^g$ and take $G\sim G(N,4\delta/N)$. Its expected number of edges is asymptotic to $2\delta N$, and a Chernoff bound makes $e(G)>3\delta N/2$ with positive probability. The expected number of cycles of length below $g$ is at most

$$
\sum_{\ell=3}^{g-1}\frac{(4\delta)^\ell}{2\ell}<(4\delta)^g,
$$

which is far below $\delta N/2$; Markov's inequality shows that, simultaneously with positive probability, there are fewer than $\delta N/2$ such cycles.

Choose such a graph and delete one edge from every cycle of length below $g$. The resulting graph has girth at least $g$ and more than $\delta N$ edges, hence average degree greater than $2\delta$. Part (a) supplies a subgraph of minimum degree at least $\delta$. It uses at most $N=(100\delta)^g$ vertices and cannot acquire any shorter cycle.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17I](../../17i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
