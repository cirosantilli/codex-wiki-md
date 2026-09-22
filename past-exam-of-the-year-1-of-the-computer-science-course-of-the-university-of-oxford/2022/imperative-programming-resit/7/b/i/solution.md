<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Keep a [FIFO queue](../../../../../../fifo-queue.md) of pending child [iterators](../../../../../../iterator.md), ordered by the breadth-first order of their parents. Defer even the call creating a node's children until that [iterator](../../../../../../iterator.md) reaches the front and is needed:

```
def breadthFirst[T](node: Node[T]): Iter[Node[T]] = {
  def childrenLater(n: Node[T]): Iter[Node[T]] = new Iter[Node[T]] {
    private lazy val children = n.children()
    def hasNext: Boolean = children.hasNext
    def next(): Node[T] = {
      require(children.hasNext, "empty child iterator")
      children.next()
    }
  }

  val pending = scala.collection.mutable.Queue.empty[Iter[Node[T]]]
  pending.enqueue(childrenLater(node))

  new Iter[Node[T]] {
    private def normalize(): Unit = {
      while (pending.nonEmpty && !pending.head.hasNext) pending.dequeue()
    }
    def hasNext: Boolean = {
      normalize()
      pending.nonEmpty
    }
    def next(): Node[T] = {
      normalize()
      require(pending.nonEmpty, "no more descendants")
      val answer = pending.head.next()
      pending.enqueue(childrenLater(answer))
      answer
    }
  }
}
```

Here **“descendants” excludes the supplied root**: the first output is its first child. A self-inclusive convention can prepend `unitIter(node)` without changing the traversal logic. The queue invariant says its [iterators](../../../../../../iterator.md) enumerate the still-unreported children of already encountered parents, in parent breadth-first order. Consuming one child appends that child's deferred [iterator](../../../../../../iterator.md) after all earlier parents' pending children. Exhausted child [iterators](../../../../../../iterator.md) contribute nothing and can be discarded. This proves increasing depth and sibling order without constructing a complete level in advance.

This [lazy breadth-first traversal with child iterators](../../../../../../lazy-breadth-first-traversal-with-child-iterators.md) never eagerly materializes all children or the whole tree. A finite prefix can therefore be traversed on a genuinely infinite tree. As with any strict breadth-first ordering, an infinite earlier level prevents reaching a deeper level; no algorithm can place a deeper node after every member of an infinite earlier level at a finite output position. For a [locally finite tree](../../../../../../locally-finite-tree.md), every finite-depth level is finite and each descendant is eventually reached, assuming the underlying [iterator](../../../../../../iterator.md) operations terminate. Fresh child [iterators](../../../../../../iterator.md) and exclusive ownership of consumed [iterator](../../../../../../iterator.md) states are essential to this argument.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
