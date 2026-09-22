<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Use **[AND-OR search](../../../../../and-or-search.md) for a [strong plan](../../../../../strong-plan.md)**. At an OR node choose a joint action; at its AND node require successful continuations for every possible outcome. A repeated state on the current branch cannot by itself establish progress. On a finite [state space](../../../../../state-space.md), the equivalent [strong planning winning-set iteration](../../../../../strong-planning-winning-set-iteration.md) starts with $W_0=\{(p,p):p\in C\}$ and repeatedly adds states with an action whose nonempty outcome [set](../../../../../set-split.md) is contained in the current winning [set](../../../../../set-split.md):

$$
W_{t+1}=W_t\cup\{s:\exists a,\ \varnothing\ne\operatorname{Results}(s,a)\subseteq W_t\}.
$$

A newly admitted state has a plan with at most $t+1$ remaining steps in the worst case. This [algorithm](../../../../../algorithm-split.md) terminates on the finite [state space](../../../../../state-space.md) and is complete for finite guaranteed-success plans. In a general [nondeterministic planning](../../../../../nondeterministic-planning.md) problem it cannot guarantee that a [strong plan](../../../../../strong-plan.md) exists: an uncontrollable self-loop can prevent inevitable progress.

**For this particular unobstructed grid, a [strong plan](../../../../../strong-plan.md) does exist.** Command Mr Robot to wait throughout and move Mrs Robot along a shortest route to his initial room. Her movement is deterministic and his waiting is unaffected by the horizontal uncertainty. This meets in $D(p_0,q_0)$ steps, regardless of every uncertain outcome, because no uncertain command is used. Thus a complete finite [AND-OR search](../../../../../and-or-search.md) will find a solution here. With an unspecified disconnected maze, existence would instead require both robots to lie in the same reachable [graph component](../../../../../component-graph-theory.md).

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
