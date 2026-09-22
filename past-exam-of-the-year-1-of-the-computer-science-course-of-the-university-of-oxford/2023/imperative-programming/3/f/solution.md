<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For each table index $b$, let $C_b=L(table(b))$ be the [set](../../../../../set-split.md) of non-null nodes reachable by following `next`. A sufficient [representation invariant](../../../../../representation-invariant.md) is:

- The [array](../../../../../array-data-structure.md) has exactly $N>0$ buckets, and every bucket heads a finite acyclic [linked list](../../../../../linked-list.md).
- The sets $C_b$ are pairwise disjoint, so one physical node cannot belong to two buckets.
- Every reachable node has a valid user identity, lies in bucket `hash(node.user)`, and has both counters between zero and `Int.MaxValue`.
- User identities are unique among all reachable nodes, not merely within a single chain.

The [abstraction function](../../../../../abstraction-function.md) maps these nodes to the total [functions](../../../../../function-split.md) of part (a): if the unique node for $u$ exists, $I(u)$ and $O(u)$ are its fields; otherwise both are zero. A stored record with two zero counters is harmless and has the same observable meaning as an absent record. This intentionally permits multiple concrete representations of the same abstract [program state](../../../../../program-state.md).

Initially every bucket is null, so the [representation invariant](../../../../../representation-invariant.md) holds and the [abstraction function](../../../../../abstraction-function.md) yields all zeros. The successful-update branch preserves every structural condition; the insertion branch creates a fresh node with a previously absent identity in its correct bucket. Both branches realize exactly the incoming-increment [postcondition](../../../../../postcondition.md), demonstrating [correct operations through an abstraction function](../../../../../correct-operations-through-an-abstraction-function.md).

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
