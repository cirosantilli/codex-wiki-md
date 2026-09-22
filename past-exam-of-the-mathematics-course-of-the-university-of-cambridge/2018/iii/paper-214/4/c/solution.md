<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume first that deleting an edge leaves two [transient graph](../../../../../../transient-graph.md) components. One component supports a finite-energy [unit flow](../../../../../../unit-flow.md) from its endpoint to infinity by the [finite-energy flow criterion for transience](../../../../../../finite-energy-flow-criterion-for-transience.md). Extend that [flow](../../../../../../flow.md) by zero across the deleted edge and throughout the other component. It remains a finite-energy [unit flow](../../../../../../unit-flow.md) on the whole [tree](../../../../../../tree-graph-theory.md), so the [tree](../../../../../../tree-graph-theory.md) is a [transient graph](../../../../../../transient-graph.md).

Conversely, root a transient [tree](../../../../../../tree-graph-theory.md) at $o$ and take its finite-energy unit electrical [flow](../../../../../../flow.md) to infinity. On a [tree](../../../../../../tree-graph-theory.md) this [flow](../../../../../../flow.md) can be chosen nonnegative in every direction away from the root: it is obtained as the limit of the currents to wired boundaries, each of which sends nonnegative current into descendant subtrees. At each nonroot vertex its incoming current equals the sum of its outgoing currents, by [flow conservation](../../../../../../flow-conservation.md).

If every vertex reached by positive current had exactly one positive-current child, the unit current would run along a single infinite ray. Every edge of that ray would carry current one, so its [energy of a flow](../../../../../../energy-of-a-flow.md) would be $\sum_{j\geq1}1=\infty$, a contradiction. Thus there is a vertex $v$ with two positive-current child edges, say $(v,x)$ and $(v,y)$.

The restricted [flow](../../../../../../flow.md) below $x$, rescaled by its incoming current, is a finite-energy [unit flow](../../../../../../unit-flow.md) from $x$ to infinity; hence the component below $x$ is a [transient graph](../../../../../../transient-graph.md). After removing $(v,x)$, the other component contains $v$, the edge $(v,y)$, and the descendant subtree below $y$. Send unit current along $(v,y)$ and then use the rescaled descendant [flow](../../../../../../flow.md) below $y$, with zero current elsewhere. Its [energy of a flow](../../../../../../energy-of-a-flow.md) is finite, so this component is a [transient graph](../../../../../../transient-graph.md) too. Therefore

$$
\boxed{G\text{ is transient}\quad\Longleftrightarrow\quad\exists e\in E:\ G\setminus e\text{ has two transient components}.}
$$

Unit edge resistances are essential here: an infinite ray with sufficiently rapidly decreasing resistances can be transient without any such splitting edge.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
