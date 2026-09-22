<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The following class uses the node type supplied in the paper:
```
class DoublyLinkedDoubleEndedQueue extends DoubleEndedQueue {
  private var first: Node = null
  private var last: Node = null

  def isEmpty: Boolean = first == null

  def addLeft(x: Int): Unit = {
    val node = new Node(x, null, first)
    if (first == null) last = node
    else first.prev = node
    first = node
  }

  def addRight(x: Int): Unit = {
    val node = new Node(x, last, null)
    if (last == null) first = node
    else last.next = node
    last = node
  }

  def getLeft(): Int = {
    require(!isEmpty)
    val old = first
    first = old.next
    if (first == null) last = null
    else first.prev = null
    old.next = null
    old.datum
  }

  def getRight(): Int = {
    require(!isEmpty)
    val old = last
    last = old.prev
    if (last == null) first = null
    else last.next = null
    old.prev = null
    old.datum
  }
}
```
An insertion connects a fresh endpoint to the old chain and updates its [reciprocal](../../../../../multiplicative-inverse.md) link. A removal reconnects the exposed endpoint to null; the singleton case also clears the opposite endpoint. The remaining chain therefore satisfies the same [representation invariant](../../../../../representation-invariant.md) and has exactly the abstract [sequence](../../../../../sequence.md) required by the specification. **Every operation performs $O(1)$ pointer work**, excluding allocation costs for a newly added node.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
