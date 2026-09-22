<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At $p=1/2$, explore the directed out-cluster of the origin by a deterministic breadth-first procedure. Maintain the set of reached [graph vertices](../../../../../../vertex-graph-theory.md) and a queue of untested [edges](../../../../../../edge-of-a-graph.md) with one reached and one unreached endpoint. For each such [edge](../../../../../../edge-of-a-graph.md), reveal its orientation. Add the unreached endpoint if the arrow points from the reached endpoint to it; otherwise discard that [edge](../../../../../../edge-of-a-graph.md). [edges](../../../../../../edge-of-a-graph.md) whose endpoints are both already reached need no further test.

An untested [edge](../../../../../../edge-of-a-graph.md) has an independent fair orientation even though the choice of the next [edge](../../../../../../edge-of-a-graph.md) depends on earlier discoveries. Its [probability](../../../../../../probability.md) of pointing toward the unreached endpoint is $1/2$, whichever geometric direction that represents. Thus the discovery procedure has exactly the same transition [probabilities](../../../../../../probability.md) as the ordinary [bond percolation](../../../../../../bond-percolation-split.md) cluster exploration at density $1/2$. In particular, for every $m$, the [probability](../../../../../../probability.md) of reaching at least $m$ [graph vertices](../../../../../../vertex-graph-theory.md) agrees in the two models. The [uniform random orientation out-cluster comparison](../../../../../../uniform-random-orientation-out-cluster-comparison.md) implies

$$
\mathbb P(|C^{\to}(0)|=\infty)=\theta(1/2).
$$

A [locally finite graph](../../../../../../locally-finite-graph.md) has an infinite directed simple ray from the origin exactly when its directed out-cluster is infinite: the exploration predecessor [edges](../../../../../../edge-of-a-graph.md) form a finitely branching rooted [tree](../../../../../../tree-graph-theory.md), to which the [König infinity lemma](../../../../../../konig-s-lemma.md) applies. Conversely, such a ray visits infinitely many reachable [graph vertices](../../../../../../vertex-graph-theory.md). Hence

$$
\boxed{\psi(1/2)=\theta(1/2)=0.}
$$

Fairness of orientations is essential to this comparison; for general $p$ the success [probability](../../../../../../probability.md) depends on the geometric direction of exploration. As usual, an infinite directed path means a ray with distinct [graph vertices](../../../../../../vertex-graph-theory.md). Allowing a finite directed cycle to be traversed repeatedly would define an infinite walk instead and would make the claimed conclusion false.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
