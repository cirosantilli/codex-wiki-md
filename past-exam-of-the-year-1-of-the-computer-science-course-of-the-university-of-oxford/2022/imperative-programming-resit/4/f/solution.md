<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Append nonzero entries in increasing index order; repeatedly calling `setElement` would unnecessarily rescan earlier entries and could make construction quadratic.

```
def makeVector(elems: Array[Double]): Node = {
  require(elems != null)
  val head = makeZeroVector(elems.length)
  var tail = head
  var i = 0
  while (i < elems.length) {
    val v = elems(i)
    require(!v.isNaN && !v.isInfinity)
    if (v != 0.0) {
      val fresh = new Node(v, i, tail, head)
      tail.next = fresh
      head.prev = fresh
      tail = fresh
    }
    i += 1
  }
  head
}
```

The [loop invariant](../../../../../loop-invariant.md) says that the list represents exactly the nonzero entries of the processed input prefix, in their original coordinate order, and `tail` is the final node or the header when none exist. Every append preserves the cycle and ordering. At exit, all input coordinates have their intended values. **Construction takes $O(n)$ time and $O(k)$ data nodes**, where $n$ is the [array](../../../../../array-data-structure.md) length and $k$ the number of nonzeros, plus one header. The input [array](../../../../../array-data-structure.md) is unchanged.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [4](../../4.md)
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
