<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**[Depth-first search](../../../../../depth-first-search.md) computes [minimax search](../../../../../minimax-search.md) values with much less live storage and naturally supports [alpha-beta pruning](../../../../../alpha-beta-pruning.md).** A parent's value needs only its current best child value and the next child to visit. Once a child subtree has been evaluated, its internal [search nodes](../../../../../search-node.md) can be discarded; a final value cannot usually be computed from a nonterminal frontier alone.

With [branching factor](../../../../../branching-factor.md) $b$ and horizon $d$, [breadth-first search](../../../../../breadth-first-search.md) stores a frontier of order $b^d$. A [depth-first search](../../../../../depth-first-search.md) implementation storing sibling lists uses $O(bd)$ [space complexity](../../../../../space-complexity.md); lazy successor generation can reduce this to $O(d)$ frames plus game-state storage. Both unpruned traversals have $O(b^d)$ [time complexity](../../../../../time-complexity.md) for $b>1$. [Depth-first search](../../../../../depth-first-search.md) also supplies a completed sibling outcome early, allowing [alpha-beta pruning](../../../../../alpha-beta-pruning.md) to reject later subtrees before generating them.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
