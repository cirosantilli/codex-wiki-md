<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Two general constructions are **[delete-relaxation heuristics](../../../../../delete-relaxation-heuristic.md)** and **[abstraction heuristics](../../../../../abstraction-heuristic.md)**. Both obtain an [admissible heuristic](../../../../../admissible-heuristic.md) by solving a problem in which every original [plan](../../../../../plan.md) remains available at no greater cost.

For a [delete-relaxation heuristic](../../../../../delete-relaxation-heuristic.md), remove every [STRIPS](../../../../../strips.md) delete effect and compute the shortest relaxed [plan](../../../../../plan.md) length $h^+(S)$. A relaxed action never makes a true fact false. Inductively, executing an original [plan](../../../../../plan.md) in the relaxed model leaves a superset of its original facts, so positive [preconditions](../../../../../precondition.md) and the positive conjunctive goal remain satisfied. Therefore

$$
\boxed{h^+(S)\le h^*(S).}
$$

The exact relaxed optimum can itself be expensive to find; merely taking the length of an arbitrary relaxed [plan](../../../../../plan.md) does not guarantee an [admissible heuristic](../../../../../admissible-heuristic.md). One can instead use a proven lower bound on the relaxed optimum.

For this coin encoding, removing delete effects loses the requirement to free an occupied stack and the requirement to destroy and later rebuild support relations. From the initial state, relaxed moves can successively move $c_1,c_2,\ldots,c_n$ from $s_1$ to $s_2$ using the empty-destination action: $\operatorname{Topmost}(g,s_2)$ is never deleted, and exposing each next source coin is still allowed. The original support-chain goal facts are never deleted either. After these $n$ actions, $\operatorname{Topmost}(g,s_1)$ and $\operatorname{Topmost}(c_1,s_2)$ also hold, so the entire goal from part (a) holds. Thus $h^+(I)\le n$, showing why this relaxation misses much of the exponential work needed with three stacks.

For an [abstraction heuristic](../../../../../abstraction-heuristic.md), project states onto selected information and project each action onto its effect on that information. Forgetting a selected collection of [planning fluents](../../../../../planning-fluent.md), and their [preconditions](../../../../../precondition.md) and goals, gives one general construction for [STRIPS](../../../../../strips.md). Define the abstract transition relation to include every projected original transition, with cost at most the original cost. The exact abstract distance is then a lower bound because any original goal-reaching [graph path](../../../../../path-in-a-graph.md) projects to an abstract goal-reaching walk:

$$
\boxed{h_{\mathrm{abs}}(S)\le h^*(S).}
$$

For the coin puzzle, a useful state abstraction remembers the stacks occupied by a chosen subset of coins and ignores the other coins, contracting the support chains past ignored coins. Moving an ignored coin leaves the abstract state unchanged; moving a retained coin is a legal move in the smaller [Tower of Hanoi](../../../../../tower-of-hanoi.md) instance. Precomputing exact abstract goal distances gives a [pattern database](../../../../../pattern-database.md). This can retain stacking and spare-stack restrictions that the [delete-relaxation heuristic](../../../../../delete-relaxation-heuristic.md) loses. Larger retained subsets give potentially stronger information but require more storage and preprocessing. Maxima of these [admissible heuristics](../../../../../admissible-heuristic.md) remain safe; unqualified sums can double-count moves.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Intelligent systems](../../../intelligent-systems-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
