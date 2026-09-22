<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the heap-numbered binary tree with root label zero and children $2k+1,2k+2$. Its strict descendants in [breadth-first search](../../../../../../breadth-first-search.md) order are **$1,2,3,\ldots$**. A machine-safe `Node[Int]` version stops at the largest representable label:

```
class NumberNode(val label: Int) extends Node[Int] {
  require(label >= 0)
  def children(): Iter[Node[Int]] = new Iter[Node[Int]] {
    private var candidate = 2L * label.toLong + 1L
    private val last = candidate + 1L
    def hasNext: Boolean = candidate <= last && candidate <= Int.MaxValue
    def next(): Node[Int] = {
      require(hasNext)
      val answer = new NumberNode(candidate.toInt)
      candidate += 1L
      answer
    }
  }
}

val traversal = breadthFirst(new NumberNode(0))
var expected = 1
while (expected <= 1000) {
  assert(traversal.hasNext)
  assert(traversal.next().label == expected)
  expected += 1
}
```

The arithmetic is widened before computing child labels, so no negative wrapped labels occur. Repeated `hasNext` calls should not skip nodes; a leaf root should produce immediate exhaustion, and uneven finite trees should retain sibling order across parents. A fresh second traversal should start again at one.

Literal unbounded increase is impossible with the bounded `Int` type. For a genuinely infinite test, change the label and child arithmetic to `BigInt`; the same construction then has no representational endpoint. The shown finite-prefix test already exercises lazy traversal without allocating the entire very large `Int`-labelled tree.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
