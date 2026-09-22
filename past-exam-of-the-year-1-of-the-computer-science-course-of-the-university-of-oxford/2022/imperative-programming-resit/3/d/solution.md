<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [trait](../../../../../trait.md) and node definition above. The reference to a “stack” in this part is a wording error: the declared class and operations implement a [FIFO queue](../../../../../fifo-queue.md).

```
class ListQueue extends Queue[Int] {
  private var first: QueueNode = null
  private var last: QueueNode = null
  private var size = 0

  def enqueue(x: Int): Unit = {
    require(size < Int.MaxValue, "queue size limit")
    val fresh = new QueueNode(x, null)
    if (last == null) first = fresh
    else last.next = fresh
    last = fresh
    size += 1
  }

  def dequeue(): Int = {
    require(first != null, "empty queue")
    val answer = first.value
    first = first.next
    size -= 1
    if (first == null) last = null
    answer
  }

  def clear(): Unit = {
    first = null
    last = null
    size = 0
  }

  def isEmpty: Boolean = size == 0
  def length: Int = size
}
```

Appending links the fresh node after the old tail, or establishes both endpoints when empty. Removing the head preserves the tail unless the final node was removed, in which case both endpoints become null. Clearing only discards the endpoint references; it need not visit or overwrite unreachable nodes. Thus all operations are **$O(1)$ in the usual pointer-operation/allocation cost model**, with later [garbage collection](../../../../../garbage-collection.md) excluded from an individual operation's bound. The [representation invariant](../../../../../representation-invariant.md) and [abstraction function](../../../../../abstraction-function.md) show the specified [sequence](../../../../../sequence.md) changes, including empty/singleton transitions.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
