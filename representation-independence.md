# Representation independence

↑ **Parent:** [Encapsulation (computer programming)](encapsulation-computer-programming.md)

[Representation independence](representation-independence.md) means that clients restricted to the promised [API](application-programming-interface.md) cannot distinguish implementations by the specified results and state transitions. State what observations count: equal returned labels and failure statuses do not imply equal running times, allocations or physical layouts. If the [API](application-programming-interface.md) also promises a resource bound, a replacement must meet that bound too.

Replace the compact [array](array-data-structure.md) in the [bounded queue with encapsulation](bounded-queue-with-encapsulation.md) by a [circular buffer](circular-buffer.md) with storage $B$, front index $h$ and count $n$. Its [representation invariant](representation-invariant.md) is $|B|=C$, $h,n\in\mathbb Z$, $0\leq h<C$ and $0\leq n\leq C$. Its [abstraction function](abstraction-function.md) reads the occupied slots using [modular arithmetic](modular-arithmetic.md):

$$
\alpha(B,h,n)=\bigl(B_{(h+i)\bmod C}\bigr)_{i=0}^{n-1}.
$$

On successful `enqueue(x)`, write $B_{(h+n)\bmod C}=x$ and increment $n$. On successful `dequeue()`, return $B_h$, replace $h$ by $(h+1)\bmod C$ and decrement $n$. Full and empty failures do not alter storage. `peek` and `size` have the same abstract meanings as before. Keeping a count distinguishes a full [circular buffer](circular-buffer.md) from an empty one even when both would have the same next insertion index.

<a id="image-the-same-bounded-queue-trace-uses-shifting-array-storage-or-a-wrapping-circular-buffer"></a>
![](queue-array-ring-representation-trace.png)

**[Figure 10](#image-the-same-bounded-queue-trace-uses-shifting-array-storage-or-a-wrapping-circular-buffer). The same bounded queue trace uses shifting array storage or a wrapping circular buffer**.

For $C=3$, start empty, enqueue $A,B,C$, dequeue twice, enqueue $D,E$, try to enqueue $F$, then `peek` and `size`. Both implementations return $A,B$ from the removals, report `full` for $F$, and finish with front $C$, size three and abstract [sequence](sequence.md) $(C,D,E)$. The compact [array](array-data-structure.md) stores $(C,D,E)$ from index zero; the [circular buffer](circular-buffer.md) stores $(D,E,C)$ with $h=2$. Their [abstraction functions](abstraction-function.md) explain why different stored entries describe the same ordered content.

Under constant-cost slot access and index arithmetic, with no resizing and labels that fit in one slot, the compact [array](array-data-structure.md) does $n-1$ slot moves on a successful removal: $O(n)$ worst-case [time complexity](time-complexity.md) as capacity varies. The [circular buffer](circular-buffer.md) does no slot moves and uses $O(1)$ worst-case [time complexity](time-complexity.md) for all four operations. Both allocate $C$ slots initially; that construction cost is separate. These are operation-count claims in [Big O notation](big-o-notation.md), not measured timings. The short correctness outline checks that each implementation's [abstraction function](abstraction-function.md) produces the specified new [sequence](sequence.md) and return value after every successful or rejected call. Repeating that check gives equal traces for clients using only this [API](application-programming-interface.md).

## ↑ Ancestors (3)

1. [Encapsulation (computer programming)](encapsulation-computer-programming.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Circular buffer](circular-buffer.md)
- [Encapsulation (computer programming)](encapsulation-computer-programming.md)
- [Representation independence](representation-independence.md)
