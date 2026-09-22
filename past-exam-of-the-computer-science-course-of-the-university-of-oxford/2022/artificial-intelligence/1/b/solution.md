<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Three different omissions produce concrete erroneous [STRIPS](../../../../../strips.md) plans. Here a route means the corresponding successive $\operatorname{Move}$ actions with the indicated first argument.

**No lethal-entry condition.** Move the agent along $s_{11},s_{21},s_{22},s_{23},s_{13}$, take the gold at $s_{13}$, and reverse the route. This nine-action [STRIPS](../../../../../strips.md) plan satisfies every supplied [precondition](../../../../../precondition.md) and the final [goal test](../../../../../goal-test.md), without firing. Physically it fails on entering the live monster’s room: the supplied [search transition model](../../../../../search-transition-model.md) neither forbids the entry nor records death. The omitted pit cell happens to be disconnected in the supplied adjacency relation, so this particular instance already excludes pit entry; that accidental protection does not encode the monster hazard.

**Supposedly stationary objects can move themselves.** The five-action [STRIPS](../../../../../strips.md) plan

$$
\begin{aligned}
&\operatorname{Move}(g,s_{13},s_{23}),\quad\operatorname{Move}(g,s_{23},s_{22}),\\
&\operatorname{Move}(g,s_{22},s_{21}),\quad\operatorname{Move}(g,s_{21},s_{11}),\\
&\operatorname{Take}(a,g,s_{11})
\end{aligned}
$$

leaves the agent at the exit and brings it the gold. The formal [preconditions](../../../../../precondition.md) hold because $x$ in $\operatorname{Move}(x,y,z)$ has no actor restriction. Gold cannot actually propel itself. The same flaw permits moving the supposedly stationary monster.

**Unrestricted pickup permits impossible inventory.** Follow the first example’s outward route, but insert $\operatorname{Take}(a,w,s_{23})$ immediately after reaching $s_{23}$. Continue to $s_{13}$, take the gold and return. This ten-action [STRIPS](../../../../../strips.md) plan ends with both $\operatorname{have}(a,w)$ and $\operatorname{have}(a,g)$ and satisfies the supplied goal. Its entrance also exposes the first flaw, but the additional, distinct defect is that pickup treats the live monster as a collectible object and deletes its location. A movement safety check alone is not a specification of which objects are collectible. The shot schema likewise lacks restrictions to the designated shooter, projectile and victim; fixing the action roles together prevents these type errors.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
