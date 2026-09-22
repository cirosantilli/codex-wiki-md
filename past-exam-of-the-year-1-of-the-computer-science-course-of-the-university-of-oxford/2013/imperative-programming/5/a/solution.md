<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [minimum stack](../../../../../minimum-stack.md): each [linked list node](../../../../../linked-list-node.md) caches the [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md) of all values from that node down to the bottom. This handles duplicate minima without searching when one is removed.
```
class Stack {
  private class Node(val value: Int, val least: Int, val next: Node)
  private var top: Node = null

  def push(x: Int): Unit = {
    val m = if (top == null) x else math.min(x, top.least)
    top = new Node(x, m, top)
  }

  def pop(): Int = {
    require(!isEmpty)
    val x = top.value
    top = top.next
    x
  }

  def isEmpty: Boolean = top == null

  def min: Int = {
    require(!isEmpty)
    top.least
  }
}
```
The [representation invariant](../../../../../representation-invariant.md) is that the chain from `top` is finite and acyclic, and every reachable node `q` satisfies

$$
q.least=\begin{cases}q.value&q.next=null,\\\min(q.value,q.next.least)&q.next\ne null.\end{cases}
$$

The [abstraction function](../../../../../abstraction-function.md) takes the values along this chain in top-to-bottom order. Thus pushing $x$ changes $s$ to $x:s$, and popping a nonempty $s$ returns its head and leaves its tail. The cached-minimum equation follows for a new node from the previously valid chain; removing a head leaves every surviving equation unchanged. Consequently

$$
\boxed{push,pop,isEmpty,min\text{ each take }O(1)\text{ worst-case time}.}
$$

The bounds use the usual constant-cost allocation and [integer arithmetic](../../../../../integer-arithmetic.md) model. Storage is linear in the number of entries. `min` and `pop` require a nonempty [stack](../../../../../stack-data-structure.md); `min` leaves it unchanged.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
