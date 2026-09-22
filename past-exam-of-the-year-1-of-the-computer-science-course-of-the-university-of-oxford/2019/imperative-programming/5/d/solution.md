<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Insert before the first entry that is at least the new value; equal values remain separate occurrences:
```
class ListPriorityQueue extends PriorityQueue[Int] {
  private var first: Node = null

  def clear(): Unit = { first = null }

  def isEmpty(): Boolean = first == null

  def insert(x: Int): Unit = {
    if (first == null || x <= first.value) {
      first = new Node(x, first)
    } else {
      var p = first
      while (p.next != null && p.next.value < x) {
        p = p.next
      }
      p.next = new Node(x, p.next)
    }
  }

  def delMin(): Int = {
    require(first != null, "Empty priority queue")
    val result = first.value
    first = first.next
    result
  }
}
```
In the scanning branch, the [loop invariant](../../../../../loop-invariant.md) says that `p` is reachable and all values from `first` through `p` are strictly smaller than `x`. The rest of the chain is unchanged and remains sorted. The [loop variant](../../../../../loop-variant.md) is the number of nodes after `p`. At exit either the next value is at least `x` or there is no next node, so inserting between `p` and `p.next` preserves the [representation invariant](../../../../../representation-invariant.md) and adds exactly one occurrence under the [abstraction function](../../../../../abstraction-function.md). The head branch covers an empty chain, a new minimum and equality with the old minimum. `delMin` returns the head's minimum value and removes exactly that occurrence.

**Insertion is $O(n)$ worst-case; `delMin`, `isEmpty` and the head-resetting `clear` are $O(1)$**. Reclaiming an abandoned chain later is garbage-collection work, not an explicit traversal performed by `clear`. Storage is $\Theta(n)$, including separate nodes for duplicate values. No fixed insertion-capacity [precondition](../../../../../precondition.md) has been added.

## ↑ Ancestors (12)

1. [D](../d.md)
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
