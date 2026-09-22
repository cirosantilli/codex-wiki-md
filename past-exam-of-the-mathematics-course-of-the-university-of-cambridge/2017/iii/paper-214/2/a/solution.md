<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the nearest-neighbour lattice [graph](../../../../../../graph-split.md) with [graph vertex](../../../../../../vertex-graph-theory.md) set $\mathbb Z^d$: an unordered pair $\{x,y\}$ is an [edge](../../../../../../edge-of-a-graph.md) precisely when $\|x-y\|_1=1$. A bond configuration is $\omega\in\{0,1\}^{E_d}$; under the [product measure](../../../../../../product-measure.md) $\mathbb P_p$, its [edge](../../../../../../edge-of-a-graph.md) coordinates are independent [Bernoulli distribution](../../../../../../bernoulli-distribution.md) with success [probability](../../../../../../probability.md) $p$. [Edges](../../../../../../edge-of-a-graph.md) with coordinate one are open. The open cluster $C(0)$ is the [connected component of a graph](../../../../../../component-graph-theory.md) reachable from the origin through open [edges](../../../../../../edge-of-a-graph.md).

Define the [percolation probability](../../../../../../percolation-probability.md) and [percolation critical probability](../../../../../../percolation-critical-probability.md) by

$$
\boxed{\theta_d(p)=\mathbb P_p(|C(0)|=\infty),\qquad p_c(d)=\inf\{p\in[0,1]:\theta_d(p)>0\}.}
$$

Equivalently, $p_c(d)=\sup\{p:\theta_d(p)=0\}$. The [monotone coupling of Bernoulli percolation](../../../../../../monotone-coupling-of-bernoulli-percolation.md) proves the equivalence: assign independent [uniform distribution](../../../../../../continuous-uniform-distribution.md) $U_e$ to the [edges](../../../../../../edge-of-a-graph.md) and open $e$ at parameter $p$ when $U_e\leq p$. Connection events and $\theta_d$ then increase with $p$. For $d\geq1$, $\theta_d(0)=0$ and $\theta_d(1)=1$, so the defining set is nonempty. The definition does not settle what happens at $p=p_c(d)$.

By translation invariance all roots have the same [probability](../../../../../../probability.md). Since the [graph vertex](../../../../../../vertex-graph-theory.md) set is countable, $\theta_d(p)=0$ implies that no [graph vertex](../../../../../../vertex-graph-theory.md) lies in an [infinite percolation cluster](../../../../../../infinite-percolation-cluster.md) [almost surely](../../../../../../almost-sure-convergence.md). Conversely a positive root [probability](../../../../../../probability.md) gives positive [probability](../../../../../../probability.md) of an [infinite percolation cluster](../../../../../../infinite-percolation-cluster.md), and [translation ergodicity of Bernoulli percolation](../../../../../../translation-ergodicity-of-bernoulli-percolation.md) then makes existence an almost-sure event. In question 2(b), $\theta$ means $\theta_2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
