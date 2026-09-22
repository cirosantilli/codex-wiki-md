<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For even $r\geq2$, take the [complete graph](../../../../complete-graph.md) $K_{r+1}$. It is an $r$-[regular graph](../../../../regular-graph.md) on an odd number of [vertices](../../../../vertex-graph-theory.md). Every [matching in a graph](../../../../matching-graph-theory-split.md) has at most $r/2$ [edges](../../../../edge-of-a-graph.md), so $r$ colours in a [proper edge colouring](../../../../proper-edge-coloring.md) could cover at most $r^2/2$ [edges](../../../../edge-of-a-graph.md). But

$$
|E(K_{r+1})|=\frac{r(r+1)}2>\frac{r^2}2.
$$

Therefore $\chi'(K_{r+1})>r$; [Vizing's theorem](../../../../vizing-s-theorem.md) gives **$\chi'(K_{r+1})=r+1$**. This includes the [graph triangle](../../../../triangle-in-a-graph.md) when $r=2$.

For odd $r\geq3$, first construct a [graph](../../../../graph-split.md) $H_r$ on $r+2$ [vertices](../../../../vertex-graph-theory.md). Start with the [complete graph](../../../../complete-graph.md) on

$$
\{v,a,b,c_1,\ldots,c_{r-1}\},
$$

and delete the [edges](../../../../edge-of-a-graph.md) $va$, $vb$, and $c_1c_2,c_3c_4,\ldots,c_{r-2}c_{r-1}$. The pairing is possible because $r-1$ is even. In the initial [complete graph](../../../../complete-graph.md), every [vertex](../../../../vertex-graph-theory.md) has [vertex degree](../../../../degree-graph-theory.md) $r+1$. The distinguished [vertex](../../../../vertex-graph-theory.md) $v$ loses two [edges](../../../../edge-of-a-graph.md) and every other [vertex](../../../../vertex-graph-theory.md) loses exactly one, giving

$$
d_{H_r}(v)=r-1,\qquad d_{H_r}(x)=r\quad(x\ne v).
$$

Take two disjoint copies of $H_r$, with distinguished [vertices](../../../../vertex-graph-theory.md) $v,v'$, and add the [edge](../../../../edge-of-a-graph.md) $vv'$. The resulting [simple graph](../../../../simple-graph.md) $G_r$ is an $r$-[regular graph](../../../../regular-graph.md). The added [edge](../../../../edge-of-a-graph.md) is the only [edge](../../../../edge-of-a-graph.md) between the two copies; each copy has the odd number $r+2$ of [vertices](../../../../vertex-graph-theory.md).

Suppose an $r$-colour [proper edge colouring](../../../../proper-edge-coloring.md) existed. At each [vertex](../../../../vertex-graph-theory.md), the $r$ incident [edges](../../../../edge-of-a-graph.md) would use all $r$ colours. Thus each colour would form a [perfect matching](../../../../perfect-matching.md). Any [perfect matching](../../../../perfect-matching.md) must use $vv'$: without it, each odd-sized copy would have to be covered by internal pairs, which is impossible by [parity](../../../../parity.md). Therefore all $r$ colour classes would have to contain the same [edge](../../../../edge-of-a-graph.md) $vv'$, a contradiction. Hence [Vizing's theorem](../../../../vizing-s-theorem.md) again gives

$$
\boxed{\chi'(G_r)=r+1>r.}
$$

These constructions give [class two regular graphs](../../../../class-two-regular-graph.md) for every $r\geq2$. The odd-$r$ construction exhibits the [bridge obstruction to regular edge colouring](../../../../bridge-obstruction-to-regular-edge-colouring.md); $H_r$ is a [connected graph](../../../../connected-graph.md) because every [vertex](../../../../vertex-graph-theory.md) other than $a,b,v$ is adjacent to $v$, while $a,b$ are adjacent to those [vertices](../../../../vertex-graph-theory.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the graph theory course of the University of Oxford](../../../split.md)
5. [Graph theory course of the University of Oxford](../../../../graph-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
