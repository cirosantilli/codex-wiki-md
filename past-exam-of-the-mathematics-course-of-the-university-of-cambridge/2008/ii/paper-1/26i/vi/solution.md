<h1 id="26i/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Write $q_{ij}=c m_{ij}$ for $i\ne j$, with a common positive constant $c$, and put $d_i=\sum_{j\ne i}m_{ij}$. The [infinitesimal generator matrix](../../../../../../transition-intensity-matrix.md) is symmetric because the graph is undirected. Thus the [uniform distribution](../../../../../../continuous-uniform-distribution.md) $\pi_i=1/|I|$ satisfies [detailed balance](../../../../../../detailed-balance.md), and the [continuous-time random walk](../../../../../../continuous-time-random-walk.md) is reversible when started uniformly.

Its [jump chain](../../../../../../jump-chain.md) chooses a link uniformly from those incident to its current vertex:

$$
\widehat P_{ij}=\frac{m_{ij}}{d_i},\qquad \boxed{\widehat\pi_i=\frac{d_i}{\sum_jd_j}.}
$$

The flux $\widehat\pi_i\widehat P_{ij}=m_{ij}/\sum_jd_j$ is symmetric, so this [random walk on a multigraph](../../../../../../random-walk-on-a-multigraph.md) is also reversible. The continuous-time equilibrium is uniform because higher-degree vertices have shorter holding times; at jump times the equilibrium is degree-weighted. If the intended proportionality constant depends on the starting vertex, $q_{ij}=c_i m_{ij}$, reversibility still holds with $\pi_i\propto1/c_i$, and the same jump chain results.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [26I](../../26i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
