<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Describe a branching vertex by the [first-order logic](../../../../../first-order-logic.md) sentence

$$
\beta=\exists x\exists y\exists z\,[E(x,y)\land E(x,z)\land y\ne z],
$$

and the existence of a sink by $\delta=\exists x\forall y\,\neg E(x,y)$. The directed path has sinks but no branching vertex; the directed cycle has neither sinks nor branching vertices; the directed arborescence has a branching vertex. Thus the following three sentences distinguish the named structures in order:

$$
\boxed{\varphi_1=\delta\land\neg\beta,\qquad\varphi_2=\forall x\exists y\,E(x,y),\qquad\varphi_3=\beta.}
$$

Here $\beta,\delta$ are abbreviations for the displayed formulas; replacing them gives sentences in the single-relation [first-order signature](../../../../../first-order-signature.md) $\{E\}$. Explicitly, $\varphi_1$ says that some vertex has no successor and that no vertex has two distinct successors. The [truth table](../../../../../truth-table.md) across the three structures is:

| Sentence | $\mathcal G_1$ | $\mathcal G_2$ | $\mathcal G_3$ |
| --- | --- | --- | --- |
| $\varphi_1$ | $1$ | $0$ | $0$ |
| $\varphi_2$ | $0$ | $1$ | $0$ |
| $\varphi_3$ | $0$ | $0$ | $1$ |

The conditions distinguish these three finite structures; they are not claimed to characterize all directed paths, cycles or trees among arbitrary [directed graphs](../../../../../directed-graph.md). Only local [out-degrees](../../../../../outdegree.md) and the presence of a sink are needed, without quantifying over paths of unbounded length.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
