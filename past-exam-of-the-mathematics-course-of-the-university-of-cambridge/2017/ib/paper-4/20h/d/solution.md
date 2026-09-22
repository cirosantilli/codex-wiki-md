<h1 id="20h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**No: the increase need not equal $\varepsilon$.** For a simple counterexample, use two edge-disjoint paths $s\to a\to t$ and $s\to b\to t$, with all four capacities equal to one. Initially the [maximum flow](../../../../../../maximum-flow-problem.md) is $2$. After every capacity increases to $1+\varepsilon$, send $1+\varepsilon$ down each path; a source [cut of a flow network](../../../../../../cut-of-a-flow-network.md) bounds the total by the same value. Hence

$$
\boxed{\text{new maximum}=2+2\varepsilon,\qquad\text{increase}=2\varepsilon}.
$$

More generally, by the [max-flow min-cut theorem](../../../../../../max-flow-min-cut-theorem.md), if $m(S)$ is the number of directed edges leaving a [cut of a flow network](../../../../../../cut-of-a-flow-network.md), [uniform capacity perturbation of a flow network](../../../../../../uniform-capacity-perturbation-of-a-flow-network.md) gives

$$
\boxed{v(\varepsilon)=\min_{S:s\in S,\,t\notin S}\bigl(c(S)+\varepsilon m(S)\bigr)}.
$$

The number of outgoing edges, and possible changes of the minimising [cut of a flow network](../../../../../../cut-of-a-flow-network.md), determine the increase. If the question were interpreted as asking for an increase of at least $\varepsilon$, this does hold when the graph has a directed $s$-to-$t$ path, because then every [cut of a flow network](../../../../../../cut-of-a-flow-network.md) has $m(S)\geq1$. Without such a path a zero-edge [cut of a flow network](../../../../../../cut-of-a-flow-network.md) remains of capacity zero and the maximum can stay zero. Thus neither an exact increment nor an unconditional positive increment follows merely by adding the same amount to every edge capacity.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [20H](../../20h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
