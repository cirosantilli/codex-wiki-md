<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A useful starting model treats a road network as a directed [flow network](../../../../../../flow-network.md) and travelers as a divisible population in a [nonatomic congestion game](../../../../../../nonatomic-congestion-game.md): an individual traveler has negligible effect on link congestion. For each source-sink pair $k$, fix a demand $d_k$ and a finite set $\mathcal P_k$ of allowed routes. Let $f_p\geq0$ be the flow on route $p$, with $\sum_{p\in\mathcal P_k}f_p=d_k$. The [link-route incidence matrix](../../../../../../link-route-incidence-matrix.md) $A$ gives link loads $v=Af$. If link $e$ has delay $\ell_e(v_e)$, the route travel time is

$$
L_p(f)=\sum_{e\in p}\ell_e(v_e).
$$

A [Wardrop equilibrium](../../../../../../wardrop-equilibrium.md) is a feasible route-flow vector for which every used route has minimum travel time among the routes serving the same source-sink pair. Equivalently, there are numbers $\lambda_k$ such that

$$
\boxed{L_p(f)\geq\lambda_k\quad(p\in\mathcal P_k),\qquad f_p>0\Longrightarrow L_p(f)=\lambda_k.}
$$

The condition says that a traveler cannot lower their own delay by changing route. It does not assert that their choice minimizes the total delay experienced by all travelers. At a [Wardrop equilibrium](../../../../../../wardrop-equilibrium.md), unused routes may have exactly the same delay as used ones.

This static [flow network](../../../../../../flow-network.md) model requires delay to depend on present link load, with each source-sink demand fixed. Models from [queueing theory](../../../../../../queueing-theory-split.md) instead describe vehicles or packets as discrete customers whose delay depends on random arrivals, service and accumulated queues; a time-dependent model must also track changes of flow and travel-time propagation. Those models answer different questions from a static [Wardrop equilibrium](../../../../../../wardrop-equilibrium.md). The static model is nevertheless valuable because its route-choice condition has a precise [convex optimization](../../../../../../convex-optimization-split.md) formulation, as developed next.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
