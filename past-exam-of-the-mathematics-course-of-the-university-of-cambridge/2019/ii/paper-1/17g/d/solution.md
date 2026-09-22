<h1 id="17g/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Suppose the only distinct eigenvalues are $d$ and $\theta$. As in part (c), $A$ acts by $d$ on $\operatorname{span}\{\mathbf e\}$ and by $\theta$ on $\mathbf e^\perp$, so its [spectral decomposition](../../../../../../spectral-decomposition.md) is

$$
A=\theta I+\frac{d-\theta}{n}J.
$$

Every diagonal entry of an adjacency matrix is zero, giving

$$
\theta+\frac{d-\theta}{n}=0.
$$

Thus every off-diagonal entry is the same number $(d-\theta)/n=-\theta$. Since these entries belong to $\{0,1\}$ and the graph is connected with at least two vertices, that common value must be one. Hence $A=J-I$ and $G$ is the [complete graph](../../../../../../complete-graph.md) $K_n$.

Conversely, $K_n$ has adjacency matrix $J-I$, with eigenvalue $n-1$ on $\operatorname{span}\{\mathbf e\}$ and eigenvalue $-1$ on $\mathbf e^\perp$. Therefore the requested graphs are precisely

$$
\boxed{K_n\quad(n\geq2)},
$$

as stated by the [connected regular graph with two adjacency eigenvalues](../../../../../../connected-regular-graph-with-two-adjacency-eigenvalues.md) characterization.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [17G](../../17g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
