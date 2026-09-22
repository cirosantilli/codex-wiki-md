<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The blue hypergraph in the question is the three-edge hypergraph $K_4^{(3)-}$. The [Erdős-Hajnal bound for the three-edge hypergraph on four vertices](../../../../../../erdos-hajnal-bound-for-the-three-edge-hypergraph-on-four-vertices.md) states that every $K_4^{(3)-}$-free three-uniform hypergraph on $N$ vertices has an independent set of size at least

$$
c\frac{\log N}{\log\log N}.
$$

Its proof exposes vertices successively and studies their link graphs. A blue triangle in a link is exactly a blue $K_4^{(3)-}$, so all links are triangle-free; applying the [Shearer independence bound for a triangle-free graph](../../../../../../shearer-independence-bound-for-a-triangle-free-graph.md) in dyadic degree ranges either adds vertices to the independent set or leaves a reservoir whose logarithm decreases by only $O(\log\log N)$ per selected vertex. Iteration yields the displayed lower bound.

Now take $N=k^{Ck}$. For sufficiently large $C$,

$$
c\frac{\log N}{\log\log N}
=c\frac{Ck\log k}{\log(Ck\log k)}
\ge k.
$$

Thus, if there is no blue copy of $H$, the blue hypergraph has an independent $k$-set, which is a red $K_k^{(3)}$. Therefore

$$
\boxed{r(H,K_k^{(3)})\le k^{Ck}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
