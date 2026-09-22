<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**All three variants are [complete search algorithms](../../../../../complete-search-algorithm.md) under the usual finite-[branching factor](../../../../../branching-factor.md), nonnegative-[heuristic function](../../../../../heuristic-function.md) assumptions.** Here $0\le h\le h^*$, with zero at goals; the supplied positive lower bound on step costs is also essential. The root is processed once before a parent-dependent priority is needed.[section 4.1, printed p. 100, footnote 4, finiteness and positive step costs](../../../../../informed-search-and-exploration-by-stuart-russell-and-peter-norvig.md) Completeness means finding a solution if one exists, not necessarily terminating when none exists.

Fix a finite solution path. Every [search node](../../../../../search-node.md) on that path has a finite priority, so let $K$ bound all of its relevant priorities. For ordinary [A-star search](../../../../../a-star-search.md) and the second variant, the priority is at least $g(n)$. Thus any [search node](../../../../../search-node.md) with priority at most $K$ has depth at most $\lfloor K/\epsilon\rfloor$. In the third variant the priority is at least $g(n')$, so its depth is at most $\lfloor K/\epsilon\rfloor+1$. A finitely branching [search tree](../../../../../search-tree.md) has finitely many [search nodes](../../../../../search-node.md) at these depths. Therefore finitely many earlier [search nodes](../../../../../search-node.md) can delay each successive [search node](../../../../../search-node.md) on the chosen solution path; eventually its goal is generated or selected, as appropriate.

Moving the [goal test](../../../../../goal-test.md) to generation cannot destroy that existence guarantee, although it can destroy optimality. Likewise the altered parent-dependent priorities remain bounded below by the accumulated cost to the [search node](../../../../../search-node.md) or its parent, which is enough for this completeness argument. If “admissible” were interpreted to allow arbitrarily negative estimates, the lower-bound argument would need an additional hypothesis; the conventional nonnegative interpretation is being used explicitly. For the literal upper-bound-only interpretation, all three can fail completeness: attach an infinite unit-cost dead-end chain with $g(n_d)=d$ and $h(n_d)=-2d$ beside a finite goal branch beginning with a cost-$3$ edge and estimate zero. Its successive low priorities can starve the finite branch. Every negative chain estimate is still at most its infinite true remaining cost.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
