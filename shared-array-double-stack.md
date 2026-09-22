# Shared-array double stack

↑ **Parent:** [Stack (data structure)](stack-data-structure.md)

Two [stacks](stack-data-structure.md) can share a fixed [array](array-data-structure.md) by growing inwards from opposite ends. Store one [stack](stack-data-structure.md) in $[0,l)$ and the other in $[r,M)$, with [representation invariant](representation-invariant.md) $0\leq l\leq r\leq M$. The first top is at $l-1$, the second at $r$, and $[l,r)$ is free. The [abstraction function](abstraction-function.md) reads the first segment backwards and the second forwards to obtain top-first [lists](list-abstract-data-type.md). Push requires $l<r$; a pop requires its own [stack](stack-data-structure.md) to be nonempty. Every operation uses constant time, and either [stack](stack-data-structure.md) can use all remaining space. The bounded [abstract data type](abstract-data-type.md) must expose or specify the shared capacity restriction.

## ↑ Ancestors (4)

1. [Stack (data structure)](stack-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
