<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use one real [linked list node](../../../../../linked-list-node.md) per occurrence, with a private reference to the first:
```
class Node(val value: Int, var next: Node)

// Inside the queue implementation:
private var first: Node = null
```
The [representation invariant](../../../../../representation-invariant.md) says that the reachable chain is finite, acyclic and nondecreasing in `value`, and is owned by the queue. Equal adjacent values are explicitly allowed. The [abstraction function](../../../../../abstraction-function.md) is the [multiset](../../../../../multiset.md) containing one occurrence of `v.value` for every reachable real [linked list node](../../../../../linked-list-node.md) `v`. Initially `first==null` represents the empty [multiset](../../../../../multiset.md). No artificial smallest `Int` is needed as a sentinel, and `Int.MinValue` remains a valid real value.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
