<h1 id="17g/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each edge $e$, let $I_e$ be the [indicator random variable](../../../../../../indicator-random-variable.md) of the event that precisely one endpoint lies in $U$. Independent inclusion of the two endpoints with probability $1/2$ gives

$$
\mathbb P(I_e=1)=2\left(\frac12\right)\left(\frac12\right)=\frac12.
$$

Because $X=\sum_{e\in E(G)}I_e$, [linearity of expectation](../../../../../../linearity-of-expectation.md) gives

$$
\boxed{\mathbb E X=\sum_{e\in E(G)}\mathbb E I_e=\frac m2.}
$$

Some realization therefore has $X\geq m/2$. Retaining its crossing edges gives a [subgraph](../../../../../../subgraph.md) that is [bipartite](../../../../../../bipartite-graph.md), with vertex classes $U$ and $V(G)\setminus U$, proving the [random cut lower bound](../../../../../../random-cut-lower-bound.md).

Now suppose $n$ is an [even number](../../../../../../even-number.md) and instead choose $U$ uniformly among all subsets of size $n/2$. For a fixed edge $uv$,

$$
\mathbb P(u\in U,v\notin U)
=\frac{n/2}{n}\frac{n/2}{n-1},
$$

and the reverse orientation has the same probability. Thus

$$
\mathbb P(I_{uv}=1)=\frac{n}{2(n-1)}.
$$

Another application of [linearity of expectation](../../../../../../linearity-of-expectation.md) gives

$$
\mathbb E X=\frac{mn}{2(n-1)}.
$$

At least one such balanced choice attains this expectation, and its crossing edges give the required [subgraph](../../../../../../subgraph.md) that is [bipartite](../../../../../../bipartite-graph.md). This is the [balanced random cut lower bound](../../../../../../balanced-random-cut-lower-bound.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [17G](../../17g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
