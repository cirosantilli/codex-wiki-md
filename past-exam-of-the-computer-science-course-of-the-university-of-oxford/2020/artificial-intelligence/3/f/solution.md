<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**The usual [alpha-beta pruning](../../../../../alpha-beta-pruning.md) inference fails because increasing B's [utility](../../../../../utility.md) need not decrease A's [utility](../../../../../utility.md).** A partially explored B-node may have found a child unfavorable to A, but B may prefer an unseen child favorable to A as well. An observed low A-coordinate therefore supplies no upper bound on the A-coordinate ultimately propagated by B.

For a concrete [counterexample](../../../../../counterexample.md), let a root A-node already have an alternative outcome $(1,0)$. In another B-node, the first explored child yields $(0,1)$. A zero-sum-style cutoff would discard its remaining children because $0<1$. But an unseen child with outcome $(100,2)$ is preferred by B, and makes the complete B-node return $(100,2)$, which A strictly prefers to its incumbent. Such a cutoff changes the answer.

The problem persists even after observing a large B-coordinate: without a known relation between coordinates or useful global [utility](../../../../../utility.md) bounds, an unseen pair may have still larger values for both players. Hence there is no generally valid ordinary scalar [alpha-beta pruning](../../../../../alpha-beta-pruning.md) rule for unrestricted [general-sum games](../../../../../general-sum-game.md). This does not rule out all [search pruning](../../../../../search-pruning.md): additional bounds, dominance information or a relationship between players' [utilities](../../../../../utility.md) can justify specific cutoffs, as in (g).

## ↑ Ancestors (11)

1. [F](../f.md)
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
