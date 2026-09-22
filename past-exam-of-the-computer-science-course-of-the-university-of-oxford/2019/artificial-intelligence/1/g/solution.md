<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

For an action [sequence](../../../../../sequence.md) $\pi$, let $T_\pi(B)$ be the [set](../../../../../set-split.md) of all physical states obtainable by applying it to the initial [belief state](../../../../../belief-state.md) $B$. Under a deterministic model this is an image; for nondeterministic outcomes it is the [union](../../../../../set-union.md) of all permitted images. For $B'\subseteq B$,

$$
T_\pi(B')\subseteq T_\pi(B).
$$

If each action is applicable to every current possibility from $B$, it is also applicable to every possibility from $B'$. If the final [belief state](../../../../../belief-state.md) for $B$ is contained in the physical goal [set](../../../../../set-split.md) $G$, then $T_\pi(B')\subseteq G$. Thus **the same [plan](../../../../../plan.md) solves every [subset](../../../../../subset.md) of $B$**.

Nothing comparable follows for an arbitrary [superset](../../../../../superset.md). For example, let an action take $s_1$ to a goal and leave $s_2$ at a non-goal. It solves $\{s_1\}$ but not $\{s_1,s_2\}$. A larger [belief state](../../../../../belief-state.md) is solved by this particular [sequence](../../../../../sequence.md) exactly when all added states also permit it and end in $G$. It may succeed on some [supersets](../../../../../superset.md) and fail on others; it cannot be guaranteed merely from success on $B$.

## ↑ Ancestors (11)

1. [G](../g.md)
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
