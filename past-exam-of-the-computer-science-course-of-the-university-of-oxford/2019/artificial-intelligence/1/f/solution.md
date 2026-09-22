<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For the [three-colourability problem](../../../../../three-colourability-problem.md), represent a candidate by a complete colour assignment $c:V\to\{r,g,b\}$, initially chosen at random. Give it the conflict [objective function](../../../../../objective-function.md)

$$
H(c)=\sum_{\{u,v\}\in E}\mathbf1_{c(u)=c(v)}.
$$

A neighbor changes the colour of one [vertex](../../../../../vertex-graph-theory.md) to either other colour. For [hill climbing](../../../../../hill-climbing.md), maximize $-H$, or equivalently repeatedly choose a recolouring that reduces $H$. One can inspect all $2|V|$ neighbors, or focus on conflicted [vertices](../../../../../vertex-graph-theory.md) and evaluate their alternative colours using only incident [edges](../../../../../edge-of-a-graph.md). Stop successfully as soon as **$H=0$**, which is exactly a [proper graph colouring](../../../../../graph-coloring-split.md) with three colours.

If no improving move exists at positive $H$, the method is stuck in a [local minimum](../../../../../local-minimum.md). Random restarts, limited sideways moves or other exploratory [local search](../../../../../local-search.md) choices can reduce this failure mode, but do not turn a finite unsuccessful run into a proof of impossibility. On a graph with no [proper graph colouring](../../../../../graph-coloring-split.md) using three colours, every complete colouring has $H>0$, so this procedure cannot return a valid colouring. Conversely, a positive-conflict stopping point also occurs on some graphs admitting a [proper graph colouring](../../../../../graph-coloring-split.md) with three colours. **Failure of [hill climbing](../../../../../hill-climbing.md) alone does not certify non-colourability.** For a concrete trap, use a [bipartite graph](../../../../../bipartite-graph-split.md) with three [vertices](../../../../../vertex-graph-theory.md) on each side and every cross-[edge](../../../../../edge-of-a-graph.md), and give each side one vertex of each colour. There are three conflicts. Recolouring any single vertex leaves it with exactly one same-colour neighbor, so no single change improves $H$, even though colouring each whole side differently solves the instance.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
