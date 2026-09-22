# Hall allocation model

↑ **Parent:** [Hall's marriage theorem](hall-s-marriage-theorem.md)

In a unit-capacity [assignment problem](assignment-problem.md), left [vertices](vertex-graph-theory.md) represent demands and right [vertices](vertex-graph-theory.md) represent individually usable resources; an [edge](edge-of-a-graph.md) records compatibility. All constraints must be encoded by those allowed pairs and by using each resource at most once. [Hall's marriage theorem](hall-s-marriage-theorem.md) decides feasibility. Costs belong to an additional [mathematical optimization](mathematical-optimization-split.md) problem; precedence between jobs or requirements for consecutive slots need additional modelling.

The authored [Notes on the design of a conference scheduler by David R. MacIver](notes-on-the-design-of-a-conference-scheduler-by-david-r-maciver.md) (Implementation, 7 August 2022) illustrates a [Hall obstruction](hall-obstruction.md) with four talks confined to three slots. With one talk per slot, that [subset](subset.md) has size four and a [graph neighbourhood](graph-neighbourhood.md) of size three. An unused slot outside its [graph neighbourhood](graph-neighbourhood.md) does not remove the bottleneck. In the three-job example above, the same [scheduling](scheduling.md) model instead has two complete assignments.

The allocation exercise in [Graph Theory by Reinhard Diestel](graph-theory-by-reinhard-diestel.md) (Matching, Covering and Packing, printed p. 20, Exercise 9) asks for disjoint [subsets](subset.md) $D_i\subseteq A_i$ of prescribed nonnegative [integer](integer-split.md) sizes $d_i$. Replace demand $i$ by $d_i$ left [vertices](vertex-graph-theory.md) with allowed resource [set](set-split.md) $A_i$. [Hall's marriage theorem](hall-s-marriage-theorem.md) gives exactly the condition

$$
\left|\bigcup_{i\in I}A_i\right|\geq\sum_{i\in I}d_i\qquad\text{for every index subset }I.
$$

For a numerical instance, let $A_1=\{1,2\}$, $A_2=\{2,3\}$, and $d_1=2,d_2=1$. The separate demands and their combined demand fit, and $D_1=\{1,2\},D_2=\{3\}$ works. Raising $d_2$ to two leaves both individual tests valid but demands four distinct resources from a [set union](set-union.md) of size three. This is the same collective obstruction with repeated demand [vertices](vertex-graph-theory.md).

## ↑ Ancestors (7)

1. [Hall's marriage theorem](hall-s-marriage-theorem.md)
2. [Matching (graph theory)](matching-graph-theory-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
