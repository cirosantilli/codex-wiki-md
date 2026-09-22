<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**With the conventional strictly positive step costs, the five answers in printed order are false, false, true, true, true.** The third answer needs that positivity convention: it is false in general if zero-cost [edges](../../../../../edge-of-a-graph.md) and unrestricted ties are admitted. Take the [goal test](../../../../../goal-test.md) on selection from the [search frontier](../../../../../search-frontier.md), and assume a finite reachable problem with a reachable [goal state](../../../../../goal-state.md); finite [branching factor](../../../../../branching-factor.md) and a positive lower bound on step costs give the corresponding [tree search](../../../../../tree-search.md) guarantees on an infinite problem. These assumptions make the usual [A-star search](../../../../../a-star-search.md) guarantees precise.[§4.1, printed pp. 94–100: best-first priorities, consistency and optimality conditions](../../../../../informed-search-and-exploration-by-stuart-russell-and-peter-norvig.md)

For the first assertion, use a [directed graph](../../../../../directed-graph.md) with transitions $s\to t$ of cost $10$, $s\to x$ of cost $1$ and $x\to t$ of cost $1$, where $t$ is the only [goal state](../../../../../goal-state.md). The [perfect heuristic](../../../../../perfect-heuristic.md) is $h^*(s)=2$, $h^*(x)=1$, $h^*(t)=0$. [Greedy best-first search](../../../../../greedy-best-first-search.md) selects the direct goal of cost $10$ because its priority is zero. The least [path cost](../../../../../path-cost.md) is $2$. Knowing the exact remaining distance does not account for an expensive transition already taken.

The same [counterexample](../../../../../counterexample.md) settles the second assertion. [Greedy best-first search](../../../../../greedy-best-first-search.md) selects $s,t$, while [A-star search](../../../../../a-star-search.md) selects $s,x,t$: after expanding $s$, the [A-star search](../../../../../a-star-search.md) priorities are $2$ for $x$ and $10$ for the direct copy of $t$. Thus even the expanded state [sets](../../../../../set-split.md) differ.

For the third assertion, let the current nonterminal [search node](../../../../../search-node.md) have finite remaining distance $h^*(s)$. The first transition of a least-cost continuation has some successor $s'$ with

$$
h^*(s)=c(s,s')+h^*(s')>h^*(s').
$$

Every older entry in the [search frontier](../../../../../search-frontier.md) has estimate at least $h^*(s)$, since the current entry was selected with minimum estimate. A newly generated successor with strictly smaller estimate therefore wins over every older entry. Whichever new successor is selected has smaller remaining distance than the current [search node](../../../../../search-node.md), so the argument repeats. Consequently the selected [search nodes](../../../../../search-node.md) form one parent–child chain; include the selected goal, or append it if “expanded” excludes goal processing. This [greedy perfect-heuristic descent](../../../../../greedy-perfect-heuristic-descent.md) does not imply least [path cost](../../../../../path-cost.md), as the first [counterexample](../../../../../counterexample.md) demonstrates.

The zero-cost qualification is substantive. Give $s$ two successors $a,b$ of cost $1$, add $a\to x$ of cost $0$, and add $x\to t$ and $b\to t$ of cost $1$. The [perfect heuristic](../../../../../perfect-heuristic.md) has values $2$ at $s$, $1$ at $a,b,x$ and $0$ at $t$. Alphabetical priority ties let [greedy best-first search](../../../../../greedy-best-first-search.md) select $s,a,b,t$, which is not one [graph path](../../../../../path-in-a-graph.md). Thus the unqualified third assertion requires a cost or tie convention absent from the printed text.

For the fourth assertion, a least remaining distance satisfies

$$
h^*(s)\le c(s,s')+h^*(s')
$$

on every [edge](../../../../../edge-of-a-graph.md), by taking that [edge](../../../../../edge-of-a-graph.md) and then a least-cost continuation. Thus $h^*$ is a [consistent heuristic](../../../../../consistent-heuristic.md). The usual [A-star search](../../../../../a-star-search.md) [graph search](../../../../../graph-search.md) finalizes each expanded state's least [path cost](../../../../../path-cost.md) and returns a least-cost goal.

For the fifth assertion, write $C^*=h^*(s_0)$. Before a goal is selected, an unexpanded prefix of an optimal [graph path](../../../../../path-in-a-graph.md) remains on the [search frontier](../../../../../search-frontier.md), with $f=g+h^*=C^*$. [A-star search](../../../../../a-star-search.md) therefore selects only [search nodes](../../../../../search-node.md) with $f\le C^*$. Since $g\ge0$,

$$
\boxed{h^*(n)\le g(n)+h^*(n)\le C^*=h^*(s_0).}
$$

This compares remaining cost, not [search depth](../../../../../search-depth.md) or accumulated [path cost](../../../../../path-cost.md). The statement can fail with negative costs; those are outside the convention used here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
