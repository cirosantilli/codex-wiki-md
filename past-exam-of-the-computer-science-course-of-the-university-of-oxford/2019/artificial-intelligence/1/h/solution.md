<h1 id="1/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Use [incremental belief-state search](../../../../../incremental-belief-state-search.md) to find only the initial possibilities needed to constrain a successful [plan](../../../../../plan.md). Choose one possible initial state, or a small [subset](../../../../../subset.md) $B_0$ of the full initial [belief state](../../../../../belief-state.md) $B$. Find an action [sequence](../../../../../sequence.md) solving this restricted problem, then simulate it from every state in $B$.

If validation succeeds, return the candidate. Otherwise choose a state that makes some action inapplicable or ends outside the goal, add it to $B_0$, and search again for a [plan](../../../../../plan.md) that works for every selected state. Replanning can revise the earlier [sequence](../../../../../sequence.md); merely appending a repair to one arbitrary candidate can miss solutions. For a finite initial [belief state](../../../../../belief-state.md), there are at most $|B|$ additions before every initial possibility has been included. If a complete restricted solver proves that even the selected [subset](../../../../../subset.md) is unsolvable, part (g) shows that the full problem is unsolvable.

The benefits are smaller intermediate [belief states](../../../../../belief-state.md), fewer states propagated through candidate actions, and avoidance of unnecessary portions of the full [power set](../../../../../power-set.md) search space. One physical-state counterexample can eliminate many invalid candidates. The worst case can still require all initial states; the method exploits instances where a few representative possibilities already force a [plan](../../../../../plan.md) that passes universal validation.

## ↑ Ancestors (11)

1. [H](../h.md)
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
